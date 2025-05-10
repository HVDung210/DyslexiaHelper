# Ứng dụng Đọc Sách Hỗ Trợ Người Khó Đọc

## Tổng Quan
Đây là một ứng dụng Android được thiết kế để hỗ trợ người khó đọc (dyslexic). Ứng dụng cung cấp các tính năng như trải nghiệm đọc tùy chỉnh, xác thực người dùng, quản lý sách và tích hợp với backend để hiển thị hình ảnh, mô tả và phát âm từ.

## Tính Năng
- Xác thực người dùng (Firebase)
- Thư viện sách và giao diện đọc
- Tùy chỉnh font chữ, màu sắc và đánh dấu cho người khó đọc
- Tra cứu từ với hình ảnh, mô tả và phát âm (thông qua backend)
- Nhập sách (EPUB, PDF, DOCX)
- Theo dõi tiến độ và đánh dấu trang

## Cấu Trúc Dự Án
- `app/src/main/java/com/example/myapplication/`: Mã nguồn chính của ứng dụng
  - `adapter/`, `controller/`, `model/`, `utils/`: Logic ứng dụng, mô hình dữ liệu và tiện ích
  - `MainActivity.java`: Điểm vào và đăng nhập
  - `ReadingActivity.java`: Giao diện đọc chính
- `app/src/main/res/`: Tài nguyên (layouts, drawables, v.v.)
- `app/build.gradle.kts`: Cấu hình build và dependencies

## Dependencies
- Firebase (Auth, Database, Analytics)
- Google ML Kit (Nhận dạng văn bản)
- Gson, OkHttp, iTextPDF, EpubLib, Mammoth (xử lý file)
- Material Components, AndroidX, Jetpack Compose

## Cách Build & Chạy
1. Mở dự án trong Android Studio.
2. Đảm bảo bạn có file `google-services.json` hợp lệ cho Firebase trong thư mục `app/`.
3. Đồng bộ Gradle và build dự án.
4. Chạy trên máy ảo hoặc thiết bị Android.

## Cấu Hình
- Cần thiết lập Firebase (`google-services.json`)
- URL API backend cần được cấu hình trong ứng dụng để sử dụng tính năng tra cứu từ. 