# Level 18 -> 19
Mục tiêu của level này là tìm ra mật khẩu  tiếp theo được lưu trong tệp ``readme`` trong thư mục home. Tuy nhiên, có vẻ như ai đó đã chỉnh sửa ``.bashrc`` để đăng xuất bạn khi đăng nhập bằng SSH.

**Note: ``.bashrc`` thường nằm trong thư mục ``home`` của người dùng. Cơ bản, ``.bashrc`` là một tệp cấu hình được đọc và thực thi bởi shell Bash khi nó được gọi dưới dạng một shell tương tác không đăng nhập**

Thay vì đăng nhập trực tiếp tới Server với SSH, chúng ta sec thực thi lệnh qua thông qua SSH.

```bandit18@bandit.labs.overthewire.org -p -2220 ls```

Kết quả cho thấy tệp ``readme``. Tiếp theo, ta sẽ sử dụng lệnh ``cat`` để lấy password trong file này.

``bandit18@bandit.overthewire.org -p 2220 cat readme``

Ta thu được kết quả:

![level18](/image/level18.png)

Password: ```awhqfNnAbc1naukrpqDYcF95h7HoMTrC```