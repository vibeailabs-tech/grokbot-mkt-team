---
name: mkt-review-check
description: Review chấm bản nháp theo checklist. Đạt, không đạt, hoặc dừng để hỏi người.
---

# Chấm bản

## Khi nào dùng

Lead giao, trong `drafts/` đã có file, `brief.md` đã có.

## Đầu vào

`meta.md`, `brief.md`, mọi file trong `drafts/`, `company/thuong-hieu.md`, `company/vi-du.md`, `company/gia.md` nếu bản nháp có giá, checklist `references/checklist.md`.

## Các bước

1. Đọc brand KB. Hồ sơ trống thì kết luận Không đạt, lý do là hồ sơ, không chê bài.
2. Đọc vòng trong meta. Vòng từ 2 trở lên và đây là lần chấm mới sau hai lần không đạt thì không yêu cầu sửa tiếp. Kết luận ghi "Dừng hỏi người".
3. Đi từng dòng checklist. Một dòng trượt là Không đạt.
4. Viết `campaigns/<id>/review.md` đúng bốn phần trong checklist.
5. Kết luận Đạt: chép các file trong `drafts/` sang `campaigns/<id>/ket-qua/cho-duyet/`. Không sửa chữ khi chép. Điền `duyet.md`: hiện trạng, việc đề xuất, nguồn, cách lùi lại.
6. Kết luận Không đạt: không chép sang outputs. Liệt kê từng chỗ để Content sửa. Không tự sửa.
7. Nói trong nhóm kết luận và đường dẫn review.md.

## Kiểm tra

Mỗi dòng Không đạt có tên file và lý do thuộc checklist. Không có lời khuyên viết thêm cho hay nếu checklist đã đạt.

## Nộp lại

`review.md`, và bản copy trong `outputs/review/<id>/` chỉ khi Đạt.

## Phải dừng

Không sửa hộ Content, không đăng, không gửi, không ghi `learnings.md` trước khi người chốt.
