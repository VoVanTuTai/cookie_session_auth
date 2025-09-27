🔐 Simple Auth
🚀 Cách chạy
1. Vào thư mục chứa dự án
cd src/cookie_session_auth
2. Cài đặt dependencies bash Copy code: npm install express Basic Auth Chạy server bash Copy code: node app.js
Kiểm tra API
POST: http://localhost:3000/auth/register
body->raw->chỉnh type sang Json nội dung "{"username":"admin", "password":"12345"}"
<img width="960" height="540" alt="3000" src="https://github.com/VoVanTuTai/cookie_session_auth/blob/main/Images_report/auth_register.png" />
mongo sau khi đăng ký
<img width="960" height="540" alt="3000" src="https://github.com/VoVanTuTai/cookie_session_auth/blob/main/Images_report/mongo_after_register.png" />
POST: http://localhost:3000/auth/login
body->raw->chỉnh type sang Json nội dung "{"username":"admin", "password":"12345"}"
<img width="960" height="540" alt="3000" src="https://github.com/VoVanTuTai/cookie_session_auth/blob/main/Images_report/auth_login.png" />
mongo sau khi đăng nhập lưu dữ liệu vòa session
<img width="960" height="540" alt="3000" src="https://github.com/VoVanTuTai/cookie_session_auth/blob/main/Images_report/mongo_after_login.png" />
GET: http://localhost:3000/auth/profile
<img width="960" height="540" alt="3000" src="https://github.com/VoVanTuTai/cookie_session_auth/blob/main/Images_report/auth_profile_after_login.png" />
GET: http://localhost:3000/auth/logout
<img width="960" height="540" alt="3000" src="https://github.com/VoVanTuTai/cookie_session_auth/blob/main/Images_report/auth_logout.png" />
Sau khi logout session bị xóa
<img width="960" height="540" alt="3000" src="https://github.com/VoVanTuTai/cookie_session_auth/blob/main/Images_report/mongo_after_logout.png" />

