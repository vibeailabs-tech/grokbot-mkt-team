# Cài lên Grok Bot

Làm sau khi bản này được duyệt và repo đã có trên GitHub. Chưa làm trong lúc thiết kế.

## 1. Đưa repo lên máy của Bot

Sáu Bot phải cùng một tài khoản owner để cùng thấy một máy.

Trên máy cloud, đặt repo tại `/workspace/grokbot-mkt-team`. Não công ty là `company/`. Mỗi việc là một thư mục trong `campaigns/`.

## 2. Điền trước khi chạy

- `company/thuong-hieu.md`: xóa chữ "điền".
- `company/gia.md` nếu việc đầu có giá.
- `references.md` khi nối thêm công cụ. Chưa nối thì không ghi là đã có.

Hồ sơ còn "điền" thì Bot phải dừng.

## 3. Tạo Bot

Tạo sáu Bot từ `bots/lead.md`, `research.md`, `content.md`, `seo.md`, `report.md`, `review.md`. Lead là primary.

## 4. Mở nhóm

Dán `bots/nhom.md`. Đủ sáu Bot. Trong nhóm chỉ Bot được `@` mới trả lời.

## 5. Bật Ask first

- Hỏi trước khi gửi email hoặc tin nhắn ra ngoài.
- Hỏi trước khi đăng bài hoặc sửa trang public.
- Hỏi trước khi chi tiền hoặc đổi ngân sách.
- Hỏi trước khi xóa file trong `ket-qua/da-duyet/`.

## 6. Chạy một social bằng tay

Chưa tạo routine. Nhắn Lead một việc social và nói bạn đã biết gì. Chọn một góc khi Lead hỏi. Chấm bằng `evals/tieu-chi.md`.

## 7. Rồi mới đặt lịch

Khi một social đạt, tạo ba routine bằng `routines/lead.md`. Đọc lại When to run. Test bằng dữ liệu giả.
