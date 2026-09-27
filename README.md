# 📸 DLog — Daily × Vlog

<p align="center">
  <b>Share your moments. Save your memories.</b>
</p>

<p align="center">
  Một ứng dụng mạng xã hội chia sẻ hình ảnh được phát triển trong khuôn khổ đồ án môn
  <b>Phát triển ứng dụng Mobile</b>.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Android-3DDC84?style=for-the-badge&logo=android&logoColor=white"/>
  <img src="https://img.shields.io/badge/Language-Java-orange?style=for-the-badge&logo=openjdk&logoColor=white"/>
  <img src="https://img.shields.io/badge/UI-Jetpack%20Compose-4285F4?style=for-the-badge&logo=jetpackcompose&logoColor=white"/>
  <img src="https://img.shields.io/badge/Firebase-Backend-FFCA28?style=for-the-badge&logo=firebase&logoColor=black"/>
</p>

---

## 📖 Giới thiệu

**DLog (Daily × Vlog)** là một ứng dụng mạng xã hội dành cho việc
**chia sẻ hình ảnh và lưu giữ những khoảnh khắc trong cuộc sống**.

Người dùng có thể đăng tải những bức ảnh của mình, viết caption,
tương tác với bài viết của người khác, theo dõi bạn bè và quản lý
trang cá nhân.

> 📷 **DLog — Share your moments.**

Ứng dụng được xây dựng nhằm áp dụng các kiến thức về:

- Phát triển ứng dụng Android
- Thiết kế giao diện Mobile
- Lập trình hướng đối tượng
- Cơ sở dữ liệu
- Xác thực người dùng
- Firebase
- Git & GitHub
- Làm việc nhóm và quản lý source code

---

## ✨ Tính năng

### 🔐 Tài khoản

- Đăng ký tài khoản
- Đăng nhập
- Đăng xuất
- Quên mật khẩu
- Chỉnh sửa thông tin cá nhân
- Thay đổi ảnh đại diện

### 🏠 Trang chủ

- Xem danh sách bài viết
- Xem bài viết mới
- Xem thông tin người đăng
- Like bài viết
- Bình luận bài viết
- Lưu bài viết

### 📝 Bài viết

- Đăng bài viết
- Upload hình ảnh
- Thêm caption
- Chỉnh sửa bài viết
- Xóa bài viết
- Xem chi tiết bài viết
- Like / Unlike
- Bình luận

### 👥 Mạng xã hội

- Theo dõi người dùng
- Hủy theo dõi
- Xem danh sách người theo dõi
- Xem danh sách đang theo dõi
- Xem trang cá nhân người khác
- Tìm kiếm người dùng

### 🔔 Thông báo

Người dùng có thể nhận thông báo khi:

- ❤️ Có người thích bài viết
- 💬 Có người bình luận
- 👤 Có người theo dõi

### 🔖 Tiện ích

- Lưu bài viết / hình ảnh
- Xem danh sách ảnh đã lưu

---

## 🖼️ Giao diện

> Một số màn hình chính của ứng dụng:

### 🔐 Authentication

| Login | Register | Forgot Password |
|:---:|:---:|:---:|
| *Coming soon* | *Coming soon* | *Coming soon* |

### 🏠 Main

| Home | Search | Post Detail |
|:---:|:---:|:---:|
| *Coming soon* | *Coming soon* | *Coming soon* |

### 👤 Profile

| My Profile | Edit Profile | Other Profile |
|:---:|:---:|:---:|
| *Coming soon* | *Coming soon* | *Coming soon* |

> 📌 Screenshot sẽ được cập nhật sau khi hoàn thiện giao diện Figma và Android.

---

## 🧩 Function Diagram

```text
                           ┌─────────────────┐
                           │      DLog       │
                           │ Photo Social App│
                           └────────┬────────┘
                                    │
        ┌──────────────┬────────────┼────────────┬──────────────┐
        │              │            │            │              │
        ▼              ▼            ▼            ▼              ▼
   👤 Account       📝 Post      👥 Social     🔍 Search     🔔 Notification
        │              │            │            │              │
        ├─ Register    ├─ Create    ├─ Follow    └─ User        ├─ Like
        ├─ Login       ├─ Edit      ├─ Unfollow     Search       ├─ Comment
        ├─ Logout      ├─ Delete    ├─ Followers                 └─ Follow
        └─ Profile     ├─ Like      └─ Following
                       └─ Comment

                              │
                              ▼
                         🔖 Saved Photos
