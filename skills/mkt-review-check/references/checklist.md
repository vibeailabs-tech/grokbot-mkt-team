# Checklist

Một dòng trượt thì cả bản Không đạt.

| Dòng | Đạt khi |
|---|---|
| Đúng việc | File nộp khớp loại trong meta: social có lịch, email có thư và dòng "Chưa gửi", audit có trang tóm tắt |
| Bám brief | Mọi sự thật trong bản nháp có một dòng trong bảng Sự thật của brief |
| Không bịa chỗ thiếu | Những dòng "Chỗ chưa có nguồn" không xuất hiện như sự thật trong bài |
| Thương hiệu | Không dùng từ cấm. CTA nằm trong danh sách được phép. Claim nằm trong "Claim được phép" hoặc trong brief có nguồn |
| Giá | Nếu có số tiền, số đó trùng `company/gia.md` ở lần đọc này |
| Góc người | Meta có `Góc người` trước khi có bản nháp cuối |
| Chưa phát hành | Không có câu nói bài đã đăng, thư đã gửi, hoặc quảng cáo đã chạy |
| Vòng sửa | Nếu review trước đã chỉ chỗ sai, bản này đã sửa đúng các dòng đó hoặc nói rõ dòng nào chưa sửa được vì thiếu nguồn |
| Vòng tối đa | Vòng trong meta nhỏ hơn 2, hoặc kết luận là "Dừng hỏi người" |

## Khuôn review.md

```text
# Review <id>
Vòng:
Kết luận: Đạt | Không đạt | Dừng hỏi người

## Đạt
-

## Không đạt
- File — câu hoặc đoạn — dòng checklist trượt

## Việc Lead làm tiếp
```

Đạt thì việc Lead là đưa `campaigns/<id>/duyet.md` sang chat riêng. Không đạt thì việc Lead là `@` Bot viết sửa đúng các dòng Không đạt và tăng vòng. Dừng hỏi người thì Lead không mở vòng mới.
