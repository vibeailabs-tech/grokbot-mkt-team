---
name: mkt-report
description: Report viết báo cáo tuần từ file người đã thả. Không ước lượng số thiếu.
---

# Báo cáo tuần

## Khi nào dùng

Lead `@Report` vào thứ Sáu, hoặc người mở campaign loại `report`.

## Đầu vào

`company/so-lieu.md`. Các `campaigns/<id>/meta.md` và `ket-qua/` của tuần. File xuất số mà người đã bỏ vào `ket-qua/`.

## Các bước

1. Đọc định nghĩa trong `company/so-lieu.md`. Bảng trống thì không so sánh kỳ.
2. Liệt kê campaign trong tuần theo chặng: đang chạy, chờ duyệt, đã duyệt.
3. Với mỗi số, ghi file nguồn và ngày của file. Không có file thì ghi "thiếu số", không điền số khác.
4. Viết `campaigns/<id-bao-cao>/drafts/bao-cao.md` với ba phần: việc đã xong, số có nguồn, câu cần người bàn.
5. Không đề xuất chi tiền. Không nói một kênh "đang thắng" nếu không có số trong file.

## Kiểm tra

Mọi số trong báo cáo có đường dẫn file. Câu thiếu số không bị biến thành kết luận.

## Nộp lại

Một file báo cáo. `@Lead` khi xong. Review chấm nếu Lead giao.

## Phải dừng

Không kéo số từ trí nhớ, không bịa lượt xem, không vào tài khoản quảng cáo.
