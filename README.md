Dự án 
Hệ thống E-Commerce

TÀI LIỆU ĐẶC TẢ 
YÊU CẦU PHẦN MỀM (SRS)

Hà Nội, tháng 12 - 2024
 
1. Giới thiệu chung

1.1. Mục đích

Tài liệu này nhằm mục đích phân tích các yêu cầu xây dựng phần mềm Hệ thống E-Commerce bao gồm mục tiêu và phạm vi hệ thống, quy trình nghiệp vụ sau khi xây dựng hệ thống thương mại điện tử, các yêu cầu chức năng và phi chức năng, các ràng buộc khác có liên quan và tiêu chuẩn nghiệm thu hệ thống.
Tài liệu này được dùng làm đầu vào cho các quá trình thiết kế, lập trình, kiểm thử hệ thống của việc xây dựng phần mềm.
Tài liệu này được xây dựng dựa trên:

●	Tài liệu phân tích yêu cầu người dùng (URD)

●	Nghiên cứu thị trường thương mại điện tử

●	Phân tích các hệ thống E-Commerce hiện có

1.2. Phạm vi

1.2.1. Trong phạm vi

Tài liệu này được áp dụng cho việc phân tích và xây dựng hệ thống E-Commerce. Trong hệ thống, người dùng có thể:

●	Duyệt và tìm kiếm sản phẩm trên website thương mại điện tử

●	Thêm sản phẩm vào giỏ hàng và thực hiện thanh toán trực tuyến

●	Quản lý tài khoản cá nhân, lịch sử đơn hàng và thông tin giao hàng

●	Đánh giá và nhận xét về sản phẩm đã mua

●	Theo dõi trạng thái đơn hàng và giao hàng

●	Sử dụng các chức năng khuyến mãi và mã giảm giá

1.2.2. Ngoài phạm vi

Tài liệu này chưa áp dụng cho:

●	Hệ thống quản lý kho hàng vật lý

●	Tích hợp với các marketplace bên thứ ba (Shopee, Lazada, Tiki...)

●	Hệ thống logistics và vận chuyển của bên thứ ba


1.3. Thuật ngữ và định nghĩa

Thuật ngữ/ từ viết tắt	Định nghĩa

E-Commerce	|| Thương mại điện tử là hình thức mua bán hàng hóa, dịch vụ thông qua các phương tiện điện tử, chủ yếu là internet

Khách hàng	Người dùng cuối sử dụng hệ thống để mua sắm sản phẩm

Admin	Quản trị viên hệ thống có quyền quản lý toàn bộ hệ thống

Vendor/Seller	Người bán hàng, có thể đăng ký để bán sản phẩm trên hệ thống

Sản phẩm	Hàng hóa hoặc dịch vụ được bán trên hệ thống

Danh mục	Phân loại sản phẩm theo nhóm để dễ dàng tìm kiếm và quản lý

Giỏ hàng	Nơi lưu trữ tạm thời các sản phẩm khách hàng muốn mua

Đơn hàng	Yêu cầu mua hàng được tạo ra khi khách hàng thực hiện thanh toán

Thanh toán	Quá trình xử lý giao dịch tài chính để hoàn tất đơn hàng

Giao hàng	Quá trình vận chuyển sản phẩm từ người bán đến khách hàng

Đánh giá	Nhận xét và chấm điểm của khách hàng về sản phẩm đã mua

Khuyến mãi	Chương trình giảm giá hoặc ưu đãi đặc biệt cho khách hàng

Mã giảm giá	Mã code cho phép khách hàng được giảm giá khi thanh toán

Wishlist	Danh sách yêu thích chứa các sản phẩm khách hàng quan tâm

Inventory	Hệ thống quản lý tồn kho sản phẩm

Session	Phiên làm việc của người dùng trên hệ thống

Cookie	Dữ liệu nhỏ được lưu trữ trên trình duyệt để ghi nhớ thông tin người dùng

