---
name: mkt-plan
description: Lead mở một campaign và giao đúng một Bot bằng cách @. Giữ phiếu duyệt.
---

# Điều phối

## Khi nào dùng

Người nhắn Lead, hoặc một routine tới giờ. Lead không viết brief và không viết bài.

## Đầu vào

Lời người, hoặc lịch trong `routines/lead.md`. Loại chỉ được là `social`, `email`, `audit`, `seo`, hoặc `report`. Thiếu đối tượng, offer, kênh, hoặc hạn thì hỏi trước, trừ routine đã ghi sẵn trong file lịch.

## Các bước

1. Chọn id `YYYYMMDD-ten-ngan`.
2. Tạo `campaigns/<id>/` từ `campaigns/_mau/`: `meta.md`, `ban-do.md`, `duyet.md`. Vòng 0. Chặng `research`. Điền mục tiêu và "xong khi" trên bản đồ.
3. Nếu người chưa nói họ đã biết gì, hỏi một câu rồi ghi vào `Người đã biết`. Routine được ghi `Người đã biết: không có thêm`.
4. Trong nhóm, `@` đúng một Bot. Research cho social, email, audit. SEO cho việc seo. Report cho việc report.
5. Research hoặc SEO xong thì đọc brief. Nhận định thiếu nguồn thì trả lại Bot đó, không giao Content.
6. Nếu `Góc người` trống và loại là social, email, hoặc seo: hỏi người ở chat riêng muốn góc nào, hoặc có cho viết mọi góc trong brief. Chặng `cho-goc`. Content chưa được viết.
7. Routine thứ Hai được đặt sẵn `Góc người: viết cả ba góc trong brief`.
8. `@Content` hoặc `@SEO` tùy loại. SEO viết bản sửa trang trong `drafts/`, không đăng. Report không đi qua Content.
9. `@Review`. Review viết `review.md` và, nếu đạt, điền `duyet.md`.
10. Đạt: chặng `cho-nguoi`. Đưa phiếu `duyet.md` sang chat riêng. Ba lựa chọn là duyệt, sửa, từ chối.
11. Không đạt và vòng dưới 2: tăng vòng, `@` Bot viết sửa đúng các dòng. Rồi `@Review` lại.
12. Đủ 2 vòng: không mở vòng mới. Hỏi người.
13. Người duyệt: ghi nguyên câu vào meta và `company/quyet-dinh.md`, chép bản sang `campaigns/<id>/ket-qua/da-duyet/`, chặng `xong`. Nhắc người tự đăng.
14. Người sửa: ghi nguyên câu, kèm lý do họ nói. Nếu còn vòng, chạy lại. Nếu họ từ chối, chặng `xong`, không chép sang `da-duyet/`.

Thứ Sáu, Lead không mở campaign mới. `@Report` đọc các `meta.md` trong tuần và file số người đã thả, rồi viết báo cáo.

Trong nhóm luôn `@` một Bot. Không viết câu chung cho cả nhóm làm việc.

## Kiểm tra

Một lúc một Bot được giao. `duyet.md` có hiện trạng, việc đề xuất, nguồn, và cách lùi lại trước khi người thấy phiếu. Lead không có file trong `drafts/`.

## Nộp lại

Meta, bản đồ, và một tin `@` Bot kế tiếp. Phiếu chờ người nằm ở chat riêng.

## Phải dừng

Không tự nghiên cứu, không viết, không gửi, không đăng, không chi tiền, không sửa `company/thuong-hieu.md`. Loại lạ thì hỏi người trước khi tạo thư mục. Không mở bot Paid. Chữ quảng cáo chỉ khi người nói rõ là bản nháp và `company/ngan-sach.md` không bị Bot hiểu thành quyền chi.
