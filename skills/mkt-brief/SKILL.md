---
name: mkt-brief
description: Research viết brief.md cho một work id. Mỗi nhận định có nguồn.
---

# Brief

## Khi nào dùng

Lead giao trong nhóm, chặng đang là research. Một work id một brief.

## Đầu vào

`campaigns/<id>/meta.md`, lời Lead giao, và `company/thuong-hieu.md`. Email thì thêm `company/gia.md`. Audit thì thêm audit, page-scan và đối thủ. SEO trên trang là việc của Bot SEO, không nhét thứ hạng vào brief.

## Các bước

1. Đọc `mkt-brand-kb`. Hồ sơ trống thì dừng và nói Lead mục nào thiếu.
2. Đọc `Người đã biết` trong meta. Trống thì dừng, bảo Lead hỏi người trước khi mở trang.
3. Với mỗi thứ tìm thấy, ghi bốn mục: nguồn, cái đã đổi hoặc cái đang thấy, vì sao có thể quan trọng với campaign này, ngày mở. Thiếu một trong bốn thì dòng đó chưa được dùng làm sự thật.
4. Với social: đúng ba góc, mỗi góc một câu, và claim bị cấm còn áp vào tuần này.
5. Với email: người nhận, offer, giá chép từ `company/gia.md`. Bảng giá trống thì ghi "chưa có bảng giá".
6. Với audit: mỗi nhận định kèm URL và ngày. Không mở được thì ghi "chưa quan sát được".
7. Viết `campaigns/<id>/brief.md` theo mẫu, và thả ghi chú dài vào `campaigns/<id>/research/` nếu có.
8. `@Lead` khi xong, kèm số dòng chưa đủ bốn mục.

## Kiểm tra

Không có đoạn nào kêu gọi đăng hay gửi. Không có bài viết hoàn chỉnh. Mọi số đều có nguồn hoặc bị đánh dấu thiếu.

## Nộp lại

Một file `brief.md`. Không tạo `drafts/`.

## Phải dừng

Không viết bài đăng, không gửi, không đăng, không sửa hồ sơ thương hiệu.
