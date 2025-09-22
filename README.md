Hệ thống bán sách
Mô tả
Ứng dụng web bán sách đơn giản xây dựng bằng Flask (Python) cho backend và HTML / CSS / JavaScript cho frontend.

Tính năng chính
- Quản lý danh mục sách (thêm, sửa, xóa, xem)
- Trang danh sách và chi tiết sách
- Giỏ hàng (thêm, xóa, đặt hàng)
- Người dùng: đăng ký, đăng nhập, đăng xuất
- Thanh toán giả lập (không tích hợp cổng thật)
- Quản trị (admin) để quản lý sách và đơn hàng

Công nghệ sử dụng
- Backend: Python, Flask, Flask-Login, Flask-WTF, SQLAlchemy  
- Database: MySQL  
- Frontent: HTML, CSS, JavaScript 
- Quản lý gói: pip, venv  

Yêu cầu
- Python 3.8+
- pip

Cài đặt nhanh (local)
1. Clone repository:
   ```bash
   git clone https://github.com/MinhPhung256/bookseller
2. Tạo virtual environment & cài dependencies:
python -m venv venv
3. Tạo virtual environment & cài dependencies:
flask db init
flask db migrate -m "Init"
flask db upgrade
4. Chạy server
python run.py

Các endpoint chính
GET / — Trang chủ (danh sách sách)
GET /book/<id> — Chi tiết sách
POST /cart/add — Thêm sách vào giỏ
GET /cart — Xem giỏ hàng
POST /checkout — Đặt hàng
GET /admin — Trang admin (yêu cầu quyền)
GET/POST /auth/login, /auth/register, /auth/logout

