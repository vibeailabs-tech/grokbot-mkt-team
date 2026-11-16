# Hệ thống marketing

Cấu trúc gốc là repo Hermes bốn vai. Bản này đã sửa theo bài [How to Build an AI Marketing Team with Grok Bot](https://espressio.ai/blog/ai-marketing-team-grok-bot/) của Espressio, 8/11/2026.

Lấy từ bài đó:

- Não công ty nằm trong `company/`, não từng việc nằm trong `campaigns/<id>/`.
- Sáu vai khởi đầu: Lead, Research, Content, SEO, Report, Review. Paid chưa thành bot.
- Trong nhóm chỉ `@` một Bot, vì nếu không thì các Bot cùng trả lời và cùng tốn usage.
- Research ghi những gì người đã biết trước khi mở trang. Mỗi sự thật có nguồn, cái đang thấy, vì sao quan trọng, và ngày.
- Content chờ `Góc người` trong meta. Lý do từ chối một bài nằm ở `company/vi-du.md`.
- Phiếu `duyet.md` có hiện trạng, việc đề xuất, nguồn, cách lùi lại, và ba lựa chọn duyệt, sửa, từ chối.

Không lấy kho dữ liệu, Herdr, hay worker CLI. Chưa có số liệu thì không giả là đã nối. Report chỉ đọc file trong campaign.

## Đường đi

```text
Người nói những gì mình đã biết
  ▼
Lead mở campaigns/<id>/ và @Research hoặc @SEO hoặc @Report
  ▼
Lead hỏi góc, ghi vào meta
  ▼
@Content hoặc @SEO viết drafts/
  ▼
@Review viết review.md và duyet.md
  ▼
Người chọn duyệt, sửa, hoặc từ chối ở chat riêng với Lead
  ▼
Bản duyệt nằm ở ket-qua/da-duyet/    người tự đăng
```

Tối đa hai vòng sửa. Nhóm không hiện thẻ duyệt, nên phiếu người ký vẫn ở chat riêng.

## Sáu Bot

| Bot | Việc | Không được |
|---|---|---|
| Lead | Mở campaign, `@` một Bot, giữ phiếu | Viết bài, đăng |
| Research | Brief, đối thủ, audit nhìn thấy | Viết bài, thứ hạng |
| Content | Social, email, trang, theo góc đã chọn | Viết khi chưa có góc, đăng |
| SEO | Bản sửa trang và câu hỏi chưa trả lời | Đăng, bịa hạng |
| Report | Báo cáo từ file có sẵn | Bịa số, đề xuất chi |
| Review | Checklist và `duyet.md` | Sửa hộ, quá 2 vòng |

Chi tiết cài nằm ở `docs/cai-dat.md`. Hồ sơ thương hiệu trong `company/thuong-hieu.md` vẫn đang trống.

## Ba routine

Múi giờ `Asia/Ho_Chi_Minh`. Lead sở hữu cả ba. Lời giao nằm ở `routines/lead.md`. Tuần đầu không đặt lịch dày hơn các mốc đó.

Routine trên Grok Bot trừ usage. Repo Hermes dùng cron không tốn token. Bản này không có đường đó. Routine mới không chạy lúc tạo. Đọc When to run, rồi Test bằng một tuần giả, không gửi đi đâu.

## Luật Ask first của owner

Một luật một hành động, gắn tài khoản owner nên áp cho mọi Bot trên máy:

- Hỏi trước khi gửi email hoặc tin nhắn ra ngoài.
- Hỏi trước khi đăng bài hoặc đổi trang public.
- Hỏi trước khi chi tiền hoặc đổi ngân sách.
- Hỏi trước khi xóa file trong `campaigns/<id>/ket-qua/da-duyet/`.

Tuần bàn giao đầu, các luật này còn đó dù Review đã đạt. Đạt nghĩa là được đưa người, không nghĩa là được đăng.

## Khi cả phòng cùng nói vào

Bản mặc định là một owner. Trưởng phòng là người duy nhất nhắn Lead. Nhân viên đưa việc qua trưởng phòng.

Khi nhiều người phải tự nhắn Lead: đổi Lead thành Team Bot. Team Bot không làm primary được. Năm Bot kia cũng nên là Team Bot cùng owner nếu cả phòng đọc cùng `company/` và `campaigns/`. Đừng gắn key cá nhân.

Chat riêng của mỗi người với Team Bot là riêng. Cổng duyệt của từng yêu cầu vẫn là người đã giao việc đó.

## Skill

Skill nằm trong `skills/`. Bot nào đọc skill nào nằm ở `skills/README.md`. Rubric audit nằm ở `skills/mkt-audit/references/rubric.md`. Checklist chấm nằm ở `skills/mkt-review-check/references/checklist.md`.

Hồ sơ thương hiệu là mẫu trống. Điền trước khi cài. Cách cài, sau khi bản này được duyệt, nằm ở `docs/cai-dat.md`.

## Nguồn ràng buộc Grok Bot

- `knowledge/13-chuan-build-team.md`
- `knowledge/08-kenh-va-hop-tac.md`
- `knowledge/07-skill-va-routine.md`
- `knowledge/02-mo-hinh-van-hanh.md`
