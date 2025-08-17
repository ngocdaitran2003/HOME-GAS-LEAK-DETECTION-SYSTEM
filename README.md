# HOME-GAS-LEAK-DETECTION-SYSTEM
Hệ thống sử dụng một vi xử lý kết hợp với các cảm biến phát hiện khí gas và phát hiện lửa. Hệ thống sẽ tự động điều khiển cơ cấu chấp hành khi phát hiện sự cố rò rỉ. Thiết bị kết nối với wifi trong nhà để gửi dữ liệu đến server. Dữ liệu hiển thị trên phần mềm dưới dạng biểu đồ. 

Hệ thống có chức năng cảnh báo khi phát hiện khí gas vượt ngưỡng và cho phép người quản lý theo dõi từ xa qua thiết bị di động. Người dùng có thể cài đặt điều khiển thủ công hoặc tự động cho hệ thống khi gặp sự cố. 

Số lượng thành viên: 4 thành viên

## Phần cứng
- ESP32
- Sensor: MQ2, DHT11
- Cơ cấu chấp hành: relay, servo, quạt gió, máy bơm, còi
- Màn hình LCD16x2
- nút nhấn

## Phần mềm 
- Arduino IDE
- Node-Red Dashboard
- MQTT Mosquitto

## Sơ đồ khối
<img src = "https://github.com/ngocdaitran2003/HOME-GAS-LEAK-DETECTION-SYSTEM/blob/main/image/so_do_khoi.png">

## Mô hình 
Nhóm dựng mô hình một căn nhà để thực nghiệm hệ thống	

<img src = "https://github.com/ngocdaitran2003/HOME-GAS-LEAK-DETECTION-SYSTEM/blob/main/image/mo_hinh_sp.jpg">

## Giao diện Node-Red
Qua việc tìm hiểu và tham khảo các dashboard, ta xây dựng một dashboard theo ý muốn của bản thân và thân thiện với người dùng. 
Trong mỗi bảng biểu đồ, ta thiết lập các flow(đường dẫn) để thiết lập kết nối giữa các node như node xử lý, node hiển thị, node điều khiển, node thông báo, node gửi và nhận dữ liệu từ mqtt.

<img src = "https://github.com/ngocdaitran2003/HOME-GAS-LEAK-DETECTION-SYSTEM/blob/main/image/giao_dien_web.png">
