# Industry Risk Snapshot: Y tế / Symptom Checker / Health Assistant

Dưới đây là đánh giá mức độ rủi ro (Risk Profile) chi tiết cho ngành **Y tế / Symptom Checker / Health Assistant** trước khi tiến hành phân tích các case study cụ thể.

## Bảng Đánh Giá Rủi Ro Ngành (Industry Risk Snapshot)

| Câu hỏi | Mức độ rủi ro (Low / Medium / High / Critical) | Vì sao? |
| :--- | :--- | :--- |
| **Nếu AI sai, có thể gây hại thể chất không?** | **Critical** | AI đưa ra lời khuyên sai lệch, bỏ sót triệu chứng nghiêm trọng hoặc chẩn đoán nhầm có thể dẫn tới việc người bệnh trì hoãn điều trị, sử dụng sai thuốc, trực tiếp gây nguy hiểm đến tính mạng hoặc tổn thương thể chất nghiêm trọng. |
| **AI có ảnh hưởng đến quyết định hệ trọng không?** | **Critical** | Các quyết định trong y tế (chẩn đoán bệnh nguy hiểm, phác đồ điều trị ung thư, phân loại bệnh nhân cấp cứu) đều là quyết định sống còn. Sự sai lệch của AI ảnh hưởng trực tiếp đến quyết định lâm sàng của bác sĩ và bệnh nhân. |
| **Hệ thống có động tới dữ liệu nhạy cảm không?** | **High** | Hệ thống bắt buộc phải xử lý dữ liệu sức khỏe cá nhân (Protected Health Information - PHI), lịch sử bệnh án, triệu chứng thầm kín. Đây là nhóm dữ liệu nhạy cảm nhất và được bảo vệ nghiêm ngặt bởi luật pháp (như HIPAA, GDPR). |
| **Nếu sai, hậu quả có khó đảo ngược không?** | **Critical** | Nếu bệnh nhân tử vong hoặc gặp biến chứng nặng dẫn đến tàn tật do chẩn đoán chậm trễ hoặc điều trị sai từ gợi ý của AI, hậu quả này hoàn toàn không thể đảo ngược được. |
| **Nếu triển khai rộng, blast radius có lớn không?** | **High** | Khi một mô hình AI y tế được tích hợp vào hệ thống bệnh án điện tử (EHR) phổ biến hoặc ứng dụng di động triệu người dùng, một lỗi hệ thống hoặc thiên lệch (bias) có thể ảnh hưởng đồng loạt đến hàng chục nghìn bệnh nhân cùng lúc. |
| **Có cần human review hoặc escalation không?** | **High** | Bắt buộc phải có sự kiểm duyệt của bác sĩ (Human-in-the-loop) hoặc quy trình chuyển tuyến (escalation) rõ ràng đến cơ sở y tế khi triệu chứng vượt quá khả năng phân loại. Tuy nhiên, rủi ro Clinician Bias và Alert Fatigue (lờn cảnh báo) vẫn rất lớn. |
| **Risk profile tổng thể của ngành** | **Critical** | Ngành y tế là lĩnh vực có mức độ dung sai lỗi cực kỳ thấp. Kết hợp các yếu tố về tính mạng con người, dữ liệu nhạy cảm và tính chất khó đảo ngược của hậu quả, rủi ro tổng thể được xếp vào mức **Critical**. |
