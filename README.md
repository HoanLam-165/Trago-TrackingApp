# 📍 TraGo – Geo-Tracking Journal App

**TraGo** là ứng dụng ghi lại hành trình di chuyển thời gian thực trên thiết bị Android, hỗ trợ đánh dấu địa điểm bằng hình ảnh và đồng bộ dữ liệu với máy chủ.

Dự án được sử dụng như một môi trường thực chiến để phát triển tính năng, kiểm thử API, logic nghiệp vụ và các vấn đề bảo mật hệ thống.

---

## 🚀 Tính năng chính

**📌 Real-time Tracking**
- Ghi nhận tọa độ GPS theo thời gian thực.
- Hiển thị lộ trình di chuyển trên bản đồ.
- **Tối ưu UX:** Tích hợp lệnh dừng theo dõi (Stop Tracking) ưu tiên hiển thị ngay trên thanh thông báo (Notification Bar) để thao tác nhanh mà không cần mở lại app.

**📷 Photo Markers**
- Đính kèm hình ảnh tại các vị trí cụ thể trên hành trình.

**🔄 Data Synchronization**
- Đồng bộ dữ liệu liền mạch giữa ứng dụng Android và Backend RESTful API.

**📴 Offline Mode**
- Lưu trữ dữ liệu cục bộ bằng Room Database khi mất kết nối.
- Tự động đồng bộ lại khi có mạng.

---

## 🛠 Tech Stack

| Thành phần | Công nghệ |
| :--- | :--- |
| **Mobile** | Kotlin, Android SDK |
| **Local Database** | Room Database |
| **Maps** | Google Maps API |
| **Backend** | Node.js, Express.js |
| **Database** | MySQL |
| **Testing Tools** | Postman, Chrome DevTools |

---

## 🧪 API Testing & Security Testing

Dự án tập trung mạnh vào kiểm thử backend và bảo mật API, đóng vai trò chứng minh năng lực của một Technical Tester.

### 🔹 API Testing
Xây dựng **Postman Collection** với hơn 15 kịch bản kiểm thử, tập trung vào các luồng nghiệp vụ chính:
> **Đăng ký / Đăng nhập** ➔ **Khởi tạo hành trình** ➔ **Đồng bộ dữ liệu** ➔ **Xuất bản lộ trình**

**Nội dung kiểm thử bao gồm:**
- Data Integrity (Tính toàn vẹn dữ liệu)
- Error Handling (Xử lý lỗi)
- API Validation (Kiểm tra dữ liệu đầu vào)
- Data Synchronization (Kiểm tra logic đồng bộ)
- Authentication & Authorization (Xác thực và phân quyền)

### 🔹 Security Testing (Thực chiến)

- **⚠️ Broken Authorization (IDOR):** Phát hiện lỗi logic cho phép người dùng trái phép truy cập và xem chi tiết hành trình của người khác thông qua việc thao túng ID trong API Request.
- **⚠️ Stored XSS:** Phát hiện lỗ hổng cho phép chèn script độc hại vào tên người dùng hoặc tên hành trình, gây nguy hiểm khi hệ thống quản trị hiển thị dữ liệu (Admin Dashboard).
- **⚠️ Input Validation & Logic Error:** Phát hiện lỗi nghiêm trọng khiến server bị **Crash (500 Internal Server Error)** khi API nhận Request Body rỗng hoặc sai định dạng trong quá trình xử lý đồng bộ.

---

## 👤 Contact

**Luyện Ngọc Lâm Hoan**
- 📧 Email: lamhoan.luyen@gmail.com
- 🔗 Portfolio: https://superficial-reward-cfb.notion.site/L-m-Hoan-Portfolio-API-Security-Logic-Testing-357cd8809d858020a5f8fce253e07e35?pvs=74
- 🔗 GitHub: [https://github.com/HoanLam-165](https://github.com/HoanLam-165)
