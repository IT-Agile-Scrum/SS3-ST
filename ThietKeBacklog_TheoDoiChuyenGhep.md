# THIẾT KẾ BACKLOG CHO TÍNH NĂNG THEO DÕI CHUYẾN GHÉP

## Phần 1 - Thiết kế
- **Epic:** Theo dõi lộ trình và hỗ trợ sự cố chuyến ghép
  - **Feature 1:** Theo dõi thông tin lộ trình và thời gian
    - **User Story 1.1:** Là khách hàng đi xe ghép, tôi muốn xem được thứ tự và thời gian dự kiến xe đến đón mình, để tôi chủ động chuẩn bị trước.
    - **User Story 1.2:** Là khách hàng đi xe ghép, tôi muốn nhìn thấy vị trí thực tế của xe trên bản đồ, để biết xe đang đi đường nào và đi đón ai.
  - **Feature 2:** Hỗ trợ xử lý sự cố và thay đổi thông tin
    - **User Story 2.1:** Là khách hàng đi xe ghép, tôi muốn nhận được thông báo ngay lập tức nếu lộ trình bị thay đổi, để không bị bất ngờ khi xe đến muộn hơn dự kiến.
    - **User Story 2.2:** Là khách hàng đi xe ghép, tôi muốn có nút "Báo cáo sự cố/Gọi hỗ trợ" trên màn hình, để được trợ giúp ngay lập tức khi chuyến đi gặp vấn đề.

## Phần 2 - Sắp xếp Backlog
Thứ tự ưu tiên trong Product Backlog (từ cao xuống thấp):
1. **User Story 1.1:** Biết thời gian và thứ tự đón (Giải quyết ngay lập tức "bao giờ đến lượt mình" - nỗi bức xúc nhất của khách).
2. **User Story 1.2:** Nhìn thấy xe trên bản đồ (Trực quan hóa, giúp giải quyết câu hỏi "xe đang đón ai").
3. **User Story 2.1:** Nhận thông báo khi thay đổi (Giúp minh bạch thông tin khi có vấn đề phát sinh).
4. **User Story 2.2:** Nút Báo cáo sự cố (Giải pháp dự phòng, ít sử dụng hơn nên ưu tiên thấp nhất).

**Phân tích theo chuẩn D.E.E.P:** 
User Story **1.1** và **1.2** cần được làm rõ chi tiết nhất (Đại diện cho chữ **D - Detailed appropriately** trong D.E.E.P). Lý do là vì chúng nằm ở mức ưu tiên cao nhất, chuẩn bị được đưa vào Sprint kế tiếp nên cần có Acceptance Criteria rõ ràng và kích thước đủ nhỏ để Dev Team ước lượng (Estimated). Ngược lại, các Story ưu tiên thấp ở dưới (như 2.2) chỉ cần giữ ở dạng ý tưởng tổng quan và sẽ bổ sung chi tiết sau khi cần (Emergent).

## Phần 3 - Xử lý tình huống

**Tình huống 1: Đường Burndown Chart đi ngang 3 ngày liền (Thiếu dữ liệu bản đồ)**
- **Dấu hiệu nhận biết:** Đường thực tế (Actual effort line) chạy ngang song song với trục thời gian trong suốt 3 ngày liên tiếp, tách xa khỏi đường lý tưởng (Ideal line) đang hướng dần xuống 0.
- **Ai xử lý:** Scrum Master.
- **Xử lý thế nào:** Scrum Master đóng vai trò tháo gỡ trở ngại (Impediment remover) bằng cách hối thúc ngay đối tác bản đồ bàn giao dữ liệu; đồng thời làm việc với Development Team để linh hoạt chuyển sang làm các User Story khác không bị phụ thuộc, tránh để nhóm bị nghẽn tiến độ.

**Tình huống 2: PO muốn đưa nguyên Epic vào Sprint để "làm một lần cho xong"**
- **Ai xử lý:** Scrum Master (hoặc Agile Coach).
- **Xử lý thế nào:** Giải thích cho PO (Đức) hiểu rằng nhồi nhét cả một Epic lớn vào 1 Sprint sẽ phá vỡ quy tắc hộp thời gian (Time-box) và tiềm ẩn rủi ro làm không kịp. Hướng dẫn PO chỉ chọn những User Story mang lại giá trị cốt lõi nhất (như 1.1 và 1.2) để chạy trước, sớm tung ra lấy phản hồi, sau đó cải thiện dần ở các Sprint sau theo đúng tinh thần Agile.
