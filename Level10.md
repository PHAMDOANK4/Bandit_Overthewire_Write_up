# Level 10 -> 11
Mục tiêu bài này là tìm Password được chứa trong file ``data.txt`` và file này đã bị mã hóa bằng base64.

Kết nối tới Server bằng SSH: 

```ssh bandit10@bandit.labs.overthewire.org -p 2220```

Với password: ``G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s``

Sau khi kết nối thành công, kiểm tra các file thư mục nghi ngờ. Có file ``data.txt`` nằm trong đường dẫn chính. Dựa vào gợi ý từ đề bài, ta sẽ thực hiện decode base64 file này.

``base64 --decode data.txt``

Và ta có được kết quả:

![level10](/image/level10.png)

Password mình tìm được nè: ```6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM```