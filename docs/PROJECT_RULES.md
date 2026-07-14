# PROJECT RULES

## Mục tiêu

Xây dựng Discord Bot Tu Tiên chất lượng cao.

Không phải bot demo.

Mọi quyết định phải ưu tiên:

- Khả năng mở rộng
- Dễ bảo trì
- Hiệu năng
- Ít bug

---

## Làm việc theo Sprint

Không nhảy Sprint.

Không bỏ qua bước.

Mỗi Sprint phải hoàn thành trước khi sang Sprint mới.

---

## Git Workflow

Sau mỗi Module hoặc Sprint:

git add .

git commit -m "..."

git push

---

## Kiến trúc

Feature-based Architecture

Module-based

Repository Pattern

Service Pattern

Không MVC truyền thống.

---

## Code

Không viết code trùng lặp.

Không hard-code.

Không console.log.

Không import vòng.

Không viết gameplay trong Command.

Không truy cập Database trực tiếp từ Command.

---

## AI

Nếu AI viết code:

- Chia nhỏ file.
- Không tạo file quá lớn.
- Không sửa module khác nếu không cần.
- Luôn theo đúng kiến trúc dự án.
- Ưu tiên kết quả hơn giải thích dài dòng.

---

## Tài liệu

Khi thêm Module mới:

Cập nhật:

- FEATURES.md
- ROADMAP.md
- CHANGELOG.md (nếu có)

---

## Quy tắc làm việc

Luôn làm từng bước.

Không nhảy bước.

Sau khi hoàn thành một bước phải xác nhận trước khi sang bước tiếp theo.
