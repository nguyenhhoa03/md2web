# md2web

Trình xem Markdown đơn giản, hỗ trợ tạo mục lục (TOC), chế độ sáng/tối và lấy file Markdown từ URL hoặc query string.

## Tính năng
- Hiển thị file Markdown từ URL.
- Hỗ trợ truyền URL Markdown qua query string (`?url=...`).
- Tự động tạo Mục lục (TOC).
- Chế độ Sáng/Tối (tự động hoặc thủ công).
- Hoạt động độc lập, không cần server.

## Cách dùng

### 1. Dùng file mặc định
Chỉ cần mở file:
```

md2web/md2web-vi-v1.1.html

```
Markdown sẽ được tải từ URL có sẵn trong mã.

### 2. Dùng URL chỉ định qua query string
```

md2web/md2web-vi-v1.1.html?url=https://example.com/file.md

```
Hoặc dạng rút gọn:
```

md2web/md2web-vi-v1.1.html?https://example.com/file.md

```

### 3. Dùng offline
Chỉnh sửa biến `MARKDOWN_URL` trong file HTML trỏ về file cục bộ.


## Giấy phép
GNU GPL v3

