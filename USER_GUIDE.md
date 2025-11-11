# HƯỚNG DẪN SỬ DỤNG MRZ READER

## YÊU CẦU HỆ THỐNG
- Windows 7/8/10/11 (64-bit)
- Không cần cài Python

## CÀI ĐẶT

### Cách 1: Tải file EXE (Đơn giản nhất)
1. Tải file `MRZ_Reader.exe` từ link được cung cấp
2. Double-click để chạy
3. Hoàn thành!

### Cách 2: Build từ source code
1. Cài Python 3.11+
2. Mở terminal tại thư mục source code
3. Cài dependencies:
   ```
   pip install -r requirements.txt
   ```
4. Chạy script build:
   ```
   build_exe.bat   .\build_exe.bat
   ```
5. File EXE sẽ được tạo trong thư mục `dist/`

## CÁCH SỬ DỤNG

### 1. Kéo thả ảnh
- Mở ứng dụng
- Kéo 1 hoặc nhiều ảnh passport vào khung "KÉO THẢ ẢNH VÀO ĐÂY"
- Đợi xử lý xong
- Xem thông tin khách trong bảng

### 2. Lắng nghe thư mục tự động
- Click nút "Chọn" bên cạnh "Thư mục lắng nghe"
- Chọn thư mục muốn theo dõi (VD: `C:\Scan\`)
- Click nút "Chọn" bên cạnh "Thư mục đã xử lý"
- Chọn thư mục lưu ảnh đã xử lý (VD: `C:\Processed\`)
- Click nút "▶️ BẮT ĐẦU QUÉT"
- Mỗi khi có ảnh mới trong thư mục lắng nghe, ứng dụng sẽ tự động đọc và hiển thị

### 3. Quét thư mục có sẵn
- Chọn thư mục lắng nghe
- Click nút "🔍 QUÉT THƯ MỤC"
- Tất cả ảnh trong thư mục sẽ được xử lý

### 4. Copy thông tin
- **Double-click** vào ô để copy nội dung
- **Right-click** để hiển thị menu copy
- **Ctrl+C** sau khi chọn ô

### 5. Xóa danh sách
- Click nút "🗑️ XÓA TẤT CẢ" để xóa toàn bộ danh sách

## XỬ LÝ SỰ CỐ

### Ứng dụng không chạy
- Tắt antivirus tạm thời
- Chạy với quyền Administrator (Right-click → Run as administrator)
- Kiểm tra Windows Defender có block file không

### Không đọc được MRZ
- Đảm bảo ảnh rõ nét, không bị mờ
- Vùng MRZ (2 dòng chữ dưới cùng passport) phải rõ ràng
- Thử xoay ảnh nếu bị ngược
- Định dạng hỗ trợ: JPG, PNG, JPEG

### Lỗi "Missing dependencies"
- Download và cài **Visual C++ Redistributable**:
  https://aka.ms/vs/17/release/vc_redist.x64.exe

## THÔNG TIN THÊM
- Ứng dụng lưu cấu hình trong file `mrz_config.json`
- Log xử lý hiển thị ở panel bên phải
- Chức năng "Điền vào Smile FO" sẽ được bổ sung sau

## HỖ TRỢ
- Email: [email của bạn]
- Phone: [số điện thoại]
