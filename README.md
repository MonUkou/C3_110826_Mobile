# 📸 Dlog

> **Dlog – Share your moments.**

Dlog là một ứng dụng di động cho phép người dùng **chia sẻ những khoảnh khắc bằng hình ảnh**, tương tác với cộng đồng và quản lý trang cá nhân.

Dự án được xây dựng trong khuôn khổ **đồ án Mobile**, với mục tiêu áp dụng kiến thức về phát triển ứng dụng di động, thiết kế giao diện, quản lý dữ liệu và làm việc nhóm bằng Git/GitHub.

---

## 📱 Giới thiệu

Trong cuộc sống hằng ngày, người dùng thường lưu giữ rất nhiều khoảnh khắc dưới dạng hình ảnh nhưng không có một không gian đơn giản để chia sẻ và tương tác với những người xung quanh.

**Dlog** hướng đến việc xây dựng một mạng xã hội hình ảnh nhỏ gọn, tập trung vào trải nghiệm:

- 📸 Chia sẻ những khoảnh khắc đáng nhớ
- ❤️ Tương tác với bài viết
- 💬 Trao đổi thông qua bình luận
- 👤 Xây dựng trang cá nhân
- 🔍 Tìm kiếm người dùng và nội dung
- 👥 Kết nối với những người dùng khác

> **Dlog = Diary + Log**  
> Một nơi để lưu lại và chia sẻ những khoảnh khắc trong cuộc sống.

---

## 🎯 Mục tiêu dự án

Dự án hướng đến các mục tiêu:

- Xây dựng một ứng dụng chia sẻ hình ảnh trên nền tảng mobile.
- Thiết kế giao diện đơn giản, hiện đại và dễ sử dụng.
- Áp dụng kiến trúc và quy trình phát triển ứng dụng mobile thực tế.
- Làm quen với việc quản lý mã nguồn bằng Git và GitHub.
- Phân chia công việc và phối hợp phát triển trong nhóm.
- Áp dụng cơ sở dữ liệu và hệ thống xác thực người dùng.
- Hoàn thiện một sản phẩm có thể trình diễn trong đồ án.

---

## ✨ Tính năng dự kiến

### 🔐 Tài khoản

- [ ] Đăng ký tài khoản
- [ ] Đăng nhập
- [ ] Đăng xuất
- [ ] Quản lý thông tin cá nhân
- [ ] Thay đổi ảnh đại diện
- [ ] Chỉnh sửa hồ sơ

### 🏠 Trang chủ

- [ ] Hiển thị danh sách bài viết
- [ ] Xem bài viết mới
- [ ] Xem thông tin người đăng
- [ ] Tương tác với bài viết

### 📸 Bài viết

- [ ] Đăng hình ảnh
- [ ] Thêm caption
- [ ] Chỉnh sửa bài viết
- [ ] Xóa bài viết
- [ ] Xem chi tiết bài viết
- [ ] Like bài viết
- [ ] Bình luận

### 👥 Mạng xã hội

- [ ] Theo dõi người dùng
- [ ] Hủy theo dõi
- [ ] Xem danh sách người theo dõi
- [ ] Tìm kiếm người dùng
- [ ] Xem trang cá nhân người dùng khác

### 🔎 Tìm kiếm

- [ ] Tìm kiếm người dùng
- [ ] Tìm kiếm bài viết
- [ ] Tìm kiếm theo từ khóa

### 🔔 Thông báo

- [ ] Thông báo lượt thích
- [ ] Thông báo bình luận
- [ ] Thông báo người theo dõi

### 🔖 Tiện ích

- [ ] Lưu bài viết yêu thích
- [ ] Quản lý bài viết đã lưu
- [ ] Xóa bài viết khỏi danh sách lưu

> **Lưu ý:** Các tính năng trên là định hướng ban đầu và có thể được điều chỉnh trong quá trình phát triển dự án.

---

## 🛠️ Công nghệ sử dụng

Dự kiến dự án sử dụng:

| Công nghệ | Mục đích |
|---|---|
| **Kotlin** | Ngôn ngữ lập trình |
| **Android Studio** | Môi trường phát triển |
| **Jetpack Compose** | Xây dựng giao diện |
| **Firebase Authentication** | Xác thực người dùng |
| **Cloud Firestore** | Lưu trữ dữ liệu |
| **Firebase Storage** | Lưu trữ hình ảnh |
| **Git** | Quản lý phiên bản |
| **GitHub** | Quản lý source code và làm việc nhóm |

> Công nghệ có thể được cập nhật khi nhóm hoàn thiện thiết kế kỹ thuật.

---

## 🏗️ Kiến trúc dự kiến

Dlog hướng đến việc tổ chức ứng dụng theo kiến trúc có khả năng mở rộng và dễ bảo trì.

```text
┌─────────────────────────────┐
│          Dlog App           │
├─────────────────────────────┤
│                             │
│       Presentation          │
│    Jetpack Compose UI       │
│                             │
├─────────────────────────────┤
│                             │
│       ViewModel / State     │
│                             │
├─────────────────────────────┤
│                             │
│        Repository           │
│                             │
├─────────────────────────────┤
│                             │
│           Firebase          │
│                             │
│  ┌────────┐ ┌────────────┐  │
│  │  Auth  │ │ Firestore  │  │
│  └────────┘ └────────────┘  │
│                             │
│       Firebase Storage      │
│                             │
└─────────────────────────────┘
