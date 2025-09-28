🏥 PhuongDongCare — Hệ thống Quản lý Phòng Khám (Spring Boot + MySQL)

PhuongDongCare là một hệ thống quản lý phòng khám dựa trên web, được xây dựng bằng Spring Boot và cơ sở dữ liệu MySQL độc lập. Hệ thống cung cấp giao diện bảo mật và phân quyền theo vai trò để quản lý lịch hẹn, buổi tư vấn và tương tác giữa bác sĩ – bệnh nhân trong môi trường y tế số.

👥 Các Vai Trò
👤 Admin

Giám sát toàn bộ nền tảng.

Có thể xem tất cả bác sĩ và bệnh nhân đã đăng ký.

Có thể xóa tài khoản bác sĩ hoặc bệnh nhân (nhưng không thể thêm hay chỉnh sửa).

Có thể xem tất cả các lịch hẹn đã lên.

Không thể chỉnh sửa hoặc xóa lịch hẹn.

Không thể xem các buổi tư vấn riêng giữa bác sĩ và bệnh nhân.

👨‍⚕️ Bác sĩ

Đăng ký bằng form an toàn, bao gồm:

Mã giấy phép hành nghề

Số CMND/CCCD

Có thể đăng nhập để truy cập Bảng điều khiển Bác sĩ.

Tính năng:

Cập nhật hồ sơ và thông tin cá nhân.

Thêm hoặc xóa lịch hẹn (chỉ những lịch đã cũ hoặc đã hoàn thành).

Tạo buổi tư vấn sau khi hẹn khám, bao gồm:

Ghi chú toa thuốc

Lời khuyên thêm

Phí tư vấn

Sau khi tạo, buổi tư vấn không thể chỉnh sửa hoặc xóa.

🧑‍💻 Bệnh nhân

Có thể đăng ký hoặc đăng nhập để truy cập Bảng điều khiển Bệnh nhân.

Tính năng:

Chỉnh sửa hồ sơ và thông tin cá nhân.

Xem các lịch hẹn sắp tới:

Đặt trực tuyến bởi chính họ

Được bác sĩ nhập thủ công sau cuộc gọi điện thoại

Đặt lịch hẹn trực tuyến bằng cách:

Lọc bác sĩ theo chuyên khoa

Chọn bác sĩ và đặt lịch qua giao diện

Xem buổi tư vấn nếu:

Thanh toán bằng tiền mặt: bác sĩ đánh dấu đã thanh toán

Thanh toán trực tuyến: được chuyển hướng đến cổng thanh toán, sau đó mới có quyền truy cập

💳 Logic Thanh Toán

Bác sĩ thiết lập trạng thái buổi tư vấn:

PAID: Bệnh nhân đã thanh toán bằng tiền mặt sau buổi hẹn.

UNPAID: Với thanh toán trực tuyến – bệnh nhân được chuyển hướng đến cổng thanh toán.

Sau khi thanh toán được xác nhận, bệnh nhân có toàn quyền truy cập buổi tư vấn.