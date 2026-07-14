# Coding Standards

## Naming

Folders:
kebab-case

Ví dụ:
player-system
combat-engine

Files:
kebab-case

Ví dụ:
player.service.ts
register.command.ts

Classes:
PascalCase

Ví dụ:
PlayerService

Interfaces:
IPlayer

Enums:
PlayerStatus

Types:
PlayerData

Functions:
camelCase

Ví dụ:
createPlayer()

Variables:
camelCase

Constants:
UPPER_SNAKE_CASE

Ví dụ:
MAX_LEVEL

---

## Command

Command chỉ làm:

- Parse input
- Permission
- Cooldown
- Gọi Service

Không viết gameplay trong Command.

---

## Service

Toàn bộ gameplay nằm ở đây.

Ví dụ:

- tính exp
- đột phá
- cộng tu vi
- combat

---

## Repository

Chỉ làm việc với Database.

Không chứa gameplay.

---

## Model

Định nghĩa Schema.

---

## Controller

Điều phối giữa Discord và Service.

---

## Utils

Helper dùng chung.

Không chứa gameplay.

---

## Validator

Kiểm tra dữ liệu đầu vào.

---

## Logger

Không dùng console.log.

Chỉ dùng Logger.

---

## Async

Luôn dùng async/await.

Không dùng callback.

---

## Error

Không throw string.

Luôn throw Error.