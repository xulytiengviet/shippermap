# ShipperMap WebGIS

Ứng dụng quản lý bản đồ khách hàng và điểm giao hàng chạy trực tiếp trên GitHub Pages.

## Truy cập

https://xulytiengviet.github.io/shippermap/

## Chức năng

- Leaflet / OpenStreetMap, GPS, lựa chọn tọa độ trên bản đồ
- Thêm, sửa, xóa mềm, tìm kiếm khách, màu nhãn phân loại
- Ghi nhận lượt giao và COD; chọn các điểm để mở Google Maps dẫn đường
- Nhập CSV, xuất CSV, sao lưu và phục hồi JSON
- Giao diện responsive, PWA cache phần khung ứng dụng; dữ liệu lưu localStorage
- Nút tạo 24 khách mô phỏng TP.HCM

## Triển khai

Repository Settings > Pages > Build and deployment > Deploy from a branch > main / (root). Trang chủ là index.html.

## Giới hạn và bảo mật

Đây là **MVP offline-first trên từng thiết bị**, không phải backend đa người dùng: chưa có đăng nhập, phân quyền, đồng bộ cloud, chia sẻ link công khai có hạn hoặc xác thực. Dữ liệu trong localStorage không được mã hóa, không nên dùng với dữ liệu cá nhân nhạy cảm, điện thoại dùng chung hoặc khách hàng thật khi chưa xây dựng backend và chính sách bảo vệ dữ liệu. Không đưa dữ liệu khách hàng vào GitHub public. Bản đồ OSM/CDN cần mạng khi chưa được cache. Google Maps thực hiện dẫn đường bên ngoài ứng dụng. Không đưa mã PIN mẫu từ tài liệu tham khảo lên môi trường thật.

Thiết kế: Long Ngo · MIT 2026.\n\nNền bản đồ ưu tiên Vietflex (phiên bản CDN cố định), có fallback Leaflet/OpenStreetMap khi thư viện Vietflex không tải. Tiles Google legacy có thể chịu điều khoản và hạn chế riêng, không được MIT license của ứng dụng bao phủ.\n\nGiấy phép mã nguồn ứng dụng: xem [LICENSE](LICENSE).
