# Kịch bản chia sẻ dữ liệu
1. Khi giáo viên chia sẻ dữ liệu từ site đối tác ví dụ https://elearning.viettel.vn/ (Goi tắt Site đối tác)
2. Site đối tác gọi API vào api.igiaoduc.vn để thông báo, site ghi nhận và xử lý lần lượt các chia sẻ, xem ví dụ tại: 
3. api.igiaoduc.vn sẽ gọi vào API Site đối tác để lấy dữ liệu, lưu vào hệ thống, sau đó hiển thị cho người duyệt trên igiaoduc.vn
4. Người duyệt xong sẽ  hiển thị lên website igiaoduc.vn

# Cách gọi API trên site igiaoduc.vn
https://github.com/igiaoduc/document/wiki/H%C6%B0%E1%BB%9Bng-d%E1%BA%ABn-s%E1%BB%AD-d%E1%BB%A5ng-API-tr%C3%AAn-site-igiaoduc

# API Server trên site igiaoduc.vn
Website site https://igiaoduc.vn/ được viết bằng NukeViet 4.4

Xây dựng https://api.igiaoduc.vn dùng NukeViet 5 và viết thêm API để quản lý và phân quyền.

Kích hoạt API của Nukeviet 5:
1. Cấu hình => Cấu hình chung chọn  Bật Remote API
2. Tài khoản => Quản trị => Quản lý API roles => Thêm các role sau đó Vào Quyền truy cập API để cấp API cho từng admin

Các api chỗ Quản lý API roles hệ thống sẽ tự scan vào file để list,  Quy luật phải viết đúng:
1. Cho module https://wiki.nukeviet.vn/programming5:module:api
2. Cho hệ thống https://github.com/nukeviet/nukeviet/tree/develop/src/includes/api
