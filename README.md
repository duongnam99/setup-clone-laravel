# Khởi đầu với project laravel sau khi clone  
## Clone
- Tạo ssh-key cho máy: `ssh-keygen`
- Lấy nội dung của ssh-key và ném vào github/gitlab: `cat ~/.ssh/id_rsa.pub`
- Clone từ github/gitlab

## Cài composer dependency 
- `composer install`: cài các gói

## Cài npm dependency
- `npm install`

## Tạo file env  
- env là file cấu hình môi trường trong laravel
- file env sẽ chưa có sau khi clone vì lí do bảo mật, ty nhiên sẽ có template của nó là env.example  
- `cp .env.example .env`: tạo file env  

## Tạo key
- laravel yêu cầu phải có key mã hóa và thường được tạo vào lưu trong file env
- `php artisan key:generate`: tạo key  

## Tạo database
- Tạo một database rỗng để sẵn sàng migrate 

## Cấu hình database trong env
- Bao gồm db_name, pass, user...

## Migrate
- `php artisan migrate`

## Seed
- Nếu có file seed (tạo mẫu trong DB) thì: `php artisan db:seed`

## Tìm hiểu project 
- Đọc các thành phần quan trọng trong project: route, controller, db, view, command...  
- (xóa cache git: `git rm -r --cached .`)