# Phòng marketing

Bản đã cải tiến theo bài Espressio, 8/11/2026. Chưa đẩy GitHub, chưa cài lên Grok Bot. Chưa có brand voice của công ty nào.

Sáu Bot đọc cùng một não công ty trong `company/`. Mỗi việc là một campaign trong `campaigns/`. Người duyệt trên phiếu `duyet.md` rồi tự đăng.

| Việc | File |
|---|---|
| Não công ty, đang trống | [company/thuong-hieu.md](company/thuong-hieu.md) |
| Một campaign mẫu | [campaigns/_mau](campaigns/_mau) |
| Chỗ tìm file | [references.md](references.md) |
| Sáu Bot và nhóm | [bots](bots) |
| Skill | [skills/README.md](skills/README.md) |
| Cài sau khi duyệt | [docs/cai-dat.md](docs/cai-dat.md) |

```text
grokbot-mkt-team/
├── company/          giọng, giá, ví dụ, quyết định, định nghĩa số
├── campaigns/<id>/   brief, research, drafts, bản đồ, phiếu duyệt
├── skills/
├── bots/             Lead, Research, Content, SEO, Report, Review
└── references.md
```

Bot Paid chưa mở. Chữ quảng cáo chỉ là bản nháp khi người yêu cầu. Không có kho số liệu: Report chỉ đọc file người thả vào campaign.
