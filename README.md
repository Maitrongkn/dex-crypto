# DEX PHP - Web3 Token Explorer

Một ứng dụng web PHP hiển thị thông tin về các token cryptocurrency, với giao diện tương tự như DEXScreener.

## Tính năng

- Hiển thị danh sách token với thông tin chi tiết
- Biểu đồ giá realtime
- Theo dõi khối lượng giao dịch và biến động giá
- Tìm kiếm token
- Xem chi tiết token và lịch sử giao dịch
- Giao diện người dùng thân thiện, responsive

## Yêu cầu hệ thống

- PHP >= 7.4
- Composer
- Apache với mod_rewrite được bật
- MySQL/MariaDB

## Cài đặt

1. Clone repository:
```bash
git clone https://github.com/Maitrongkn/dex-crypto
cd dex-php
```

2. Cài đặt dependencies:
```bash
composer install
```

3. Tạo file .env từ mẫu:
```bash
cp .env.example .env
```

4. Cấu hình file .env với thông tin database và các API key cần thiết

5. Tạo virtual host trỏ đến thư mục public/

6. Đảm bảo thư mục storage/ có quyền ghi:
```bash
chmod -R 775 storage/
```

## Cấu trúc thư mục

```
dex-php/
├── public/          # Document root
│   ├── assets/      # CSS, JavaScript, images
│   └── index.php    # Front controller
├── src/             # PHP source code
│   └── Controllers/ # Controller classes
├── templates/       # Twig templates
├── vendor/         # Composer dependencies
└── .env            # Environment configuration
```

## Phát triển

1. Chạy server development:
```bash
php -S localhost:8000 -t public/
```

2. Truy cập ứng dụng tại http://localhost:8000
