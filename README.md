# Cảm biến chất lượng không khí MKE-S17 AGS10 I2C TVOC IAQ Sensor

**MKE-S17 AGS10 I2C TVOC IAQ Sensor** là cảm biến chất lượng không khí sử dụng để phát hiện và giám sát các **hợp chất hữu cơ dễ bay hơi (VOC)** trong môi trường. Cảm biến tích hợp **chip ASIC chuyên dụng** kết hợp công nghệ cảm biến khí và xử lý tín hiệu số, mang lại độ nhạy tốt, độ tin cậy cao, mức tiêu thụ điện năng thấp và khả năng hoạt động ổn định trong thời gian dài.

**MKE-S17 AGS10 I2C TVOC IAQ Sensor** sử dụng công nghệ cảm biến **MEMS** với vật liệu bán dẫn oxit kim loại, cho khả năng phản hồi nhanh khi nồng độ khí thay đổi và thời gian hồi phục ngắn. Tín hiệu đầu ra sử dụng chuẩn **I2C Digital**, giúp kết nối đơn giản với các vi điều khiển và hệ thống nhúng, giao tiếp I2C cũng cho phép kết nối nhiều thiết bị trên cùng một bus, giúp thuận tiện khi xây dựng các hệ thống cần nhiều cảm biến.

**MKE-S17 AGS10 I2C TVOC IAQ Sensor** đặc biệt phù hợp cho các ứng dụng cần **theo dõi và đánh giá chất lượng không khí trong nhà**, chẳng hạn như **giám sát không khí phòng làm việc, phòng học, phòng ngủ, hệ thống thông gió**. Ngoài ra, MKE-S17 có thể tích hợp vào **máy lọc không khí, thiết bị gia dụng thông minh, hệ thống HVAC, thiết bị IoT** để theo dõi xu hướng thay đổi của TVOC và đưa ra các cảnh báo hoặc điều khiển tự động phù hợp. Trong lĩnh vực **STEM và giáo dục**, MKE-S17 phù hợp để xây dựng các mô hình **trạm giám sát chất lượng không khí, thiết bị đo môi trường IoT, hệ thống cảnh báo VOC, nhà thông minh và các dự án thu thập dữ liệu môi trường**.

**MKE-S17 I2C AGS10 TVOC IAQ Sensor** hỗ trợ điện áp giao tiếp **3.3V và 5VDC**, cho phép kết nối với các bo mạch điều khiển phổ biến như **Arduino, Raspberry Pi, Jetson Nano, Micro:bit** và nhiều nền tảng khác. Sản phẩm đi kèm **cáp kết nối 4P XH2.54 – Dupont**, đảm bảo kết nối chắc chắn, ổn định và thuận tiện trong quá trình lắp đặt và sử dụng.

## Thông số kỹ thuật

- Điện áp cấp nguồn: 5VDC
- Chuẩn tín hiệu điều khiển: I2C (tần số ≤ 15kHz)
- Điện áp giao tiếp: TTL 3.3 / 5VDC
- Cảm biến sử dụng: AGS10 TVOC Gas Sensor ASAIR
- Dòng điện hoạt động: 28 ± 5mA
- Công suất tiêu thụ: 75mW
- Dải đo: 0 ~ 99.999ppb (TVOC)
- Độ chính xác: ±25% giá trị đo (tại 25°C / 50%RH)
- Chu kỳ lấy mẫu: ≥ 2 giây
- Thời gian gia nhiệt ban đầu: 120 giây
- Nhiệt độ làm việc: 0 ~ 50°C
- Độ ẩm làm việc: 0 ~ 95% RH
- Tuổi thọ: > 5 năm (tại 25°C, trong không khí sạch)
- Khí chuẩn thử nghiệm: Ethanol
- Khả năng tương thích:
  - Arduino
  - Raspberry Pi
  - Jetson Nano
  - Micro:bit
  - Và các board điều khiển 3.3/5VDC khác
- Thiết kế mạch:
  - Ổn định, chống nhiễu
  - Phù hợp cho ứng dụng học tập và thực tế
- Đi kèm cáp kết nối: 4P XH2.54 – Dupont

## Các chân tín hiệu

| MKE-S11 | Ghi chú                   |
| :-------: | :---------------------- |
| `GND`     | Chân cấp nguồn âm 0VDC    |
| `5V`     | Chân cấp nguồn dương 5VDC |
| `SDA`   | Chân tín hiệu I2C Serial Data|
| `SCL`   | Chân tín hiệu I2C Serial Clock|


## Hướng dẫn sử dụng

### Hướng dẫn kết nối
- Cấp nguồn 5VDC cho mạch qua hai chân `GND` và `5V`
- Kết nối chân `SCL` của cảm biến với chân I2C Clock của mạch điều khiển.
- Kết nối chân `SDA` của cảm biến với chân I2C Data của mạch điều khiển.

### Hướng dẫn sử dụng với Arduino Uno / Vietduino Uno / ESP32
- Trong **Tools / Library Manager**, tìm và cài đặt bộ thư viện tổng hợp **"MKE_ONE" by MakerEdu.vn**
- Mở chương trình mẫu tại **File / Examples / MKE_ONE / Sensor / MKE_S17_AGS10**
- Cấu hình board mạch tương ứng là **Arduino Uno / ESP32**, chọn đúng cổng **COM Port** của mạch và nhấn **Upload** để nạp chương trình.
- Cấp nguồn 5VDC cho mạch, kết nối chân `SDA` và `SCL` của cảm biến với chân điều khiển được khai báo trong chương trình.
- Xem kết quả mạch hoạt động theo chương trình đã nạp.

### Hướng dẫn lập trình với Micro:bit (kéo thả khối)

- Khởi động [Microsoft MakeCode](https://makecode.microbit.org/) và **Import** chương trình theo đường link sau: `https://github.com/makereduvn/mke_s17_ags10_microbit/`
- Kết nối mạch Micro:bit và **Download** chương trình.
- Cấp nguồn 5VDC cho mạch, kết nối chân `SDA` và `SCL` của cảm biến với chân điều khiển được khai báo trong chương trình.
- Xem kết quả mạch hoạt động theo chương trình đã nạp.

Nếu bắt đầu tự án mới cần cài đặt Extension **MKE_ONE_MICROBIT** trên [Microsoft MakeCode](https://makecode.microbit.org/) theo [hướng dẫn tại đây](https://github.com/makereduvn/MKE_ONE_MICROBIT). Sau khi cài đặt thành công, các khối lệnh của Extension **MKE_ONE_MICROBIT** sẽ xuất hiện trong danh sách block và sẵn sàng để sử dụng.

## Kích thước sản phẩm
![MKE-S17 AGS10](/extras/MKE-S17_1.jpg)

## Hình ảnh sản phẩm
![MKE-S17 AGS10](/extras/MKE-S17_2.png)
![MKE-S17 AGS10](/extras/MKE-S17_3.png)

## Miễn trừ trách nhiệm
Sản phẩm này là bo mạch phát triển được thiết kế phục vụ cho mục đích nghiên cứu, thử nghiệm và học tập, không phải là một thiết bị hoàn chỉnh. Trong trường hợp người dùng kết hợp mạch này với các linh kiện, thiết bị hoặc phần mềm khác để tạo thành một hệ thống hoặc sản phẩm hoàn chỉnh, mọi chức năng và tính phù hợp của sản phẩm sau cùng đều thuộc trách nhiệm của người dùng.
