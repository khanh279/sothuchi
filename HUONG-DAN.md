# Sổ tiền

Một sổ duy nhất cho chi tiêu cá nhân, quỹ nhóm, chia bill và trả nợ. Cài được lên màn hình chính và dùng được khi mất mạng.

## Cách dùng

Thanh dưới cùng có ba mục:

- **Tổng quan:** chọn thời gian xem (Tháng, Năm, Tất cả, Tuỳ chọn), số tiền đã chi, khung Nợ (ai nợ tôi, tôi nợ ai; bấm **Đối soát** để xem ai trả cho ai), các bill, số dư từng quỹ và chi tiêu cá nhân theo mục.
- **Lịch sử:** chọn thời gian ở trên, rồi chọn một trong bốn ô Cá nhân, Quỹ, Chia bill, Trả nợ. Bấm vào từng khoản để sửa hoặc xoá.
- **Thiết lập:** ngân sách chi tiêu hàng tháng, danh sách người, các mục chi tiêu, sao lưu và dữ liệu.

Ở trang Tổng quan và Lịch sử có hai nút nổi:

- **+ Chi tiêu** (bên phải): nhập khoản chi cá nhân; đổi sang ô Quỹ ở đầu trang để nhập khoản chi của quỹ.
- **+ Quỹ, bill, nợ** (bên trái): Đóng quỹ, Chia bill, Trả nợ; mở lại đúng ô đang dùng lần trước.

Mỗi lần mở, app luôn vào trang Tổng quan.

Vài điểm nên biết:

- Dòng "Còn lại" và "mỗi ngày chi được khoảng" trên thẻ Đã chi chỉ hiện khi đã đặt ngân sách tháng trong Thiết lập.
- Danh sách người trong Thiết lập dùng để chọn thành viên khi chia bill, trả nợ và chọn nhanh khi đóng quỹ. Ở Đóng quỹ có thể gõ tên bất kỳ; tên tự gõ chỉ lưu trong khoản đóng đó.
- Phần "Đối soát" là cách trả gọn nhất để mọi người hết nợ, mỗi người chỉ trả một lần, nên đôi khi một người vừa nhận vừa trả.
- Số tiền ở quỹ, bill và nợ nhập theo nghìn đồng (k); chi tiêu cá nhân nhập theo đồng.
- Khi nhập bill, nút nhỏ bên trái ô chia của mỗi người đổi giữa "×" (chia theo hệ số) và "=" (trả một mức cố định, phần còn lại chia cho những người khác).
- Trong Lịch sử → Chia bill, mở một bill để tích từng khoản đã trả hoặc tích "Đã trả cả bill". Khoản đã tích không còn tính là nợ, nên đừng ghi thêm khoản đó ở Trả nợ.

## Đưa lên GitHub Pages

1. Tạo một repository mới trên GitHub (để Public), ví dụ `so-tien`.
2. Tải toàn bộ file trong thư mục này lên nhánh `main`, giữ nguyên cấu trúc: `index.html`, `manifest.webmanifest`, `sw.js` và thư mục `icons/` nằm ở gốc repository.
3. Vào **Settings → Pages**, chọn **Deploy from a branch**, nhánh `main`, thư mục `/ (root)`, rồi bấm **Save**.
4. Chờ khoảng một phút, mở `https://<tên-tài-khoản>.github.io/so-tien/`.

Nếu đã đưa bản Sổ tiền cũ lên rồi, chỉ cần tải đè các file mới lên đúng repository đó; điện thoại sẽ tự lấy bản mới ở lần mở kế tiếp (có thể phải đóng app rồi mở lại một lần).

## Cài lên điện thoại

- **iPhone (Safari):** mở trang, bấm nút Chia sẻ rồi chọn **Thêm vào Màn hình chính**.
- **Android (Chrome):** mở trang, bấm menu ⋮ rồi chọn **Thêm vào màn hình chính** hoặc **Cài đặt ứng dụng**.

## Dữ liệu từ ba app cũ

Sổ tiền dùng lại đúng chỗ lưu của ba app cũ (Sổ Chi Tiêu, Quỹ nhóm, Chia Bill), nên:

- **Mở bằng Safari/Chrome ở cùng địa chỉ `<tên-tài-khoản>.github.io`:** dữ liệu cũ tự hiện ra, không phải làm gì.
- **Bản cài ở màn hình chính iPhone** có kho dữ liệu riêng cho từng app, nên cần chuyển tay:
  - Quỹ nhóm, Chia Bill: trong app cũ bấm sao lưu/xuất dữ liệu để sao chép, rồi trong Sổ tiền vào **Thiết lập → Sao lưu và dữ liệu → Khôi phục**, dán vào và bấm **Khôi phục**.
  - Sổ Chi Tiêu cũ không có nút sao lưu, nên các khoản đã ghi trong bản cài ở màn hình chính không chuyển sang được bằng cách này.

## Sao lưu

Vào **Thiết lập → Sao lưu và dữ liệu** để lưu một file chứa toàn bộ sổ (chi tiêu, quỹ, bill, nợ, danh sách người), khôi phục từ file hoặc từ đoạn dữ liệu dán vào, và xoá dữ liệu từng phần. Dữ liệu chỉ nằm trong trình duyệt của máy, không gửi đi đâu; xoá dữ liệu trình duyệt hoặc gỡ app sẽ mất, nên hãy sao lưu thường xuyên.

## Cập nhật app

Sau khi sửa `index.html`, mở `sw.js` và tăng số phiên bản ở dòng `const CACHE = 'so-tien-v11'` (ví dụ thành `v12`). Điện thoại sẽ tải bản mới ở lần mở kế tiếp.
