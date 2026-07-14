# Kiến trúc dự án Tu Tiên Discord Bot

## Nguyên tắc

- Mỗi tính năng là một Module độc lập.
- Không được import chéo giữa các Module.
- Chỉ được giao tiếp thông qua Core hoặc Shared.
- Không viết logic lớn trong Command.
- Command chỉ nhận dữ liệu và gọi Service.

---

## Cấu trúc

src/
├── bootstrap
├── core
├── modules
├── shared

---

## Core

Core chứa:

- Discord Client
- Database
- Logger
- Cache
- Scheduler
- Event Loader
- Command Loader

Core không chứa gameplay.

---

## Modules

Ví dụ:

modules/player
modules/combat
modules/market

Mỗi Module tự quản lý:

- commands
- services
- models
- repositories
- events
- interfaces

---

## Shared

Shared chứa:

- constants
- utils
- enums
- types
- validators
- decorators

Không viết gameplay trong Shared.

---

## Quy tắc Code

- 1 file chỉ nên có 1 class.
- Không viết file quá 400 dòng.
- Hàm không quá 50 dòng nếu có thể.
- Tên biến dùng tiếng Anh.
- Comment dùng tiếng Việt khi cần giải thích logic phức tạp.
- Không hard-code ID Discord.
- Không hard-code giá vật phẩm.
- Mọi cấu hình đưa vào Config hoặc Database.

---

## Database

Không truy cập MongoDB trực tiếp trong Command.

Command
↓
Service
↓
Repository
↓
MongoDB

---

## Logger

Không dùng console.log trong gameplay.

Chỉ dùng Logger.

---

## Mục tiêu

Code dễ đọc.

Dễ mở rộng.

Dễ sửa lỗi.

Dễ thêm Module mới.