1.4. Giả định

●	Người dùng có kết nối internet ổn định để sử dụng hệ thống

●	Khách hàng có thiết bị hỗ trợ trình duyệt web hiện đại

●	Người bán có kiến thức cơ bản về thương mại điện tử

●	Hệ thống thanh toán của ngân hàng hoạt động bình thường

1.5. Rủi ro

●	Rủi ro bảo mật: Thông tin cá nhân và tài chính của khách hàng có thể bị đánh cắp

●	Rủi ro thanh toán: Giao dịch có thể thất bại do lỗi hệ thống ngân hàng hoặc mạng

●	Rủi ro gian lận: Khách hàng hoặc người bán có thể thực hiện các hành vi gian lận

●	Rủi ro kỹ thuật: Hệ thống có thể gặp sự cố do tải cao hoặc lỗi phần mềm

●	Rủi ro pháp lý: Thay đổi trong quy định pháp luật về thương mại điện tử

●	Rủi ro cạnh tranh: Các đối thủ cạnh tranh có thể ra mắt sản phẩm tương tự tốt hơn

●	Rủi ro logistics: Sự cố trong quá trình giao hàng có thể ảnh hưởng đến trải nghiệm khách hàng

2. Tương tác với hệ thống E-Commerce

Trước khi đi vào tổng quan hệ thống, phần này đưa ra một cái nhìn tổng quan về cách khách hàng tương tác với hệ thống E-Commerce thông qua website và ứng dụng di động.

2.1. Trải nghiệm khách hàng

2.1.1. Trang chủ và khám phá sản phẩm

Hình 2.1.1. Trang chủ hệ thống E-Commerce

●	Trang chủ hiển thị khi khách hàng truy cập vào website lần đầu

●	Trang chủ bao gồm:

  ○	Header với logo, thanh tìm kiếm, giỏ hàng và tài khoản người dùng

  ○	Banner quảng cáo các sản phẩm nổi bật và chương trình khuyến mãi

  ○	Danh mục sản phẩm chính

  ○	Sản phẩm bán chạy, sản phẩm mới, sản phẩm được đề xuất

  ○	Footer với thông tin liên hệ và chính sách

Hình 2.1.2. Trang danh sách sản phẩm

●	Khi khách hàng click vào danh mục hoặc tìm kiếm sản phẩm

●	Hiển thị danh sách sản phẩm với:

  ○	Hình ảnh sản phẩm

  ○	Tên sản phẩm và giá

  ○	Đánh giá sao và số lượng đánh giá

  ○	Nút "Thêm vào giỏ hàng" và "Yêu thích"

●	Có các bộ lọc: giá, thương hiệu, đánh giá, tình trạng kho


2.1.2. Chi tiết sản phẩm và mua hàng

Hình 2.1.3. Trang chi tiết sản phẩm

●	Khi khách hàng click vào sản phẩm cụ thể

●	Hiển thị thông tin chi tiết:

  ○	Gallery hình ảnh sản phẩm

  ○	Tên, giá, mô tả chi tiết sản phẩm

  ○	Thông số kỹ thuật

  ○	Tùy chọn: màu sắc, kích thước, số lượng

  ○	Nút "Thêm vào giỏ hàng" và "Mua ngay"

  ○	Thông tin người bán và chính sách đổi trả

  ○	Đánh giá và nhận xét của khách hàng khác

Hình 2.1.4. Giỏ hàng

●	Khi khách hàng thêm sản phẩm vào giỏ hàng

●	Hiển thị:

  ○	Danh sách sản phẩm trong giỏ hàng

  ○	Số lượng và giá từng sản phẩm
  
  ○	Tổng tiền tạm tính
    
  ○	Mã giảm giá (nếu có)

  ○	Nút "Tiếp tục mua sắm" và "Thanh toán"


2.1.3. Thanh toán và hoàn tất đơn hàng


