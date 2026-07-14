# AI Guide

## Mục tiêu dự án

Đây là Discord Bot Tu Tiên được viết bằng:

- TypeScript
- Discord.js v14
- MongoDB
- Mongoose

Kiến trúc:

Feature-based Architecture

Module-based

Không được viết theo kiểu MVC truyền thống.

---

## Luật

Gameplay nằm trong Service.

Repository chỉ truy cập Database.

Command không chứa gameplay.

Không hard-code.

Không viết file quá lớn.

Không tạo code trùng lặp.

Ưu tiên Generic.

Ưu tiên mở rộng.

---

## Module

Mỗi Module gồm:

commands/

controllers/

services/

repositories/

models/

events/

interfaces/

types/

validators/

utils/

---

## Coding

Luôn dùng async/await.

Không dùng callback.

Luôn try/catch.

Không console.log.

Chỉ Logger.

---

## Database

MongoDB

Mongoose

Repository Pattern

---

## Style

Code ngắn.

Dễ đọc.

Comment khi logic phức tạp.

Không viết code dài dòng.

---

## Ưu tiên

Hiệu năng.

Khả năng mở rộng.

Khả năng bảo trì.

Ít bug.

Ít lặp code.

---

## Khi AI tạo code

Luôn chia file.

Không gộp nhiều class.

Không gộp nhiều module.

Không phá kiến trúc.

Không sửa code module khác nếu không cần.

Nếu cần tạo file mới phải đúng cấu trúc project.