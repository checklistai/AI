# Checklist Turnaround Air India - GitHub Pages

Bộ file này được chuyển đổi từ checklist Excel `Checklist_AI.xlsx` sang web tĩnh chạy miễn phí trên GitHub Pages.

## Cách dùng nhanh
1. Mở `index.html` bằng Chrome/Edge để test offline.
2. Nhập `Flight No.`, `Date`, `STA/Chocks on planned`.
3. Bấm `Now` để ghi Actual Time cho từng mốc, hoặc nhập thủ công.
4. Web tự tính:
   - Planned Time = Base Time + offset từng task.
   - Delay Y/N = Yes nếu Actual Time muộn hơn Planned Time.
   - Delay Minutes = Actual Time - Planned Time, dạng hh:mm; sớm hơn sẽ có dấu âm.
5. Dùng `Xuất CSV`, `In/PDF`, hoặc `Copy báo cáo` để lưu/gửi kết quả.

## Cách đưa lên GitHub Pages
1. Tạo repository mới trên GitHub, ví dụ: `turnaround-checklist-ai`.
2. Upload file `index.html` vào repository.
3. Vào Settings → Pages.
4. Source: chọn `Deploy from a branch`.
5. Branch: chọn `main` và folder `/root`.
6. Save. GitHub sẽ tạo link web dạng `https://<username>.github.io/turnaround-checklist-ai/`.

## Lưu ý quan trọng
- GitHub Pages là web tĩnh, dữ liệu sẽ được lưu trên trình duyệt bằng `localStorage`.
- Nếu cần toàn đội nhập dữ liệu và lưu tập trung để quản lý/audit, cần tích hợp thêm Google Sheets, Microsoft Lists, SharePoint List hoặc database riêng.
- Ảnh evidence/photo hiện ghi nhận tên file khi export; với website tĩnh không upload ảnh lên server.
