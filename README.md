# Mạch Mtiny ESP8266 ESP-12S (Arduino Compatible)

![](/image/12s_01.jpg)

## Giới thiệu

Mạch Mtiny ESP8266 ESP-12S (Arduino Compatible) được nghiên cứu và và sản xuất bởi MakerLab.vn dựa trên module Wifi SoC ESP8266 ESP-12S từ Ai-Thinker, mạch có thiết kế nhỏ gọn tiện lắp đặt, dễ dàng kết nối và lập trình với phần mềm Arduino qua mạch nạp Mtiny Programmer với chuẩn nạp Mtiny Socket.

Mtiny là viết tắt của Maker Tiny là dự án tạo ra các mạch vi điều khiển với thiết kế nhỏ gọn sử dụng chuẩn chân cắm DIP 2.54mm, các mạch Mtiny cùng sử dụng chung mạch nạp chương trình và giao tiếp máy tính Mtiny Programmer với chuẩn nạp Mtiny Socket.

## Thông số kỹ thuật

<table><thead>
  <tr>
    <th>Model</th>
    <th>Mtiny ESP8266 ESP-12S (Arduino Compatible)</th>
  </tr></thead>
<tbody>
  <tr>
    <td>MCU</td>
    <td>Wifi SoC ESP8266 Espressif Systems</td>
  </tr>
  <tr>
    <td>Power Supply</td>
    <td>3V3 Pin: 3.0 ~ 3.6VDC, Typical 3.3VDC, Current &gt; 500mA</td>
  </tr>
  <tr>
    <td>Interface</td>
    <td>UART/HSPI/I2C/I2S/IR Remote Control GPIO/PWM</td>
  </tr>
  <tr>
    <td>SPI Flash</td>
    <td>Default 32Mbit</td>
  </tr>
  <tr>
    <td>UART Baudrate</td>
    <td>Support 300 ~ 4608000 bps, Default 115200 bps</td>
  </tr>
  <tr>
    <td>Wifi</td>
    <td>802.11 b/g/n support<br>802.11 n support (2.4 GHz), up to 72.2 Mbp</td>
  </tr>
  <tr>
    <td>Frequency Range</td>
    <td>2412 ~ 2484MHz</td>
  </tr>
  <tr>
    <td>Security</td>
    <td>WEP / WPA-PSK / WPA2-PSK</td>
  </tr>
  <tr>
    <td>Antenna</td>
    <td>PCB</td>
  </tr>
  <tr>
    <td>Button</td>
    <td>RST (Reset) / IO0</td>
  </tr>
  <tr>
    <td>Led</td>
    <td>Power Led</td>
  </tr>
  <tr>
    <td>Packet</td>
    <td>DIP18 (9x2) 2.54mm</td>
  </tr>
  <tr>
    <td>Programmer</td>
    <td><a href="https://wiki.makerlab.vn/index.php/M%E1%BA%A1ch_Mtiny_Programmer_(Arduino_Compatible)">Mạch Mtiny Programmer (Arduino Compatible)</a></td>
  </tr>
  <tr>
    <td>Programmer Connector</td>
    <td>Mtiny Socket - IDC 8-Pin (2x4)</td>
  </tr>
</tbody></table>

## Kích thước

![](/image/12s_02.jpg)

## Các tính năng vượt trội

1) Thiết kế nhỏ gọn với chuẩn chân cắm DIP 2.54mm, tương thích với hầu hết các loại BreadBoard thông dụng.

2) Thuộc Series Mtiny nên sử dụng chung mạch nạp chương trình và giao tiếp máy tính Mtiny Programmer với chuẩn nạp Mtiny Socket.

3) Bổ sung thêm các linh kiện giúp ổn định, chống nhiễu.

4) Sau khi đã nạp chương trình, có thể cấp nguồn linh hoạt cho mạch bằng mạch Mtiny Power (6~24VDC) hoặc cấp nguồn trực tiếp qua chân 3V3 (3~3.3VDC).

## Hình ảnh

![](/image/12s_03.jpg)

## Hướng dẫn sử dụng

### Hướng dẫn hàn Mtiny Socket và kết nối với Mạch Mtiny Programmer cho Mạch Mtiny ESP8266 ESP-12S

- Mạch Mtiny ESP8266 ESP-12S sử dụng mạch nạp Mtiny Programer với chuẩn nạp Mtiny Socket để nạp chương trình và cấp nguồn bằng máy tính, hàn Mtiny Socket sử dụng rào đực đôi Header 2x4pins theo chiều hướng lên và kết nối như sau:

![](/image/12s_04.jpg)

### Hướng dẫn nạp chương trình với Arduino sử dụng mạch Mtiny Programmer

#### Hướng dẫn sử dụng phần mềm Arduino cơ bản

1) Giới thiệu về Arduino

2) Ngôn ngữ lập trình Arduino

3) Cách cài đặt phần mềm Arduino IDE

