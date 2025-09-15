---
title: "Portfolio - Phương Xương Đức"
description: "Các dự án STEM tiêu biểu"
---

#  Dự án: Mô hình phân loại rác thải bằng AI và IoT  
**Mục tiêu:** Xây dựng hệ thống phân loại rác bằng camera và AI.  
**Công nghệ:** Python (OpenCV, YOLOv8), Pygame (GUI), Arduino + L298 (điện tử).  
**Vai trò:**  
- Lập trình xử lý ảnh bằng Python + YOLOv8.  
- Xây dựng giao diện hiển thị kết quả nhận diện bằng Pygame.  
- Thiết kế và lắp ráp mạch Arduino + module L298 để điều khiển cơ cấu cơ khí.  
**Kết quả:**  
- Mô hình hoạt động thời gian thực, nhận diện rác hữu cơ/vô cơ chính xác ~90%.  
<iframe src="https://drive.google.com/file/d/1-wqpGlxZnTiOzT2HyFA41_EjQ1HWaNsS/preview" 
        width="640" height="480" allow="autoplay"></iframe>

---

# 🍅 Dự án: Mô hình phân loại cà chua sống – chín  

**Mục tiêu:** Tự động phân loại cà chua bằng cảm biến.  
**Công nghệ:** Arduino C++, cảm biến màu, cảm biến hồng ngoại, relay, servo, PCB thủ công.  
**Vai trò:**  
- Lập trình Arduino C++ để xử lý tín hiệu cảm biến & điều khiển relay.  
- Thiết kế logic FIFO (queue) lưu trạng thái từng quả cà chua.  
- Điều khiển servo gạt cà chua chín sang khay riêng.  
**Kết quả:**  
- Hệ thống chạy ổn định, có thể dừng băng chuyền chính xác, phân loại theo màu thành công.  
<iframe src="https://drive.google.com/file/d/1_bU1zOZZ7Gc4fuHFyMl2LXb0AtOJSCoH/preview" 
        width="640" height="480" allow="autoplay"></iframe> 
---

# 🚗 Dự án: Xe tự hành Arduino  

**Mục tiêu:** Giúp học sinh THCS học lập trình robot đơn giản.  
**Công nghệ:** Arduino Uno, mạch L298, 2 động cơ giảm tốc.  
**Vai trò:**  
- Phát triển thư viện C++ với các lệnh đơn giản: `di_thang()`, `queo_trai()`, `dung_lai()`.  
- Tích hợp thư viện vào Arduino IDE để học sinh dễ sử dụng.  
**Kết quả:**  
- Học sinh có thể lập trình xe chạy theo lộ trình mà không cần hiểu chi tiết mạch điện tử.  
**Ví dụ:**
- Để xe đi thẳng, thay vì nhập:
```cpp
// Khai báo chân điều khiển L298
int IN1 = 4;
int IN2 = 5;
int IN3 = 6;
int IN4 = 7;

void setup() {
  pinMode(IN1, OUTPUT);
  pinMode(IN2, OUTPUT);
  pinMode(IN3, OUTPUT);
  pinMode(IN4, OUTPUT);
}

void loop() {
  // Xe đi thẳng (cả 2 động cơ cùng quay tiến)
  digitalWrite(IN1, HIGH);
  digitalWrite(IN2, LOW);
  digitalWrite(IN3, HIGH);
  digitalWrite(IN4, LOW);
  
}
```
- Học sinh co thể nhập:

```cpp
#include "robot.h"
Robot xe(4, 5,  6, 7);

void setup(){}
void loop(){
        xe.di_thang();
}
```