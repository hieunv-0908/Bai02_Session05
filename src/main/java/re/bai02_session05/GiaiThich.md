## Thiết kế API

| Chức năng | Method | URL | Query params | Status thành công | Status lỗi |
|---|---|---|---|---|---|
| Lấy danh sách sách | GET | /books | page=1&limit=10&author=... | 200 OK | 400 Bad Request |
| Lấy chi tiết sách | GET | /books/{id} | Không | 200 OK | 404 Not Found |
| Thêm sách mới | POST | /books | Không | 201 Created | 400 Bad Request |
| Cập nhật toàn bộ thông tin sách | PUT | /books/{id} | Không | 200 OK | 404 Not Found |
| Cập nhật số lượng sách | PATCH | /books/{id} | Không | 200 OK | 400 Bad Request |
| Xóa sách | DELETE | /books/{id} | Không | 204 No Content | 404 Not Found |
| Lấy danh sách thẻ mượn của một sách | GET | /books/{id}/loans | Không | 200 OK | 404 Not Found |
| Lấy danh sách tất cả thẻ mượn | GET | /loans | page=1&limit=10 | 200 OK | 400 Bad Request |
| Tạo thẻ mượn mới | POST | /loans | Không | 201 Created | 400 Bad Request |
| Lấy chi tiết thẻ mượn | GET | /loans/{id} | Không | 200 OK | 404 Not Found |
| Trả sách (cập nhật ngày trả) | PATCH | /loans/{id} | Không | 200 OK | 404 Not Found |
| Xóa thẻ mượn | DELETE | /loans/{id} | Không | 204 No Content | 404 Not Found |