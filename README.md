# CS2225.2020.N001
Đồ án cuối kỳ: Nhận dạng sản phẩm hạt điều nguyên liệu đáp ứng tiêu chuẩn mang chỉ dẫn địa lý "Bình Phước"
# Giới thiệu
Tỉnh Bình Phước được mệnh danh là “thủ phủ điều” của Việt Nam với 137.891 ha cây điều (theo Cục Thống kê tỉnh Bình Phước, tháng 11/2020), chiếm gần 50 % diện tích cây điều của cả nước, cho ra các sản phẩm có chất lượng cao, được khách hàng và các chuyên gia đánh giá là “ngon nhất thế giới”, từ đó đã tạo ra thương hiệu “Hạt điều Bình Phước” nổi tiếng trong nước và thị trường quốc tế, được xuất khẩu đến 25 quốc gia và vùng lãnh thổ. Hạt điều Bình Phước đã được Cục Sở hữu trí tuệ cấp Giấy chứng nhận bảo hộ chỉ dẫn địa lý “ngày 13/3/2018.

Tuy nhiên, hạt điều Bình Phước chỉ cho thu hoạch 1 vụ trong năm nên nhiều doanh nghiệp chế biến điều không đủ nguyên liệu để chế biến, phải nhập khẩu điều nguyên liệu của các nước khác ở Châu Phi, Châu Mỹ, Ấn độ, Campuchia… Vì vậy đặt ra thách thức trong công tác quản lý thị trường để tránh tình trạng nút bóng thương hiệu “Hạt điều Bình Phước” nhưng thực chất là điều nhập khẩu.

Hiện nay, có nhiều đối tượng sản xuất, kinh doanh các sản phẩm hạt điều kém chất lượng, giả mạo thương hiệu “Hạt điều Bình Phước” và bày bán tràn lan trên thị thường, đặc biệt trên mạng xã hội. Mới đây, Công tỉnh Bình Phước đã phát hiện và xử phạt 4 cơ sở kinh doanh trên địa bàn thị xã Phước Long và huyện Bù Đăng tỉnh Bình Phước (https://laodong.vn/thi-truong/buoc-tieu-huy-gan-6-tan-hat-dieu-kem-chat-luong-rao-ban-tren-mang-xa-hoi-875473.ldo) vì sản xuất, kinh doanh hạt điều kém chất lượng rao bán trên mạng xã hội.

Để giúp người dân truy xuất được nguồn gốc hạt điều Bình Phước, thời gian qua Sở Khoa học và Công nghệ tỉnh Bình Phước đã ứng dụng giải pháp tem điện tử QR-code (VNPT-Check). Tuy nhiên, giải pháp này chỉ hỗ trợ truy xuất nguồn gốc nơi sản xuất ra sản phẩm, chống hàng giả và chỉ phù hợp với các doanh nghiệp có uy tín trên thị trường mà không có khả năng tự nhận diện để phân biệt được nguồn gốc sản phẩm. Người tiêu dùng nếu không phải là chuyên gia hoặc người có nhiều kinh nghiệm trong sản xuất hạt điều thì khó có thể phát hiện ra sản phẩm nào là hạt điều Bình Phước khi chưa có công cụ hỗ trợ nhận diện.

Trên cơ sở kết quả nghiên cứu đặc trưng về mặt cảm quan của hạt điều nguyên liệu, nhóm đề xuất ứng dụng công nghệ nhận dạng thị giác máy tính để xây dựng công cụ hỗ trợ nhận dạng sản phẩm hạt điều nguyên liệu có đáp ứng tiêu chuẩn mang chỉ dẫn địa lý “Bình Phước” hay không.
![margin penalty for target logit](https://github.com/happy-fruit-vietnam/CS2225.2020.N001/blob/master/resources/quytrinhtongquat.png)

# Dữ liệu Training
Dữ liệu 800 bức ảnh hạt điều được thu thập và chụp bằng camera của Iphone 6
Trong đó: 400 bức ảnh là hạt điều đạt chuẩn Bình Phước và 400 bức ảnh không đạt chuẩn

# Train mô hình
Ta chia làm 2 bước chính:
## Bước 1: Xác định vị trí hạt điều trên ảnh bằng Yolo V4
## Bước 2: Phân lớp (classification) hạt điều đạt chuẩn và không đạt chuẩn
### Chi tiết được trình bày và diễn giải trong link Notebook phía dưới
Link notebook Google Colab: https://colab.research.google.com/drive/1jTAcvXfqnGlaWCsWS0ulVWBCg3qINnfs?usp=sharing
