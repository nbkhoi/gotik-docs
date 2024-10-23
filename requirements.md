# Functional Requirements

## Sign up

- Người dùng sử dụng email, và phone number để đăng ký tài khoản
- Yêu cầu xác thực otp qua email hoặc phone number để xác minh địa chỉ email hoặc phone number là hợp lệ

## Sign in

- Người dùng có thể sử dụng email hoặc phone number để đăng nhập với password
- Trường hợp người dùng không muốn sử dung password có thể sử dụng chức năng đăng nhập với OTP

## Forgot password

- Người dùng có thể sử dụng email hoặc phone number để lấy lại mật khẩu
- Hệ thống sẽ gửi otp qua email hoặc phone number để xác minh địa chỉ email hoặc phone number là hợp lệ
- Người dùng nhập otp
- Người dùng nhập mật khẩu mới và xác nhận mật khẩu mới

## Profile

- Người dùng có thể cập nhật thông tin cá nhân. Thông tin cá nhân bao gồm:
  - Ảnh đại diện
  - Họ và tên
  - Phone number
  - Email
  - Ngày tháng năm sinh
  - Giới tính

## Terms and conditions

Người dùng được mặc đinh là đã đọc và đồng ý với điều khoản sử dụng của hệ thống để sử dụng hệ thống

## Search Component

Người dùng có thể tìm kiếm show theo các tiêu chí sau:

- Tên show
- Nghệ sĩ tham gia
- Địa điểm
- Thời gian diễn ra

### Trending Keyword Suggestions

Khi người dùng nhập từ khóa tìm kiếm, hệ thống sẽ đề xuất các từ khóa tìm kiếm phổ biến

### Recommended Shows

Khi người dùng click vào ô tìm kiếm, hệ thống sẽ đề xuất các show thuộc recommended shows. Hiển thị mặc định 6 show. Có button để xem thêm show. Khi click vào button này, hiển thị thêm 6 show nữa.

## Browse Shows

Có một filter để lọc show theo các category sau:

- Nhạc sống
... [TBD]

## Promoted Shows with Carousel

Có một carousel hiển thị các show trending

## Reccomended Shows

Người dùng có thể xem danh sách các show theo từng được đề xuất theo các tiêu chí sau:

- Sự kiện đặc biệt
- Xu hướng
- Sắp diễn ra (lọc theo thời gian ví dụ: tuần này, tháng này)

## Select Show (Option 1)

Trên danh sách show, người dùng có thể chọn show để xem chi tiết thông tin của show.
Chi tiết thông tin show bao gồm:

- Tên show
- Hình ảnh (banner)
- Thời gian diễn ra
- Địa điểm
- Giá vé
- Button để mua vé
- Giới thiệu show
- Danh sách showtimes
  Bao gồm:
  - Thời gian diễn ra (ngày, giờ)
  - Danh sách các loại(hạng) vé
    Thông tin hạng vé bao gồm:
    - Tên Hạng vé (vé VIP, vé thường, hoặc CAT, hoặc Zone,... tùy theo show).
    - Giá vé
  - Button để mua vé
- Danh sách các nghệ sĩ tham gia show (Optional)
- Thông tin về đơn vị tổ chức show
- Thông tin về đơn vị bảo trợ show (Optional)

Đối với mỗi show cần đề xuất các show liên quan. Xem tính năng Related Shows

### Related Shows

Khi xem chi tiết thông tin của một show, hệ thống cần đề xuất các show liên quan dựa trên các tiêu chí sau:

- Cùng thể loại
- Cùng nghệ sĩ tham gia
- Cùng đơn vị tổ chức
- Thời gian diễn ra gần với thơi gian diễn ra của show hiện tại

Hiển thị mặc định 8 show liên quan
Có button để xem thêm show liên quan. Khi click vào button này, hiển thị thêm 8 show liên quan nữa.

### Buy Ticket

Tại trang chi tiết show, tùy vào số lượng showtimes của show, hệ thống sẽ hiển thị button là `Mua vé` hoặc `Chọn showtime`.

#### Trường hợp 1: Show có nhiều showtimes

Nếu show có nhiều showtimes, button sẽ là `Chọn showtime`. Người dùng clich vào button Chọn showtime, hệ thống sẽ chuyển người dùng đến section chọn showtime. Ở đây, người dùng chọn showtime mà họ muốn mua vé.
Người dùng click vào button `Mua vé` ở showtime mà họ muốn mua vé thì behavior sẽ phụ thuộc vào việc show có seat map hay không.

Lưu ý quan trọng: Người dùng phải đăng nhập trước khi mua vé. Sau khi click vào button `Mua vé`, nếu người dùng chưa đăng nhập, hệ thống sẽ chuyển người dùng đến trang đăng nhập. Sau khi đăng nhập thành công, hệ thống sẽ chuyển người dùng đến trang mua vé.

