# Sổ tiền

Một app gộp ba sổ: **Chi tiêu** (chi tiêu cá nhân, ngân sách tháng), **Quỹ nhóm** (thu, chi, báo cáo quỹ) và **Chia bill** (chia bill, cho vay, trả nợ). Chọn sổ ở thanh trên cùng; thanh dưới cùng là các mục của sổ đang mở. Cài được lên màn hình chính và dùng được khi mất mạng.

## Đưa lên GitHub Pages

1. Tạo một repository mới trên GitHub (để Public), ví dụ `so-tien`.
2. Tải toàn bộ file trong thư mục này lên nhánh `main`, giữ nguyên cấu trúc: `index.html`, `manifest.webmanifest`, `sw.js` và thư mục `icons/` nằm ở gốc repository.
3. Vào **Settings → Pages**, chọn **Deploy from a branch**, nhánh `main`, thư mục `/ (root)`, rồi bấm **Save**.
4. Chờ khoảng một phút, mở `https://<tên-tài-khoản>.github.io/so-tien/`.

## Cài lên điện thoại

- **iPhone (Safari):** mở trang, bấm nút Chia sẻ rồi chọn **Thêm vào Màn hình chính**.
- **Android (Chrome):** mở trang, bấm menu ⋮ rồi chọn **Thêm vào màn hình chính** hoặc **Cài đặt ứng dụng**.

## Dữ liệu từ ba app cũ

Sổ tiền dùng lại đúng chỗ lưu của ba app cũ, nên:

- **Mở bằng Safari/Chrome, cùng tài khoản GitHub Pages** (cùng địa chỉ `<tên-tài-khoản>.github.io`): dữ liệu cũ tự hiện ra, không phải làm gì.
- **Bản cài ở màn hình chính iPhone** có kho dữ liệu riêng cho từng app, nên cần chuyển tay:
  - Quỹ nhóm, Chia Bill: trong app cũ bấm sao lưu/xuất dữ liệu để sao chép, rồi trong Sổ tiền mở tab cuối của sổ bất kỳ (Thiết lập hoặc Báo cáo) → **Sao lưu và dữ liệu** → **Khôi phục** → dán vào → **Khôi phục**.
  - Sổ Chi Tiêu cũ không có nút sao lưu, nên các khoản đã ghi trong bản cài ở màn hình chính không chuyển sang được bằng cách này.

## Sao lưu

Mục **Sao lưu và dữ liệu** nằm ở cuối tab Thiết lập (sổ Chi tiêu) và tab Báo cáo (sổ Quỹ nhóm, Chia bill): lưu một file chứa cả ba sổ, khôi phục từ file hoặc từ đoạn dữ liệu dán vào, và xoá dữ liệu từng sổ. Dữ liệu chỉ nằm trong trình duyệt của máy, không gửi đi đâu; xoá dữ liệu trình duyệt hoặc gỡ app sẽ mất, nên hãy sao lưu thường xuyên.

## Cập nhật app

Sau khi sửa `index.html`, mở `sw.js` và tăng số phiên bản ở dòng `const CACHE = 'so-tien-v6'` (ví dụ thành `v2`). Điện thoại sẽ tải bản mới ở lần mở kế tiếp.
