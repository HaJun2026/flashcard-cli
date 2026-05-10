# /ghi-chu — Ghi chú nghiên cứu có cấu trúc

Khi được gọi với `/ghi-chu [chủ đề]`, hãy giúp người dùng tổ chức ghi chú nghiên cứu theo quy trình sau:

## Bước 1 — Xác định chủ đề
Hỏi người dùng (nếu chưa cung cấp):
- Chủ đề cần ghi chú là gì?
- Nguồn: sách, bài báo, video, hay kinh nghiệm thực tế?
- Mức độ hiểu hiện tại: mới bắt đầu / có nền tảng / nâng cao?

## Bước 2 — Tạo ghi chú có cấu trúc
Tổ chức nội dung người dùng cung cấp thành format:

```markdown
# [Chủ đề]
> Nguồn: [tên nguồn] — [ngày]

## Ý chính
- ...

## Chi tiết
### [Khái niệm 1]
[Giải thích bằng ngôn ngữ đơn giản]
**Ví dụ:** ...

### [Khái niệm 2]
...

## Câu hỏi mở
- Điều gì chưa rõ?
- Cần tìm hiểu thêm về gì?

## Liên kết với kiến thức đã biết
- Liên quan đến: [chủ đề khác]
- Khác với: [khái niệm dễ nhầm]

## Flashcard gợi ý
Q: ...
A: ...
```

## Bước 3 — Gợi ý hành động tiếp theo
Sau khi tạo ghi chú, hỏi người dùng có muốn:
- Tạo flashcard từ ghi chú này bằng lệnh `/flashcard`?
- Tìm tài liệu liên quan trên GitHub với `/github-review`?
- Lưu ghi chú vào file `.md` trong thư mục `notes/`?
