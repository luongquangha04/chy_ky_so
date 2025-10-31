# chy_ky_so
tải open ssl và reader forxit PDF
<img width="968" height="184" alt="image" src="https://github.com/user-attachments/assets/c6daa98f-308c-4411-b0af-a0ee0d9e0973" />
<img width="926" height="416" alt="image" src="https://github.com/user-attachments/assets/02b9fcf2-f6fa-4be4-b8c7-af5210456011" />
tạo khóa bí mật 
<img width="1083" height="167" alt="image" src="https://github.com/user-attachments/assets/2478b7d4-1c92-45db-afb9-511d8be4248d" />

# 1️⃣ Tạo khóa bí mật
openssl genrsa -out private.pem 2048

# 2️⃣ Tạo yêu cầu cấp chứng chỉ (CSR)
openssl req -new -key private.pem -out request.csr -subj "/CN=Student58KTPM"

# 3️⃣ Tạo chứng chỉ tự ký (self-signed)
openssl x509 -req -in request.csr -signkey private.pem -out cert.pem -days 365

<img width="1176" height="123" alt="image" src="https://github.com/user-attachments/assets/0bfd26f0-f6e2-4ecf-9176-e33d136ed9a4" />

kết quả 
![Uploading image.png…]()
