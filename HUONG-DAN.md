# Sổ Thu Chi

Một sổ duy nhất cho chi tiêu cá nhân, quỹ nhóm, chia bill và trả nợ. Cài được lên màn hình chính và dùng được khi mất mạng.

## Cách dùng

Thanh dưới cùng có ba mục:

- **Tổng quan:** chọn thời gian xem (Tháng, Năm, Tất cả, Tuỳ chọn), số tiền đã chi, số dư quỹ (dòng nhỏ ở đáy thẻ Đã chi, chỉ để xem, luôn tính từ trước đến nay; nhiều hơn 4 quỹ thì hiện 3 quỹ có số dư lớn nhất và gộp phần còn lại thành "+N quỹ"), khung Nợ (ai nợ tôi, tôi nợ ai; bấm **Đối soát** để xem ai trả cho ai), các bill và chi tiêu cá nhân theo mục.
- **Lịch sử:** chọn thời gian ở trên, rồi chọn một trong bốn ô Cá nhân, Quỹ, Chia bill, Trả nợ; dòng chữ nhỏ dưới tiêu đề ghi khoảng thời gian đang xem. Các khoản xếp theo ngày. Chạm một khoản chi tiêu hoặc trả nợ để sửa hoặc xoá; chạm một bill để xem chi tiết, rồi bấm Sửa hoặc Xóa.
- **Thiết lập:** ngân sách chi tiêu hàng tháng, danh sách người, các mục chi tiêu, sao lưu và dữ liệu.

Ở trang Tổng quan và Lịch sử có hai nút nổi:

- **+ Chi tiêu** (bên phải): nhập khoản chi cá nhân; đổi sang ô Quỹ ở đầu trang để nhập khoản chi của quỹ.
- **+ Quỹ, bill, nợ** (bên trái): Đóng quỹ, Chia bill, Trả nợ; mở lại đúng ô đang dùng lần trước.

Mỗi lần mở, app luôn vào trang Tổng quan. Từ trang nhập, nút Back của điện thoại đưa về trang vừa xem. Bấm Sửa một khoản trong Lịch sử, lưu hoặc huỷ xong app tự quay lại đúng chỗ đang xem. Chạm lại biểu tượng của trang đang đứng để cuộn về đầu trang.

Vài điểm nên biết:

- Dòng "Còn lại" và "mỗi ngày chi được khoảng" trên thẻ Đã chi chỉ hiện khi đã đặt ngân sách tháng trong Thiết lập.
- Danh sách người trong Thiết lập dùng để chọn thành viên khi chia bill, trả nợ và chọn nhanh khi đóng quỹ. Ở Đóng quỹ có thể gõ tên bất kỳ; tên tự gõ chỉ lưu trong khoản đóng đó.
- Phần "Đối soát" là danh sách ai trả cho ai để cả nhóm hết nợ. Nếu nợ trực tiếp đã gọn thì giữ nguyên ai nợ ai trả người đó; nếu có người phải trả nhiều nơi thì app gộp nợ để mỗi người chỉ trả một lần, nên đôi khi một người vừa nhận vừa trả. Các dòng "Nợ tôi / Tôi nợ" phía trên lấy từ chính danh sách này nên luôn khớp với Đối soát.
- Mọi số tiền trong app đều hiển thị theo đồng (₫). Khi nhập, quỹ, bill và nợ gõ theo nghìn (ô nhập có sẵn đuôi ".000 ₫" và tự thêm dấu chấm hàng nghìn, gõ 7000 hiện 7.000 tức 7.000.000 ₫); chi tiêu cá nhân gõ đủ số đồng, có nút nhập nhanh +5k đến +500k.
- Chia bill: mỗi dòng gồm tên, số tiền đóng và hệ số; chuyển sang trả cố định thì ô nhập mức cố định hiện ngay bên dưới.
- Ở Tổng quan, số dư từng quỹ hiện nhỏ ở cuối khung tổng chi (tối đa 4 quỹ, quỹ còn lại gộp thành "+N quỹ"; chạm vào đó để xem tất cả, chạm "Thu gọn" để thu lại).
- Khi nhập bill, bấm ô mục chi (dưới ô nội dung) để chọn mục như chi tiêu cá nhân. Chi tiêu cá nhân từ bill được ghi theo tiền thật sự bạn bỏ ra: phần bạn tự trả cho mình được ghi ngay ngày của bill (tên "… (chia bill)"); phần bạn còn nợ người khác chỉ được ghi khi bạn trả qua Đối soát, theo ngày trả (tên "Trả …"). Dòng chữ nhỏ dưới mỗi khoản ghi rõ bill nào (tên, ngày, tổng, phần của bạn); Lịch sử → Trả nợ cũng ghi khoản trả đó trả cho bill nào. Tiền người khác trả lại bạn và phần trả dư chuyển hộ người khác không tính là chi tiêu. Sửa / xoá bill hoặc khoản trả nợ thì các khoản này tự cập nhật.
- Khi nhập bill, nút nhỏ bên trái ô chia của mỗi người đổi giữa "×" (chia theo hệ số) và "=" (trả một mức cố định, phần còn lại chia cho những người khác).
- Trong **Đối soát**, bấm vào một dòng để ghi thanh toán: bấm "Toàn bộ" hoặc nhập số tiền rồi bấm Lưu. Khoản này được lưu vào Lịch sử → Trả nợ (ghi chú "Đối soát"), sửa hoặc xoá ở đó như mọi khoản trả nợ khác.

