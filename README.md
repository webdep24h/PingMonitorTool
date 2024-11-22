# Ping Monitor

Ứng dụng giám sát ping và gửi thông báo qua Telegram.

![Banner](https://raw.githubusercontent.com/webdep24h/PingMonitorTool/main/images/Ping-monitor-telegram.png)


# [Hướng dẫn sử dụng phần mềm chi tiết dành cho người dùng]

---

### 🛠️ Tải xuống và chạy

[![Click để tải](https://raw.githubusercontent.com/webdep24h/PingMonitorTool/main/images/Download.png)](https://github.com/webdep24h/PingMonitorTool/raw/main/PingMonitor.rar)

Download tool tại: [PingMonitorTool](https://github.com/webdep24h/PingMonitorTool/raw/main/PingMonitor.rar)

---

![Ping](https://raw.githubusercontent.com/webdep24h/PingMonitorTool/main/images/ping-monitor.png)


### 📂 Cấu trúc thư mục
```plaintext
PingMonitor/
├── config/
│   ├── config.json # Chứa thông tin bot telegram, cần thay thông tin bot của bạn để sử dụng
│   └── hosts.json  # Chứa tin IP/ Thiết bị (Sử dụng PM "Quản lý file Hosts" đi kèm để thay đổi, chỉnh sửa)
├── File Import mẫu/ # Chứa các file dữ liệu mẫu cần Inport
├── PingMonitor.exe # Ứng dụng giám sát ping
└── Quản lý file Hosts # Ứng dụng quản lý, thêm sửa, xóa file hosts.json ở trên
```

### 📋 Hướng dẫn sử dụng

1. **Cài đặt Telegram Bot**:
   - Thay thông tin bot của bạn vào file `config/config.json`.

   ![Sửa thông tin file Bot Telegram](https://raw.githubusercontent.com/webdep24h/PingMonitorTool/main/images/ping-bot-telegram.png)  


2. **Cấu hình danh sách thiết bị giám sát**:
   - Sửa file `config/hosts.json` hoặc sử dụng ứng dụng **Quản lý file Hosts** để thêm/sửa/xóa thiết bị.
 

![Quản lý file Hosts](https://raw.githubusercontent.com/webdep24h/PingMonitorTool/main/images/ping-monitor-1.png)


![Chọn file Hosts](https://raw.githubusercontent.com/webdep24h/PingMonitorTool/main/images/ping-monitor-2.png)


![Thêm/ Xóa dữ liệu file Hosts](https://raw.githubusercontent.com/webdep24h/PingMonitorTool/main/images/ping-monitor-3.png)


3. **Chạy ứng dụng**:
   - Chạy file `PingMonitor.exe`.

4. **Xem kết quả**:
   - Kết quả được lưu trong file log hoặc gửi cảnh báo qua Telegram.


### 📌 Ghi chú

- **`config.json`**: Bạn cần thêm thông tin **Bot Token** và **Chat ID** của Telegram Bot.
- **`hosts.json`**: Chứa danh sách các thiết bị theo dõi. Định dạng mẫu:
  ```json
  [
    {"host": "192.168.1.1", "name": "Router"},
    {"host": "google.com", "name": "Google"}
  ]
   ```

## Chi tiết cách viết ứng dụng
https://blog.webdep24h.com/2024/11/ping-monitor.html

## Mã nguồn
https://github.com/webdep24h/ping_monitor
