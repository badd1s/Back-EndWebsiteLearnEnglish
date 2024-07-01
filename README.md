# Cách sử dụng Back-End

### Clone dự án vào Visual Studio Code, sau đó mở "Terminal".

### Chạy `npm install` để tải các thư viện của dự án trong "package.json".

### Tạo file mới ".env" với nội dung như sau

NODE_ENV = development
ACCESS_TOKEN_SECRET = {dán vào đây token mới}
REFRESH_TOKEN_SECRET = {dán vào đây token mới}
DATABASE_URI = {dán vào đây liên kết với CSDL ở MongoDB}
PORT = 3500

#### Cách tạo token mới

Mở "Terminal" trong VSCode
Gõ: `node`
Tiếp tục: `require('crypto').randomBytes(64).toString('hex')`

Cần 2 kết quả, sau đó dán ACCESS_TOKEN_SECRET và REFRESH_TOKEN_SECRET trong ".env".

### Chạy `npm run dev` để bắt đầu.
