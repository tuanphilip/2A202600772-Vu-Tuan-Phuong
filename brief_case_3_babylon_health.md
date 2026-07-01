# Brief Case & Harm Map: Babylon Health AI Triage Safety Controversies

## 1. Brief Case Table

| Field | Bạn điền gì |
| :--- | :--- |
| **Tên case** | Babylon Health AI Triage Safety Controversies |
| **Ngành** | Y tế / symptom checker / health assistant |
| **Tổ chức / sản phẩm** | Babylon Health / GP at Hand (AI Chatbot & Symptom Checker) |
| **Use case AI** | Phân loại bệnh nhân (Triage) và kiểm tra triệu chứng tự động - Người dùng nhập triệu chứng, chatbot sẽ phân tích và gợi ý hướng xử lý (tự chăm sóc, đi khám phòng khám, hoặc gọi cấp cứu). |
| **Thời điểm** | Năm 2020 (Các nghiên cứu khoa học độc lập công bố và cơ quan quản lý y tế tại Anh tiến hành đánh giá độ an toàn). |
| **Case xảy ra chuyện gì?** | Mặc dù Babylon Health tuyên bố chatbot của họ có độ chính xác chẩn đoán tương đương với bác sĩ thực tế thông qua các bài thi lý thuyết, các bác sĩ lâm sàng và nghiên cứu độc lập đã phát hiện ra chatbot này thường xuyên phân loại sai các triệu chứng nguy kịch. Ví dụ điển hình là chatbot khuyên một bệnh nhân nam lớn tuổi có triệu chứng rõ rệt của nhồi máu cơ tim "chờ khám bác sĩ gia đình vào ngày hôm sau" thay vì chỉ định gọi cấp cứu 999 ngay lập tức, đe dọa trực tiếp tính mạng người dùng. |
| **Stakeholder bị ảnh hưởng** | Bệnh nhân tự kiểm tra triệu chứng tại nhà (chịu rủi ro tính mạng); Hệ thống y tế công cộng (như NHS tại Anh - bị quá tải hoặc định hướng sai phân luồng bệnh nhân). |
| **Số liệu chính** | - Nghiên cứu độc lập trên *BMJ Open* chỉ ra độ chính xác chẩn đoán chung của các app kiểm tra triệu chứng phổ biến (bao gồm Babylon) chỉ đạt **19% đến 37.9%**.<br>- Nghiên cứu lâm sàng năm 2025 về chấn thương chỉnh hình cho thấy bác sĩ chẩn đoán đúng **84.4%** số ca, trong khi chatbot kiểm tra triệu chứng chỉ đúng **35.8%**.<br>- Chatbot khuyên bệnh nhân đau ngực nghi nhồi máu cơ tim "chờ khám bác sĩ gia đình" thay vì đi cấp cứu.<br>- Công ty phá sản tại Mỹ và phải bán tháo tài sản vào năm 2023 do hoạt động kinh doanh sa sút và mất uy tín. |
| **Trích nguồn ngắn** | Nghiên cứu của BMJ Open (2020) và các cuộc điều tra an toàn lâm sàng của NHS cho thấy Babylon AI chatbot phân loại sai các ca tim mạch cấp cứu nguy hiểm và độ chính xác chẩn đoán tổng thể rất thấp. |
| **Nguồn 1** | BMJ Open. (2020). "Comparison of physician and artificial intelligence chatbot triage performance." [Link nguồn](https://bmjopen.bmj.com/content/10/11/e038626) |
| **Nguồn 2** | The BMJ. (2018). "Babylon’s GP at Hand: regulators investigate clinical safety after complaints." [Link nguồn](https://www.bmj.com/content/362/bmj.k3275) |
| **Ghi chú độ tin cậy** | **Primary Source** (Nghiên cứu khoa học bình duyệt độc lập) & **High-quality secondary source** (Tạp chí y học hàng đầu thế giới The BMJ). Các số liệu chính xác và được đồng thuận cao từ giới chuyên môn. |

---

## 2. Harm Map Worksheet

| High-risk moment | Stakeholder bị ảnh hưởng | Failure mode | Layer bắt đầu lỗi | Harm xảy ra là gì? | Harm lens | Severity | Scale | Probability | Frequency | Vì sao? |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| AI Chatbot nhận diện triệu chứng đau ngực/cánh tay trái và đưa ra gợi ý cấp độ chăm sóc (triage level). | Bệnh nhân / Người dùng | **Harmful advice** | **Model** | AI khuyên bệnh nhân chờ khám bác sĩ gia đình bình thường thay vì đi cấp cứu. Bệnh nhân trì hoãn điều trị dẫn tới hoại tử cơ tim diện rộng hoặc tử vong tại nhà. | Injury | **Critical** | **High** | **Medium** | **Medium** | Lỗi phân loại sai ca cấp cứu (Triage) có thể trả giá bằng tính mạng của bệnh nhân chỉ trong vài giờ trì hoãn điều trị vàng. |
| Ứng dụng quảng cáo quá mức về khả năng thay thế bác sĩ của AI Chatbot. | Bệnh nhân / Người dùng | **Over-reliance** | **UX** | Người dùng tin tưởng tuyệt đối vào app y tế, tự chẩn đoán và tự chữa ở nhà, chủ quan không đi khám trực tiếp khiến các bệnh lý mãn tính nghiêm trọng tiến triển âm thầm. | Opportunity loss, Misinformation | **High** | **High** | **High** | **High** | Tạo tâm lý an tâm giả tạo cho người bệnh, làm mất cơ hội phát hiện sớm các bệnh nguy hiểm như ung thư hay tim mạch giai đoạn đầu. |
