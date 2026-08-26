# CW Datacenter iOS IPA Builder

Repository này chỉ dùng để build gói source `CW-Datacenter-iOS-1.6.0-GitHub-IPA-Build.zip` thành IPA unsigned bằng GitHub Actions.

## Cách dùng

1. Giữ đúng một gói source ZIP ở root repository.
2. Upload hoặc thay thế ZIP sẽ tự kích hoạt workflow **Build CW Datacenter iOS IPA**.
3. Có thể chạy thủ công tại **Actions → Build CW Datacenter iOS IPA → Run workflow**.
4. Khi thành công, tải artifact `CW-Datacenter-iOS-1.4.0`.

Tên artifact/IPA được giữ cố định để tương thích quy trình cũ. Phiên bản thật được workflow kiểm tra cả trước và sau khi compile: `1.6.0` build `10600`.

Nếu compile lỗi, workflow tải thêm artifact `CW-Datacenter-iOS-1.6.0-build-log` chứa `xcodebuild.log` để gửi lại kiểm tra.

IPA tạo ra là bản unsigned và cần được ký trước khi cài lên iPhone.