4) Cách cài đặt Driver và nạp chương trình cho mạch Arduino / Arduino Compatible

5) Cách cài đặt các thư viện phần cứng Arduino Library

6) Cách sử dụng Serial Monitor & Serial Plotter trên phần mềm Arduino

#### Hướng dẫn kết nối và nạp chương trình cho Mạch Mtiny ESP8266 ESP-12S trên phần mềm Arduino

1) Kết nối máy tính: Kết nối Mạch Mtiny ESP8266 ESP-12S với Mạch Mtiny Programmer bằng cáp IDC 2x4pins, kết nối Mạch Mtiny Programmer với máy tính bằng cáp USB-C sẽ thấy Led nguồn PWR trên mạch Mtiny Programmer và Mtiny ESP8266 ESP-12S phát sáng:

![](/image/12s_05.jpg)
2) Cài đặt Driver: Mạch Mtiny Programmer sử dụng IC nạp chương trình và giao tiếp máy tính CH340, các bạn có thể tham khảo hướng dẫn cài đặt Driver tại đây cho hệ điều hành Windows, lưu ý hệ điều hành MacOS hoặc Linux sẽ tự nhận Driver mà không cần cài đặt.

3) Cấu hình mạch trên phần mềm Arduino: Để cấu hình mạch trên phần mềm Arduino chúng ta cần làm các bước sau:

- Copy đường link sau và dán vào mục File > Preferences > Additional boards manager URLs (trên Windows) hoặc Arduino IDE > Settings > Additional boards manager URLs (trên MacOS) sau đó nhấn OK:  

        <http://arduino.esp8266.com/stable/package_esp8266com_index.json>

![](/image/12s_06.png)

- Tiếp theo chọn Tools > Board > Boards Manager..., tìm từ khoá ESP8266 sẽ thấy mục "esp8266 by ESP8266 Comunity", nhấn Install và chờ đợi cho đến khi cài đặt hoàn tất:
![](/image/12s_07.png)
- Sau khi cài đặt hoàn tất, tắt và khởi động lại phần mềm Arduino, sau đó thiết lập Board tại Tools > Board > esp8266 > Generic ESP8266 Module và Port (cổng kết nối) cho mạch, nếu không xác định được cổng kết nối có thể ngắt kết nối mạch và kết nối lại đồng thời kiểm tra phần Port để thấy cổng kết nối mới của mạch xuất hiện:
![](/image/12s_08.png)
- Các thiết lập mặc định để nạp chương trình của mạch sẽ như hình dưới đây:

> **Lưu ý:**  
Flash Size của các bản Mtiny ESP8266 mặc định là 4MB, các bạn chọn các tuỳ chọn chia phân vùng phù hợp với mục đích sử dụng.

![](/image/12s_09.png)

- Sau khi đã hoàn thành các thiết lập cơ bản bạn có thể nạp chương trình Hello World Serial Monitor sau vào mạch để test bằng cách nhấn vào nút Upload hoặc chọn Sketch > Upload sẽ thấy chuỗi ký tự "Hello World" được truyền lên máy tính qua Serial Monitor trên phần mềm Arduino:

```ino
/*
  Hello World Serial Monitor Mtiny ESP8266
 Prints "Hello World"" to the Serial Monitor.
*/

void setup() {
  // initialize serial communications at 9600 bps:
  Serial.begin(9600);
}

void loop() {
  // print "Hello World" to the Serial Monitor:
  Serial.println("Hello World");
  // wait 1000 milliseconds before the next loop
  delay(1000);
}
```

![](/image/12s_10.png)

- Sau khi nạp chương trình các bạn bật Serial Monitor tại Tools > Serial Monitor chỉnh tốc độ Baudrate là 9600 thể thấy kết quả:

![](/image/12s_11.png)


### Hướng dẫn cấp nguồn sử dụng mạch Mtiny Power sau khi đã nạp chương trình

Trong các trường hợp đã nạp chương trình (không cần sử dụng đến mạch nạp), muốn cấp nguồn riêng cho các mạch Mtiny và các mạch khác trong hệ thống, các bạn có thể sử dụng mạch Mtiny Power kết nối với các chân 3V3-5V-GND trên Mtiny Socket như sau:

<table><thead>
  <tr>
    <td>Power Input</td>
    <td>USB-C: 5VDC (Support USB Power Bank)<br>Domino (VIN): 6~24VDC</td>
  </tr></thead>
<tbody>
  <tr>
    <td>Power Output</td>
    <td>5VDC - Max 500mA (USB-C Input)<br>5VDC - Max 1500mA (Domino Input)<br>3.3VDC - Max 700mA</td>
  </tr>
</tbody>
</table>

![](/image/mtiny_esp07s_12.jpg)

## Nhà phân phối

Có thể mua Mạch Mtiny ESP8266 ESP-07S (Arduino Compatible) tại các nhà phân phối sau:

- [Hshop.vn - Điện tử & Robot.](hshop.vn)