##### Trường hợp 1.1: Show có seat map

Nếu show có seat map, hệ thống sẽ chuyển người dùng đến trang chọn ghế ngồi. Người dùng chọn ghế ngồi mà họ muốn mua vé. Sau khi chọn ghế ngồi, hệ thống sẽ hiển thị thông tin chi tiết về ghế ngồi đã chọn và giá vé tạm tính. Người dùng click vào button `Tiếp tục` để chuyển đến trang chọn hình thức thanh toán.

##### Trường hợp 1.2: Show không có seat map

Nếu show không có seat map, hệ thống sẽ chuyển người dùng đến trang chọn hạng vé. Người dùng chọn hạng vé mà họ muốn mua vé. Sau khi chọn hạng vé và số lượng vé, hệ thống sẽ hiển thị thông tin chi tiết về hạng vé đã chọn, số lượng, giá vé và tổng tiền tạm tính. Người dùng click vào button `Tiếp tục` để chuyển đến trang chọn hình thức thanh toán.

#### Trường hợp 2: Show chỉ có 1 showtime

Nếu show chỉ có 1 showtime, button sẽ là `Mua vé`. Người dùng click vào button `Mua vé` thì behavior sẽ đi theo các flow 1.1 hoặc 1.2 tùy vào việc show có seat map hay không.

### Seat Map

Khi chọn showtime của show có seat map, hệ thống sẽ hiển thị trang chọn ghế ngồi. Yêu cầu của trang chọn ghế ngồi như sau:

- Hiển thị seat map của show một cách trực quan theo layout của show
- Mỗi ghế ngồi có thể ở trạng thái:
  - Không thể chọn (đỏ)
  - Đang chọn (xanh lá)
  - Đang trống (trắng)
  Có legend để giải thích ý nghĩa của mỗi trạng thái
- Hiển thị thông tin cơ bản về showtime như tên show, thời gian diễn ra, địa điểm, hạng vé, giá vé. Sử dụng màu sắc và legend để giải thích ý nghĩa hạng vé và giá vé tương ứng.

### Order Summary (Option 1)

Bên phải trang mua vé, hiển thị order summary bao gồm:

- Showtime đã chọn
- Hạng vé đã chọn và sô lượng vé tương ứng
- Số ghế ngồi đã chọn (nếu có)
- Tổng tiền tạm tính
- Button `Tiếp tục` để chuyển đến trang chọn hình thức thanh toán

## Select Show (Option 2)

Tại danh sách show, người dùng có thể chọn show để mua vé. Khi click vào show, hệ thống sẽ chuyển người dùng đến trang mua vé. Trang mua vé bao gồm:

### Basic Information

Bao gồm:

- Tên show
- Hình ảnh (banner)
- Thời gian diễn ra
- Địa điểm
- Giá vé
- Button để xem chi tiết show

### Showtimes

Danh sách các showtimes của show được hiển thị ở bên trái. Mỗi showtime bao gồm ngày, giờ diễn ra. Khi click vào showtime, hệ thống sẽ tải component chọn ghế ngồi hoặc chọn hạng vé tùy vào việc show có seat map hay không.

#### Trường hợp 1: Show có seat map

Khi click vào showtime, hệ thống sẽ hiển thị trang chọn ghế ngồi. Yêu cầu của trang chọn ghế ngồi như sau:

- Hiển thị seat map của show một cách trực quan theo layout của show
- Mỗi ghế ngồi có thể ở trạng thái:
  - Không thể chọn (đỏ)
  - Đang chọn (xanh lá)
  - Đang trống (trắng)
  Có legend để giải thích ý nghĩa của mỗi trạng thái
  Hạng vé được hiển thị màu sắc khác nhau để phân biệt
  Có legend để giải thích ý nghĩa của mỗi màu sắc hạng vé và giá vé tương ứng.

#### Trường hợp 2: Show không có seat map

Khi click vào showtime, hệ thống sẽ hiển thị trang chọn hạng vé. Yêu cầu của trang chọn hạng vé như sau:

- Hiển thị danh sách các hạng vé của show
- Mỗi hạng vé bao gồm:
  - Tên hạng vé
  - Giá vé
  - Component chọn số lượng vé

### Order Summary (Option 2)

Bên phải trang mua vé, hiển thị order summary bao gồm:

- Showtime đã chọn
- Hạng vé đã chọn và sô lượng vé tương ứng
- Số ghế ngồi đã chọn (nếu có)
- Tổng tiền tạm tính
- Button `Tiếp tục` để chuyển đến trang chọn hình thức thanh toán

## Payment

Sau khi click `Tiếp tục` ở Order Summary, hệ thống sẽ chuyển người dùng đến trang Thanh toán. Trang thanh toán bao gồm:

- Thông tin nhận vé
  - Họ và tên
  - Email
  - Số điện thoại
  (Thông tin này sẽ được điền sẵn từ thông tin người dùng đã đăng ký)

- Order Summary
  - Showtime đã chọn
  - Hạng vé đã chọn và sô lượng vé tương ứng
  - Số ghế ngồi đã chọn (nếu có)
  - Nhập mã giảm giá (nếu có). Button `Áp dụng` để áp dụng mã giảm giá. Sau khi áp dụng mã giảm giá, hệ thống sẽ hiển thị giá vé đã giảm và tổng tiền tạm tính mới.
  - Tổng tiền tạm tính
  
- Hình thức thanh toán:
  - Momo
  - NAPAS

- Button `Thanh toán` để chuyển đến trang xác nhận thanh toán

Sau khi click vào button `Thanh toán`, hệ thống sẽ xử lý thanh toán và chuyển người dùng đến trang thanh toán được cung cấp bởi hệ thống thanh toán (3rd party).

### Trường hợp thanh toán thành công

Nếu thanh toán thành công, hệ thống sẽ chuyển người dùng trở về trang xác nhận mua vé thành công. Trang xác nhận mua vé thành công bao gồm:

- Thông tin chi tiết về vé đã mua
- Button để download vé

#### Confirmation Email

Sau khi mua vé thành công, hệ thống sẽ gửi email xác nhận mua vé thành công cho người dùng. Email xác nhận mua vé bao gồm:

- Thông tin chi tiết về vé đã mua
  - Mã đơn hàng
  - Số ghế ngồi (nếu có) / Khu vực ngồi (nếu có)
  - Hạng vé
  - Tên show
  - Showtime
  - Địa điểm
  - Điều khoản và điều kiện
  - Thông tin người mua vé: Họ và tên, email, số điện thoại
  - Chi tiết đơn hàng: Phương thức thanh toán, thời gian đặt vé
  - Số lượng vé, hạng vé, số tiền thực tế đã thanh toán
  - File đính kèm: Vé điện tử (PDF). Số lượng file đính kèm bằng số lượng vé đã mua.

### Trường hợp thanh toán thất bại

Nếu thanh toán thất bại, hệ thống sẽ chuyển người dùng trở về trang xác nhận thanh toán thất bại. Trang xác nhận thanh toán thất bại bao gồm:

- Thông báo lỗi
- Button để thử lại thanh toán

### Trường hợp hủy thanh toán

Nếu người dùng hủy thanh toán, hệ thống sẽ chuyển người dùng trở về trang xác nhận hủy thanh toán. Trang xác nhận hủy thanh toán bao gồm:

- Thông báo hủy thanh toán
- Button `Huỷ đơn hàng`
- Button `Tiếp tục mua vé`

#### Huỷ đơn hàng

Khi click vào button `Huỷ đơn hàng`, hệ thống sẽ xử lý hủy đơn hàng và chuyển người dùng trở về trang seat map hoặc chọn hạng vé tùy vào việc show có seat map hay không.

#### Tiếp tục mua vé

Khi click vào button `Tiếp tục mua vé`, hệ thống sẽ giữ người dùng ở trang thanh toán và giữ nguyên thông tin đã nhập trước đó để người dùng có thể tiếp tục thanh toán.

## My Tickets

Tên top menu: `Vé của tôi`
Người dùng click vào menu `Vé của tôi`, hệ thống sẽ chuyển người dùng đến trang `Vé của tôi`. Trang `Vé của tôi` bao gồm:

Nếu người dùng chưa đăng nhập, hệ thống sẽ chuyển người dùng đến trang đăng nhập trước khi chuyển đến trang `Vé của tôi`.

- Bên trái trang: Sidebar menu
  - Thông tin tài khoản
  - Vé đã mua
  - Sự kiện của tôi

- Ở giữa là danh sách các vé đã mua. Có thể lọc vé theo các tiêu chí sau: Tât cả, Thành công, Đang xử lý, Đã hủy. Đối với filter `Tất cả` và `Thành công`, có thêm sub-filter theo: Sắp diễn ra, Đã kết thúc. Kết quả hiển thị danh sách các vé đã mua. Mỗi vé bao gồm:
  - Tên show
  - Showtime
  - Địa điểm
  - Số lượng vé
  - Hạng vé
  - Số ghế ngồi (nếu có)
  - Tổng tiền
  - Button `Download vé`
  - Button `Hủy vé`

## Organizer Center

### Oganzier Dashboard

Dashboard chỉ available cho các nhà tổ chức lớn. Các nhà tổ chức nhỏ sẽ không nhìn thấy dashboard này.

### Show Management

#### Show List

#### Create Show

#### Edit Show

### Quản lý xuất file (TBD)

### Điều khoản và điều kiện cho ban tổ chức (TBD)