## Đưa lên GitHub Pages

1. Tạo một repository mới trên GitHub (để Public), ví dụ `so-tien`.
2. Tải toàn bộ file trong thư mục này lên nhánh `main`, giữ nguyên cấu trúc: `index.html`, `manifest.webmanifest`, `sw.js` và thư mục `icons/` nằm ở gốc repository.
3. Vào **Settings → Pages**, chọn **Deploy from a branch**, nhánh `main`, thư mục `/ (root)`, rồi bấm **Save**.
4. Chờ khoảng một phút, mở `https://<tên-tài-khoản>.github.io/so-tien/`.

Nếu đã đưa bản Sổ Thu Chi cũ lên rồi, chỉ cần tải đè các file mới lên đúng repository đó; điện thoại sẽ tự lấy bản mới ở lần mở kế tiếp (có thể phải đóng app rồi mở lại một lần).

## Cài lên điện thoại

- **iPhone (Safari):** mở trang, bấm nút Chia sẻ rồi chọn **Thêm vào Màn hình chính**.
- **Android (Chrome):** mở trang, bấm menu ⋮ rồi chọn **Thêm vào màn hình chính** hoặc **Cài đặt ứng dụng**.

## Dữ liệu từ ba app cũ

Sổ Thu Chi dùng lại đúng chỗ lưu của ba app cũ (Sổ Chi Tiêu, Quỹ nhóm, Chia Bill), nên:

- **Mở bằng Safari/Chrome ở cùng địa chỉ `<tên-tài-khoản>.github.io`:** dữ liệu cũ tự hiện ra, không phải làm gì.
- **Bản cài ở màn hình chính iPhone** có kho dữ liệu riêng cho từng app, nên cần chuyển tay:
  - Quỹ nhóm, Chia Bill: trong app cũ bấm sao lưu/xuất dữ liệu để sao chép, rồi trong Sổ Thu Chi vào **Thiết lập → Sao lưu và dữ liệu → Khôi phục**, dán vào và bấm **Khôi phục**.
  - Sổ Chi Tiêu cũ không có nút sao lưu, nên các khoản đã ghi trong bản cài ở màn hình chính không chuyển sang được bằng cách này.

## Sao lưu

Vào **Thiết lập → Sao lưu và dữ liệu** để lưu một file chứa toàn bộ sổ (chi tiêu, quỹ, bill, nợ, danh sách người), khôi phục từ file hoặc từ đoạn dữ liệu dán vào, và xoá dữ liệu từng phần. Dữ liệu chỉ nằm trong trình duyệt của máy, không gửi đi đâu; xoá dữ liệu trình duyệt hoặc gỡ app sẽ mất, nên hãy sao lưu thường xuyên.

## Cập nhật app

Sau khi sửa `index.html`, mở `sw.js` và tăng số phiên bản ở dòng `const CACHE = 'so-tien-v40'` (ví dụ thành `v41`). Điện thoại sẽ tải bản mới ở lần mở kế tiếp.
