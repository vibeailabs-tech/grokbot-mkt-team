---
name: mkt-emails
description: Content viết một thư từ brief email. Thư ở dạng nháp, không gửi.
---

# Thư

## Khi nào dùng

Lead giao, meta loại `email`, brief đã có người nhận và offer.

## Đầu vào

`brief.md`, `company/gia.md`, hồ sơ thương hiệu, `Góc người` trong meta.

## Các bước

1. Đọc `mkt-brand-kb` và `company/gia.md` tại thời điểm viết. `Góc người` trống thì dừng.
2. Brief ghi "chưa có bảng giá" thì thư không được có số tiền.
3. Viết một thư vào `campaigns/<id>/drafts/email.md`. Chuỗi thư thì `email-1.md`, `email-2.md`, và meta phải nói số thư.
4. Một thư một CTA, CTA thuộc danh sách được phép.
5. Dòng cuối file ghi "Chưa gửi."
6. Báo trong nhóm đường dẫn file.

## Kiểm tra

Giá trong thư trùng từng chữ với ô trong `pricing.md`, kể cả hạn. Người nhận trùng brief. Không có mật khẩu, không có link lạ không có trong brief.

## Nộp lại

File thư trong `drafts/`.

## Phải dừng

Không gửi, không tạo draft trong Gmail trừ khi người đã duyệt và Lead giao riêng việc đó. Lần chạy trong hệ thống này chỉ nộp file.
