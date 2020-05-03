## Các quy tắc cần áp dụng khi làm việc cùng git

# Tham khảo ( VUI LÒNG ĐỌC KĨ BÀI NÀY, VÌ BÀI NÀY ĐÃ NÓI HẾT VỀ CÁC BƯỚC ĐỂ LÀM RỒI)
- https://nvie.com/posts/a-successful-git-branching-model/

# Quy tắc
- Các tính năng mới đều được phân nhánh từ branch develop ( sử dụng $ git checkout -b feat/myfeature develop), quy tắc đặt tên có tiêu đều feat/ ở đầu
- Các brand feature sau khi dev và test xong thì merge vào branch develop
- Sau khi merge , lên github tao pull request để leader review . Nếu ok thì tạo branch release( đặt tên có tiền tố release-) và tạo pull request để review merge vào branch master
- Nếu có lỗi phát sinh của tính năng sau khi đã merge vào master( đang trong quá tình chạy product) thì tạo branch mới ( với tiền tố hotfix-) và fix lỗi trên branch này, sau đó merge lại vào master

