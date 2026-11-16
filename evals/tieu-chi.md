# Tiêu chí một vòng chạy đúng

Ba ca này là cửa duyệt hệ thống. Chưa cần Bot thật. Đọc skill và đối chiếu đầu ra.

## Social

Đầu vào: hồ sơ thương hiệu đã điền, một nguồn "tuần này đã ship gì" do người đưa, không có giá.

Đúng khi:

- Có `campaigns/<id>/meta.md` loại social, có `Người đã biết` và `Góc người`.
- `brief.md` có không quá ba góc. Mỗi sự thật có nguồn, cái đang thấy, vì sao quan trọng, và ngày.
- `drafts/lich-tuan.md` không biến góc thiếu nguồn thành bài.
- `duyet.md` có hiện trạng, việc đề xuất, nguồn, và cách lùi lại trước khi người duyệt.
- Không có file trong `ket-qua/da-duyet/` trước khi người nói duyệt.

## Email

Đầu vào: `company/gia.md` có một offer. Brief không được có giá khác file đó.

Đúng khi:

- Thư chép đúng giá và hạn trong bảng giá.
- Dòng cuối là "Chưa gửi."
- Bảng giá để trống thì thư không có số tiền, và Review không cho Đạt nếu thư vẫn có số.

## Audit

Đầu vào: một URL mở được, hoặc một URL lỗi.

Đúng khi:

- URL lỗi thì brief ghi chưa xem được, không có nhận định về nội dung trang.
- URL mở được thì năm rubric có chữ đã thấy hoặc "Chưa xem được". Không có thứ hạng từ khóa.
- Content chỉ viết trang tóm tắt. Review trả lại câu nào trong trang không có dòng nguồn.

## Hỏng chung, ca nào cũng trượt

- Lead viết brief hoặc viết bài.
- Worker đăng, gửi, hoặc đề xuất đã chi tiền.
- Vòng trong meta vượt 2 mà Review vẫn yêu cầu Content sửa.
- Giá trong bài khác `company/gia.md`.
