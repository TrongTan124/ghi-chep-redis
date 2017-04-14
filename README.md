Đây là ghi chép của tôi trong quá trình tìm hiểu về Redis
====

Redis là một cơ sở dữ liệu dạng key-value. Các key của redis có thể là kiểu dữ liệu kiểu strings, hashes, lists, sets và sorted sets.

Redis định kỳ lưu dữ liệu xuống ổ cứng, điều này làm cho redis giống như một cơ sở dữ liệu chứ không chỉ là caching server đơn thuần

Các cấu trúc dữ liệu Redis cung cấp cũng rất hay, nó bao gồm dạng key-value như memcached, và những kiểu dữ liệu phức tạp hơn như Hashes - tương tự như một structure trong c, 
dạng Lists - đây là tập hợp có thứ tự, dễ dàng biến thành ngăn xếp (stack) hay hàng đợi (queue), 
dạng Sets - tập hợp không có thứ tự các phần tử không trùng lặp, dạng Sorted Sets - tập hợp có thứ tự các phần tử không trùng lặp
Ngoài ra, Redis cũng cung cấp cơ chế những cơ chế mạnh mẽ khác, chẳng hạn như pub/sub - rất thích hợp cho việc tạo kênh chat

Toàn bộ dữ liệu của Redis được lưu trên bộ nhớ nên tốc độ xử lý cực kỳ nhanh, thậm chí có phần vượt trên memcached. Theo định kỳ dữ liệu từ trên bộ nhớ sẽ được đẩy xuống ổ đĩa

Redis là một sự lựa chọn tuyệt vời khi ta cần đến một server lưu trữ dữ liệu đòi hỏi tính mở rộng cao (scaleable) và chia sẻ bởi nhiều tiền trình, 
nhiều ứng dụng và nhiều server khác nhau. Chỉ riêng cơ chế tương tác giữa các tiến trình đã cực kỳ khó nhằn rồi. 
Do đó việc ta có thể tương tác cross-platform, cross-server, và cross-application đã làm Redis trở thành một lựa chọn đúng đắn cho rất rất nhiều công việc khác nhau. 
Tốc độ cực cao của Redis cũng có thể được lợi dụng để làm caching layer

----
Mọi ý kiến đóng góp có thể phản hồi theo địa chỉ sau:
- Skype: crazyman12487
- Gmail: nguyentrongtan124@gmail.com