Hình 2.1.5. Trang thanh toán

●	Khi khách hàng click "Thanh toán" từ giỏ hàng

●	Bao gồm các bước:

  ○	Đăng nhập hoặc nhập thông tin khách hàng

  ○	Chọn địa chỉ giao hàng

  ○	Chọn phương thức vận chuyển

  ○	Chọn phương thức thanh toán

  ○	Xác nhận đơn hàng và thanh toán

Hình 2.1.6. Xác nhận đơn hàng

●	Sau khi thanh toán thành công


●	Hiển thị:

  ○	Mã đơn hàng

  ○	Thông tin sản phẩm đã đặt

  ○	Thông tin giao hàng

  ○	Tổng tiền đã thanh toán

  ○	Thời gian dự kiến giao hàng


2.2. Quản lý tài khoản khách hàng

2.2.1. Đăng ký và đăng nhập

Hình 2.2.1. Form đăng ký tài khoản

●	Khách hàng có thể đăng ký tài khoản mới

●	Thông tin cần thiết:


  ○	Email hoặc số điện thoại

  ○	Mật khẩu

  ○	Họ tên

  ○	Ngày sinh (tùy chọn)

●	Có thể đăng ký qua mạng xã hội (Google)


Hình 2.2.2. Trang quản lý tài khoản

●	Sau khi đăng nhập thành công

●	Khách hàng có thể:

  ○	Xem và chỉnh sửa thông tin cá nhân

  ○	Quản lý địa chỉ giao hàng

  ○	Xem lịch sử đơn hàng

  ○	Theo dõi trạng thái đơn hàng

  ○	Quản lý danh sách yêu thích

  ○	Đổi mật khẩu

2.3. Tương tác với người bán

●	Khách hàng có thể:

  ○	Xem thông tin sản phẩm

  ○	Gửi tin nhắn hỏi về sản phẩm

  ○	Theo dõi shop yêu thích

3. Tổng quan

3.1. Tổng quan hệ thống

●	Hệ thống E-Commerce là một nền tảng thương mại điện tử cho phép khách hàng mua sắm trực tuyến và người bán quản lý cửa hàng của họ.

●	Hệ thống cung cấp trải nghiệm mua sắm hoàn chỉnh từ việc duyệt sản phẩm, thêm vào giỏ hàng, thanh toán đến theo dõi đơn hàng.


●	Các tính năng chính:

  ○	Quản lý sản phẩm và danh mục

  ○	Giỏ hàng và thanh toán trực tuyến
  
  ○	Quản lý đơn hàng và giao hàng
  
  ○	Chương trình khuyến mãi và mã giảm giá

  ○	Quản lý tài khoản khách hàng và người bán

3.2. Mô hình tổng quan hệ thống

[Sơ đồ kiến trúc hệ thống E-Commerce]

3.3. Danh sách chức năng

●	Dashboard Admin:

  ○	Thống kê doanh thu, đơn hàng, khách 
  
  ○	Báo cáo theo thời gian và danh mục

  ○	Giám sát hoạt động hệ thống


●	Quản lý sản phẩm:

  ○	Thêm, sửa, xóa sản phẩm

  ○	Quản lý danh mục sản phẩm

  ○	Quản lý kho hàng và tồn kho

  ○	Thiết lập giá và khuyến mãi

●	Quản lý đơn hàng:

  ○	Xem danh sách đơn hàng

  ○	Cập nhật trạng thái đơn hàng

  ○	Xử lý hoàn trả và đổi hàng

  ○	In hóa đơn và phiếu giao hàng


●	Quản lý khách hàng:

  ○	Xem danh sách khách hàng

  ○	Quản lý thông tin khách hàng

  ○	Phân nhóm khách hàng

  ○	Gửi email marketing

