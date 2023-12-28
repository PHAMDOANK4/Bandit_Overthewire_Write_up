# Level 17 -> 18

Trong level trước ta thu được RSA key và copy lưu lại vào 1 file bất kì. Ví dụ: keyRSA.private.

Phân quyền lại cho file key đó:

``chmod 600 keyRSA.private``

Kết nối tới Server bằng SSH: 

```ssh -i keyRSA.private bandit17@bandit.labs.overthewire.org -p 2220```

Theo yêu cầu đề bài, ta nghĩ ngay sử dụng lệnh ``diff`` để tìm sự khác biệt giữa 2 tệp.

```diff passwords.old passwords.new```

Ta có kết quả:

![level17](/image/level17.png)

Đọc kĩ đề thì thấy bảo password nằm trong file ``passwords.new``

Và, Password cần tìm là: ```hga5tuuCLF6fFzUpnagiMN8ssu9LFrdg```