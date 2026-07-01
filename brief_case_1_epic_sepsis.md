# Brief Case & Harm Map: Epic Sepsis Model Failure

## 1. Brief Case Table

| Field | Bạn điền gì |
| :--- | :--- |
| **Tên case** | Epic Sepsis Model (ESM) Failure |
| **Ngành** | Y tế / symptom checker / health assistant |
| **Tổ chức / sản phẩm** | Epic Systems / Epic Sepsis Model |
| **Use case AI** | Dự đoán sớm sự khởi phát của nhiễm trùng huyết (sepsis) ở bệnh nhân nội trú để tự động phát cảnh báo cho nhân viên y tế hành động kịp thời. |
| **Thời điểm** | Tháng 6 năm 2021 (Thời điểm công bố nghiên cứu đánh giá độc lập của Đại học Michigan trên tạp chí JAMA Internal Medicine). |
| **Case xảy ra chuyện gì?** | Một nghiên cứu độc lập quy mô lớn phát hiện thuật toán dự đoán nhiễm trùng huyết được cài đặt sẵn trên hệ thống bệnh án điện tử Epic hoạt động kém hiệu quả hơn nhiều so với công bố của hãng. Hệ thống bỏ sót tới 2/3 số ca bệnh thực tế và tạo ra một lượng lớn cảnh báo giả, dẫn đến hội chứng lờn cảnh báo (alert fatigue) của nhân viên y tế và tăng nguy cơ chậm trễ điều trị cho bệnh nhân. |
| **Stakeholder bị ảnh hưởng** | Bệnh nhân nội trú (nguy cơ suy đa tạng, tử vong do phát hiện muộn); Bác sĩ và Điều dưỡng (quá tải thông tin, stress lâm sàng do cảnh báo giả liên tục). |
| **Số liệu chính** | - Mô hình **bỏ sót 67%** (2/3) số ca nhiễm trùng huyết thực tế.<br>- **86% số cảnh báo** được tạo ra là **cảnh báo giả** (False Positive).<br>- Chỉ số **AUROC thực tế đạt 0.63**, thấp hơn nhiều so với mức công bố **0.76 - 0.83** của Epic.<br>- Nghiên cứu thực hiện trên **38.455 đợt điều trị** của **27.722 bệnh nhân**. |
| **Trích nguồn ngắn** | Nghiên cứu của Wong và cộng sự (2021) trên tạp chí JAMA Internal Medicine chứng minh Epic Sepsis Model bỏ sót 67% ca nhiễm trùng huyết và 86% số cảnh báo là giả. |
| **Nguồn 1** | Wong, A., et al. (2021). "External Validation of a Widely Implemented Proprietary Sepsis Prediction Model." *JAMA Internal Medicine*, 181(8), 1065-1070. [Link nguồn](https://jamanetwork.com/journals/jamainternalmedicine/fullarticle/2781307) |
| **Nguồn 2** | STAT News. (June 21, 2021). "Epic Systems’ sepsis algorithm missed 67% of cases, study finds." [Link nguồn](https://www.statnews.com/2021/06/21/epic-systems-sepsis-algorithm-missed-67-percent-cases/) |
| **Ghi chú độ tin cậy** | **Primary Source** (Nghiên cứu khoa học độc lập được bình duyệt chéo) & **High-quality secondary source** (Báo chí y tế uy tín chuyên sâu). Các số liệu thống nhất và không có mâu thuẫn. |

---

## 2. Harm Map Worksheet

| High-risk moment | Stakeholder bị ảnh hưởng | Failure mode | Layer bắt đầu lỗi | Harm xảy ra là gì? | Harm lens | Severity | Scale | Probability | Frequency | Vì sao? |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| AI âm thầm phân tích các chỉ số sinh tồn của bệnh nhân nhưng **không phát cảnh báo** khi nhiễm trùng huyết thực tế đang bắt đầu khởi phát. | Bệnh nhân nội trú | **Over-reliance** | **Model** | Bệnh nhân bị bỏ sót "giờ vàng" để dùng kháng sinh và bù dịch, dẫn đến tiến triển sốc nhiễm trùng, suy đa tạng và tử vong. Bác sĩ ỷ lại vào hệ thống nên chủ quan giảm tần suất theo dõi thủ công. | Injury, Opportunity loss | **Critical** | **High** | **High** | **High** | Nhiễm trùng huyết tiến triển cực kỳ nhanh. Việc bỏ sót 67% số ca trong khi nhân viên y tế tin tưởng hệ thống là cực kỳ nguy hiểm và dễ dẫn đến tử vong. |
| AI liên tục **gửi cảnh báo giả** đến màn hình theo dõi của nhân viên y tế đối với các bệnh nhân không bị nhiễm trùng huyết. | Bác sĩ, Điều dưỡng, Bệnh nhân | **Harmful advice** | **Model** | Nhân viên y tế bị quá tải thông tin, sinh ra hội chứng "nhờn cảnh báo" và có xu hướng tắt hoặc lờ đi mọi cảnh báo y tế. Bệnh nhân bị chỉ định các can thiệp y tế không cần thiết (xét nghiệm cấy máu, dùng kháng sinh phổ rộng gây kháng thuốc). | Opportunity loss, Injury | **Medium** | **High** | **High** | **High** | Tỷ lệ cảnh báo giả lên tới 86% tạo áp lực cực lớn lên tài nguyên bệnh viện và thời gian của bác sĩ, đồng thời làm lu mờ những cảnh báo đúng. |