●	Hệ thống thanh toán:

  ○	Tích hợp các cổng thanh toán

  ○	Xử lý giao dịch trực tuyến

  ○	Quản lý hoàn tiền

  ○	Báo cáo tài chính

●	Quản lý giao hàng:

  ○	Tích hợp với đơn vị vận chuyển

  ○	Tính phí giao hàng

  ○	Theo dõi trạng thái giao hàng

  ○	Quản lý địa chỉ giao hàng

●	Marketing và khuyến mãi:

  ○	Tạo mã giảm giá

  ○	Thiết lập chương trình khuyến mãi

  ○	Email marketing

  ○	Quảng cáo sản phẩm

●	Báo cáo và thống kê:

  ○	Báo cáo doanh thu

  ○	Thống kê sản phẩm bán chạy

  ○	Phân tích hành vi khách hàng

  ○	Báo cáo tồn kho

●	Cài đặt hệ thống:

  ○	Cấu hình chung


  ○	Quản lý người dùng và phân quyền

  ○	Cài đặt thanh toán và giao hàng

  ○	Quản lý template và giao diện

4. Chức năng hệ thống

4.1. Sitemap

[Sơ đồ sitemap của hệ thống E-Commerce]

4.2. Độ ưu tiên

STT	Chức năng hệ thống	Độ ưu tiên

1	Quản lý sản phẩm	Cao nhất

2	Giỏ hàng và thanh toán	Cao nhất

3	Quản lý đơn hàng	Cao

4	Quản lý khách hàng	Cao

5	Hệ thống thanh toán	Cao

6	Dashboard Admin	Trung bình

7	Quản lý giao hàng	Trung bình

8	Marketing và khuyến mãi	Trung bình

9	Báo cáo và thống kê	Thấp

10	Cài đặt hệ thống	Thấp

4.3. Dữ liệu đầu vào

●	Thông tin sản phẩm: tên, mô tả, giá, hình ảnh, danh mục

●	Thông tin khách hàng: họ tên, email, số điện thoại, địa chỉ

●	Thông tin đơn hàng: sản phẩm, số lượng, giá, địa chỉ giao hàng

●	Thông tin thanh toán: phương thức, số tiền, trạng thái giao dịch

●	Dữ liệu cấu hình: thuế, phí giao hàng, chính sách đổi trả

5. Giao diện

5.1. Dashboard 

●	Tổng quan hệ thống:


  ○	Hiển thị các chỉ số KPI chính: doanh thu, đơn hàng, khách hàng mới

  ○	Biểu đồ doanh thu theo thời gian

  ○	Top sản phẩm bán chạy

  ○	Đơn hàng cần xử lý


●	Thống kê chi tiết:

  ○	Doanh thu theo ngày/tháng/năm

  ○	Số lượng đơn hàng và trạng thái

  ○	Thống kê khách hàng mới và khách hàng quay lại

  ○	Tỷ lệ chuyển đổi từ lượt xem thành đơn hàng

5.2. Quản lý sản phẩm

●	Danh sách sản phẩm:

  ○	Hiển thị bảng danh sách tất cả sản phẩm

  ○	Tìm kiếm và lọc sản phẩm theo danh mục, giá, trạng thái

  ○	Chức năng sắp xếp theo tên, giá, ngày tạo

  ○	Thao tác nhanh: chỉnh sửa, xóa, ẩn/hiện sản phẩm

●	Thêm/Chỉnh sửa sản phẩm:

  ○	Form nhập thông tin sản phẩm chi tiết

  ○	Upload và quản lý hình ảnh sản phẩm

  ○	Thiết lập SEO cho sản phẩm

  ○	Quản lý biến thể sản phẩm (màu sắc, kích thước)



5.3. Quản lý đơn hàng

●	Danh sách đơn hàng:

  ○	Hiển thị tất cả đơn hàng với thông tin cơ bản

  ○	Lọc theo trạng thái, ngày đặt, khách hàng

  ○	Tìm kiếm theo mã đơn hàng hoặc tên khách hàng

  ○	Cập nhật trạng thái đơn hàng hàng loạt

