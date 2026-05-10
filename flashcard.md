# /flashcard — Tạo và ôn flashcard học tập

Skill này tích hợp với CLI tool `flashcard.py` (cùng thư mục) để quản lý flashcard học tập.

**Repo GitHub:** `https://github.com/HaJun2026/flashcard-cli`
**Local tool:** `.claude/commands/flashcard/flashcard.py`

---

## Cách dùng

### Tạo flashcard từ ghi chú hiện tại
```
/flashcard tạo
```
Đọc nội dung người dùng vừa chia sẻ, tự động trích xuất 3–7 cặp Q&A phù hợp.
Sau đó chạy lệnh để lưu:
```bash
python .claude/commands/flashcard/flashcard.py add "câu hỏi" "câu trả lời" --tag [chủ đề]
```

### Ôn tập
```
/flashcard ôn [tag]
```
Chạy quiz session:
```bash
python .claude/commands/flashcard/flashcard.py quiz --tag [tag] --count 10
```

### Xem danh sách
```
/flashcard danh sách [tag]
```
```bash
python .claude/commands/flashcard/flashcard.py list --tag [tag]
```

### Xoá card
```
/flashcard xoá [id]
```
```bash
python .claude/commands/flashcard/flashcard.py delete [id]
```

---

## Tags gợi ý
- `python` — lập trình Python
- `web` — HTML/CSS/JS/React/Next.js
- `backend` — API, database, server
- `general` — kiến thức tổng quát

---

## Luồng mặc định

Nếu không có tham số, hỏi người dùng:
> "Bạn muốn: (1) tạo flashcard từ chủ đề, (2) ôn tập, hay (3) xem danh sách?"

Khi tạo flashcard, ưu tiên bám theo format:
- **Q:** Ngắn gọn, hỏi đúng 1 khái niệm
- **A:** Trả lời súc tích, thêm ví dụ nếu cần
