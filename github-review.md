# /github-review — Review & học từ GitHub qua MCP

Skill này dùng GitHub MCP để tra cứu, đọc code, và học từ các repo/PR thực tế.

**Yêu cầu:** MCP GitHub phải được cấu hình trong `.claude/settings.json` với `GITHUB_PERSONAL_ACCESS_TOKEN`.

---

## Cách dùng

### 1. Xem PR để học code review
```
/github-review pr [owner/repo] [số PR]
```
Khi người dùng cung cấp repo và PR number, dùng GitHub MCP để:
1. Lấy danh sách files thay đổi trong PR
2. Đọc diff của từng file
3. Phân tích và giải thích:
   - Mục đích của thay đổi này là gì?
   - Pattern/kỹ thuật nào được dùng?
   - Điểm tốt trong code?
   - Điều gì có thể cải thiện?
4. Tóm tắt thành bài học rút ra

### 2. Khám phá repo để học kiến trúc
```
/github-review repo [owner/repo]
```
Dùng GitHub MCP để:
1. Đọc README và cấu trúc thư mục
2. Đọc các file cấu hình chính (package.json, pyproject.toml, ...)
3. Vẽ sơ đồ kiến trúc bằng text/ASCII
4. Giải thích tech stack và lý do lựa chọn

### 3. Tìm ví dụ về một pattern/library
```
/github-review search [từ khoá] trong [owner/repo]
```
Dùng GitHub MCP search để tìm cách người ta dùng thực tế.

---

## Luồng xử lý mặc định

Nếu người dùng không chỉ rõ lệnh con, hỏi:
> "Bạn muốn: (1) review PR, (2) khám phá repo, hay (3) tìm ví dụ code?"

Sau khi hoàn thành, hỏi có muốn tạo ghi chú với `/ghi-chu` không.
