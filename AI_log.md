# Nhật ký lỗi và kiểm tra

Ngày ghi nhận: 2026-10-30

## Lỗi 1: Không hiện ảnh

- **Bước tái hiện:** Mở `index.html` và kiểm tra phần giao diện portfolio.
- **Kỳ vọng:** Ảnh `assets/vỹ.jpg` được hiển thị trong trang giới thiệu cá nhân.
- **Thực tế:** Không có ảnh nào xuất hiện.
- **Nguyên nhân:** Tệp `assets/vỹ.jpg` có tồn tại, nhưng `index.html` không có thẻ `<img>` và `css/style.css` cũng không có `background-image` tham chiếu đến tệp này.
- **Cách sửa đề xuất:** Thêm thẻ ảnh với đường dẫn tương đối `assets/vỹ.jpg` vào phần giới thiệu, đồng thời thêm `alt` mô tả ảnh.
- **Kiểm tra lại:** Sau khi sửa, tải lại `index.html` và xác nhận ảnh hiển thị; kiểm tra thêm ở kích thước màn hình nhỏ.

## Lỗi 2: Nghi ngờ sai đường dẫn

- **Bước kiểm tra:** Đối chiếu các đường dẫn trong `index.html`, `ket-qua.html` và `css/style.css` với cấu trúc thư mục.
- **Kết quả:** Chưa tái hiện được lỗi sai đường dẫn đối với CSS, liên kết nội bộ hoặc trang kết quả. Các đường dẫn `css/style.css`, `ket-qua.html` và các liên kết neo đều đúng.
- **Lưu ý:** Tệp ảnh nằm tại `assets/vỹ.jpg`; nếu thêm ảnh, phải dùng đúng thư mục `assets` và đúng tên tệp có dấu, hoặc đổi tên tệp sang tên không dấu rồi cập nhật tham chiếu tương ứng.