●	Chi tiết đơn hàng:

  ○	Thông tin đầy đủ về đơn hàng

  ○	Danh sách sản phẩm và số lượng

  ○	Thông tin khách hàng và địa chỉ giao hàng

  ○	Lịch sử thay đổi trạng thái đơn hàng


5.4. Quản lý khách hàng

●	Danh sách khách hàng:

  ○	Hiển thị thông tin cơ bản của khách hàng

  ○	Tìm kiếm theo tên, email, số điện thoại

  ○	Lọc theo nhóm khách hàng, ngày đăng ký

  ○	Xuất danh sách khách hàng

●	Hồ sơ khách hàng:

  ○	Thông tin chi tiết khách hàng

  ○	Lịch sử đơn hàng

  ○	Tổng giá trị đơn hàng

  ○	Ghi chú và nhãn khách hàng

5.5. Cài đặt hệ thống

●	Cài đặt chung:

  ○	Thông tin cửa hàng: tên, logo, địa chỉ, liên hệ

  ○	Cài đặt múi giờ và ngôn ngữ

  ○	Cấu hình email và thông báo

  ○	Chính sách bảo mật và điều khoản sử dụng


●	Cài đặt thanh toán:

  ○	Cấu hình các cổng thanh toán

  ○	Thiết lập phí giao dịch

  ○	Cài đặt tiền tệ và thuế

  ○	Quản lý phương thức thanh toán

●	Cài đặt giao hàng:

  ○	Cấu hình đơn vị vận chuyển

  ○	Thiết lập phí giao hàng theo khu vực

  ○	Cài đặt thời gian giao hàng

  ○	Quản lý địa chỉ kho hàng

●	Quản lý người dùng:

  ○	Danh sách admin và nhân viên

  ○	Phân quyền truy cập các chức năng

  ○	Quản lý vai trò và quyền hạn

  ○	Lịch sử hoạt động của người dùng

6. Yêu cầu phi chức năng

6.1. Hiệu suất

●	Thời gian tải trang không quá 3 giây

●	Hệ thống có thể xử lý đồng thời 1000 người dùng

●	Thời gian phản hồi API không quá 500ms

●	Uptime hệ thống đạt 99.9%

6.2. Bảo mật

●	Mã hóa dữ liệu nhạy cảm (mật khẩu, thông tin thanh toán)

●	Xác thực hai yếu tố cho tài khoản admin

●	Tuân thủ chuẩn PCI DSS cho thanh toán

●	Backup dữ liệu định kỳ và khôi phục khi cần

6.3. Khả năng mở rộng

●	Kiến trúc microservices để dễ dàng mở rộng

●	Hỗ trợ load balancing và auto scaling


●	Database có thể scale horizontal

●	API RESTful để tích hợp với hệ thống khác


6.4. Tương thích

●	Hỗ trợ các trình duyệt phổ biến (Chrome, Firefox, Safari, Edge)

●	Responsive design cho mobile và tablet

●	Tương thích với các hệ điều hành khác nhau

●	Hỗ trợ đa ngôn ngữ và đa tiền tệ

7. Kết luận

Tài liệu đặc tả yêu cầu phần mềm này đã mô tả chi tiết các yêu cầu chức năng và phi chức năng cho hệ thống E-Commerce. Việc triển khai hệ thống cần tuân thủ nghiêm ngặt các yêu cầu đã được định nghĩa để đảm bảo chất lượng và hiệu quả của sản phẩm cuối cùng.

Hệ thống E-Commerce khi hoàn thành sẽ cung cấp một nền tảng thương mại điện tử hoàn chỉnh, đáp ứng nhu cầu của cả khách hàng và người bán, đồng thời đảm bảo tính bảo mật, hiệu suất và khả năng mở rộng trong tương lai.
