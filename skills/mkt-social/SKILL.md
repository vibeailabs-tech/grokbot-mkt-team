---
name: mkt-social
description: Content viết lịch tuần và bài nháp từ brief social. Không đăng.
---

# Bài social

## Khi nào dùng

Lead giao, meta loại `social`, đã có `brief.md` với đủ ba góc hoặc Lead chấp nhận ít hơn và ghi trong meta.

## Đầu vào

`brief.md`, `company/thuong-hieu.md`, `company/vi-du.md`, và `Góc người` trong meta.

## Các bước

1. Đọc `mkt-brand-kb`. Hồ sơ trống thì dừng.
2. `Góc người` trống thì dừng. `@Lead` và không viết bài.
3. Đọc brief và `company/vi-du.md`. Góc nằm trong "Chỗ chưa có nguồn" thì không viết thành bài.
4. Viết `campaigns/<id>/drafts/lich-tuan.md` theo mẫu. Mặc định năm ngày làm việc, mỗi ngày một bài, trừ khi meta nói khác. Chỉ viết các góc người đã chọn. Nếu họ chọn cả ba, viết cả ba.
5. Mỗi bài dùng một góc trong brief, một CTA nằm trong danh sách được phép, và chỉ những claim có nguồn trong brief hoặc hồ sơ.
6. Giọng bám ba tính cách và tránh từ cấm. Viết tiếng Việt có dấu.
7. `@Lead`: số bài viết được, số góc bỏ vì thiếu nguồn.

## Kiểm tra

Không có câu "đã đăng". Không có giá nếu brief không có giá kèm nguồn. Không có claim nằm trong danh sách cấm.

## Nộp lại

Một file `drafts/lich-tuan.md`.

## Phải dừng

Không đăng, không lên lịch trên mạng xã hội, không gửi.
