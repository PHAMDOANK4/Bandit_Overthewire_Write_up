# Level 9 -> 10
Mục tiêu level này là tìm password cho level tiếp theo ở trong file ``data.txt``, và nó chuỗi này chứa vài kí tự con người có thể đọc được, và trước nó có một số kí tự ``=``.

Kết nối tới Server bằng SSH: 

```ssh bandit9@bandit.labs.overthewire.org -p 2220```

Với password: ``EN632PlfYiZbn3PhVK3XOGSlNInNE00t``

Sau khi kết nối thành công, sử dụng lệnh ``ls`` để kiểm tra các file, thư mục chứa thông tin nghi ngờ. Và ta thấy có file ``data.txt``, mở ra ta thấy các thông tin:

![level9_1](/image/level9_1.png)

Theo gợi ý đầu bài, ta tìm chuỗi kí tự con người có thể đọc: ``strings data.txt``

![level9_2](/image/level9_2.png)

Tiếp tục, khai thác thêm thông tin từ gọi ý là có dấu ``=`` trong chuỗi. Ta sử dụng command: ``strings data.txt | grep "^=="``

![level9_3](/image/level9_3.png)

Và ta tìm thấy password cần tìm.
Password nè: ``G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s``