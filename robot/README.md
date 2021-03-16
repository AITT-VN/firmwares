# Hướng dẫn cập nhật firmware cho các robot lắp ráp
## Cài đặt driver cho mạch điều khiển.
Để PC có thể nhận được Node WiFi thì bạn cần phải cài đặt driver:
1. Bạn download driver CH341SER.
2. Click vào INSTALL.

![Image](../images/ch340.png?raw=true)

Trong trường hợp có thông báo lỗi thì bạn có thể thử Uninstall rồi Install lại.

## Download tool uPyCraft để cập nhật firmware
Để cập nhật firmware cho board điều khiển của các robot lắp ráp, ta cần download và chạy phần mềm uPyCraft.
Bạn hãy download file uPyCraft_V1.1.exe về máy.

## Download firmware
Bạn download file firmware (file có đuôi là .bin) tùy thuộc vào dòng robot bạn đang muốn cập nhật.
- ArmBot -> armbot_xx.bin
- BatmanBot -> batmanbot_xx.bin
- PetBot -> petbot_xx.bin
- SpiderBot -> spiderbot_xx.bin
- TankBot -> tankbot_xx.bin
- TransformBot -> transformbot_xx.bin

với xx là số version của file firmware. Các bạn cứ chọn file có version mới nhất là tốt nhất.

## Update firmware trong uPyCraft
Sau khi download file uPyCraft_V1.1.exe, bạn hãy chạy để mở phần mềm uPyCraft. Nếu được hỏi có muốn cài đặt thêm font chữ hay không, bạn chọn Cancel.

![Image](../images/upycraft_install_font.png?raw=true)

Giao diện của uPyCraft:

![Image](../images/upycraft.png?raw=true)

Bạn vào menu Tools > BurnFirmware. Trong phần Firmware Choose, bạn chọn Users và chọn file .bin mà đã download ở trên. Các mục khác bạn để như trong hình dưới đây.

Mục com thì phần mềm sẽ tự động chọn cổng của board trên máy (số của cổng COM có thể khác nhau giữa các máy).

![Image](../images/upycraft_burn_firmware.png?raw=true)

Bạn click ok để bắt đầu flash firmware. Sau khi flash xong, bạn hãy reset board để firmware mới được chạy.
