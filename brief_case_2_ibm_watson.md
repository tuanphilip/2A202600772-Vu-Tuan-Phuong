# Brief Case & Harm Map: IBM Watson for Oncology Unsafe Recommendations

## 1. Brief Case Table

| Field | Bạn điền gì |
| :--- | :--- |
| **Tên case** | IBM Watson for Oncology Unsafe Recommendations |
| **Ngành** | Y tế / symptom checker / health assistant |
| **Tổ chức / sản phẩm** | IBM / Watson for Oncology (Hệ thống siêu máy tính hỗ trợ điều trị ung thư) |
| **Use case AI** | Hỗ trợ quyết định lâm sàng (Clinical Decision Support) - Đọc hồ sơ bệnh án và đề xuất phác đồ điều trị ung thư tối ưu cho bác sĩ. |
| **Thời điểm** | Tháng 7 năm 2018 (Phóng sự điều tra của STAT News dựa trên tài liệu rò rỉ của IBM). |
| **Case xảy ra chuyện gì?** | Các tài liệu nội bộ bị rò rỉ tiết lộ Watson for Oncology thường xuyên đưa ra các khuyến nghị điều trị ung thư không chính xác, lỗi thời và nguy hiểm cho tính mạng bệnh nhân. Nguyên nhân cốt lõi là do hệ thống được huấn luyện phần lớn trên các ca bệnh giả định ("synthetic cases") do các bác sĩ tại Memorial Sloan Kettering tự biên soạn, thay vì sử dụng dữ liệu bệnh nhân thực tế ngoài đời thực, dẫn đến việc mô hình thiếu sự kiểm chứng lâm sàng thực tế và bị thiên lệch nặng nề. |
| **Stakeholder bị ảnh hưởng** | Bệnh nhân ung thư (nguy cơ gặp biến chứng nghiêm trọng hoặc tử vong do phác đồ điều trị nguy hiểm); Bác sĩ điều trị (bị dẫn dắt bởi thông tin sai lệch). |
| **Số liệu chính** | - Hệ thống đã hỗ trợ điều trị cho hơn **84.000 bệnh nhân** tại **230 bệnh viện** toàn cầu trước khi bị phanh phui.<br>- Đề xuất phác đồ chứa thuốc **Bevacizumab** (thuốc có cảnh báo hộp đen FDA về nguy cơ gây xuất huyết tử vong) cho một bệnh nhân ung thư phổi 65 tuổi đang bị **xuất huyết nặng**.<br>- Dự án thất bại hoàn toàn về mặt thương mại và IBM phải bán tháo tài sản của Watson Health vào năm 2022 với mức định giá chỉ còn khoảng **1 tỷ USD** (so với hàng tỷ USD đầu tư ban đầu). |
| **Trích nguồn ngắn** | Phóng sự của STAT News (2018) trích dẫn tài liệu nội bộ thừa nhận hệ thống Watson đưa ra những khuyến nghị "không an toàn và không chính xác" và được huấn luyện trên dữ liệu giả lập. |
| **Nguồn 1** | STAT News. (July 25, 2018). "IBM’s Watson gave ‘unsafe and incorrect’ cancer treatments, internal documents show." [Link nguồn](https://www.statnews.com/2018/07/25/ibm-watson-unsafe-cancer-treatment-recommendations/) |
| **Nguồn 2** | HealthCare Dive. (July 26, 2018). "IBM defended Watson for Oncology after report of 'unsafe' cancer recommendations." [Link nguồn](https://www.healthcaredive.com/news/ibm-defended-watson-for-oncology-after-report-of-unsafe-cancer-recommend/528682/) |
| **Ghi chú độ tin cậy** | **High-quality secondary source** (Phóng sự điều tra chuyên sâu của tờ báo công nghệ sinh học/y tế hàng đầu dựa trên tài liệu thuyết trình nội bộ của Phó giám đốc y tế IBM Watson Health). Không có mâu thuẫn số liệu. |

---

## 2. Harm Map Worksheet

| High-risk moment | Stakeholder bị ảnh hưởng | Failure mode | Layer bắt đầu lỗi | Harm xảy ra là gì? | Harm lens | Severity | Scale | Probability | Frequency | Vì sao? |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| AI đề xuất phác đồ điều trị cụ thể cho bệnh nhân dựa trên dữ liệu bệnh án lâm sàng. | Bệnh nhân ung thư | **Harmful advice** | **Grounding** | AI đề xuất các thuốc chống chỉ định nguy hiểm (như Bevacizumab cho bệnh nhân đang xuất huyết). Nếu bác sĩ áp dụng theo, bệnh nhân có thể tử vong do xuất huyết nội tạng nặng. | Injury | **Critical** | **Medium** | **Medium** | **Medium** | Thuốc đề xuất có cảnh báo hộp đen FDA. Việc AI bỏ qua chống chỉ định lâm sàng cơ bản đe dọa trực tiếp đến tính mạng bệnh nhân. |
| Bác sĩ huấn luyện hệ thống bằng cách nhập các ca bệnh giả định chủ quan thay vì nạp bệnh án thực tế. | Bác sĩ điều trị, Bệnh nhân | **Bias / fairness** | **Grounding** | Hệ thống đề xuất phác đồ mang tính thiên vị cục bộ của bệnh viện MSK, không phù hợp với điều kiện kinh tế, thiết bị và cơ địa bệnh nhân ở các quốc gia khác, gây lãng phí tiền bạc và mất thời cơ vàng điều trị đúng cách. | Opportunity loss, Dignity loss | **High** | **High** | **High** | **High** | Việc bán một hệ thống AI chưa chín muồi và thiên lệch ra toàn cầu khiến hàng nghìn bệnh nhân chịu phác đồ kém tối ưu và tốn kém vô ích. |
