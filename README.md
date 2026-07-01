# VinAI-Lab Day 24: AI Safety, Risk Mapping & Case Studies Analysis

Dự án này chứa các tài liệu phân tích, đánh giá mức độ rủi ro (Risk Profile) và xây dựng bản đồ tác hại (Harm Map) cho các ứng dụng trí tuệ nhân tạo (AI) trong thực tế. Trọng tâm của bài Lab 24 tập trung vào việc nghiên cứu các case study thất bại điển hình trong lĩnh vực y tế (Healthcare) và so sánh bức tranh rủi ro giữa 6 ngành công nghiệp khác nhau.

---

## 📂 Cấu Trúc Thư Mục & Tài Liệu

Thư mục bao gồm các file tài liệu Markdown chi tiết phục vụ cho việc phân tích và so sánh:

*   [day24-track1-lab.pdf](file:///d:/VinAI-Lab/Day%2024%20Lab/day24-track1-lab.pdf): Tài liệu hướng dẫn gốc và đề bài chi tiết của bài Lab.
*   [industry_risk_snapshot.md](file:///d:/VinAI-Lab/Day%2024%20Lab/industry_risk_snapshot.md): Đánh giá bức tranh rủi ro tổng quát của ngành **Y tế / Symptom Checker / Health Assistant** trước khi phân tích cụ thể.
*   [brief_case_1_epic_sepsis.md](file:///d:/VinAI-Lab/Day%2024%20Lab/brief_case_1_epic_sepsis.md): Phân tích chi tiết về sự thất bại của hệ thống dự đoán nhiễm trùng huyết **Epic Sepsis Model (ESM)**.
*   [brief_case_2_ibm_watson.md](file:///d:/VinAI-Lab/Day%2024%20Lab/brief_case_2_ibm_watson.md): Phân tích các khuyến nghị điều trị ung thư không an toàn từ siêu máy tính **IBM Watson for Oncology**.
*   [brief_case_3_babylon_health.md](file:///d:/VinAI-Lab/Day%2024%20Lab/brief_case_3_babylon_health.md): Đánh giá tranh cãi về độ an toàn lâm sàng của ứng dụng phân loại triệu chứng **Babylon Health AI Triage**.
*   [group_comparison.md](file:///d:/VinAI-Lab/Day%2024%20Lab/group_comparison.md): Bảng đối chiếu và tổng hợp Risk Profile giữa 6 ngành công nghiệp chính (Tuyển dụng, Giáo dục, Y tế, Xe tự lái, Truyền thông và Sáng tạo nội dung).

---

## 🧠 Các Phương Pháp & Khái Niệm Cốt Lõi

### 1. Bản Đồ Tác Hại (Harm Map)
Mỗi case study đều được phân tích thông qua một **Harm Map Worksheet** nhằm mổ xẻ rủi ro ở các khía cạnh:
*   **High-risk moment**: Thời điểm nhạy cảm, dễ xảy ra lỗi nhất trong luồng vận hành của AI.
*   **Failure mode**: Dạng lỗi của hệ thống (ví dụ: *Harmful advice*, *Over-reliance*, *Bias / fairness*, *Hallucination*).
*   **Layer bắt đầu lỗi**: Tầng phát sinh lỗi (Model, UX, Grounding, Safety).
*   **Harm & Harm Lens**: Tác hại cụ thể và phân loại tác hại đối với con người (*Injury*, *Opportunity loss*, *Dignity loss*, *Privacy loss*, *Misinformation*).
*   **Severity, Scale, Probability, Frequency**: Các chỉ số đánh giá độ nghiêm trọng, quy mô ảnh hưởng, xác suất và tần suất xảy ra lỗi.

### 2. Risk Profile Giữa Các Ngành Công Nghiệp
Bài Lab phân loại rủi ro của các hệ thống AI thành 3 nhóm chính:
*   **Nhóm Rủi ro Chí mạng (Critical Risk - Y tế, Xe tự lái)**: Can thiệp vật lý, ảnh hưởng trực tiếp đến tính mạng con người, hậu quả không thể đảo ngược, yêu cầu tiêu chuẩn bàn giao khắt khe và bắt buộc có *Human-in-the-loop*.
*   **Nhóm Rủi ro Hệ thống/Xã hội (High Risk - Tuyển dụng, Truyền thông)**: Gây thiên lệch, bất bình đẳng xã hội, lan truyền tin giả với quy mô ảnh hưởng (Scale) cực kỳ rộng lớn.
*   **Nhóm Rủi ro Nhận thức/Sáng tạo (Medium Risk - Giáo dục, Sáng tạo nội dung)**: Rủi ro liên quan đến vi phạm bản quyền hoặc ảo tưởng thông tin (Hallucination), dễ dàng kiểm duyệt và đảo ngược hậu quả bởi con người.

---

## 🛠️ Hướng Dẫn Thực Hành

1. **Đọc tài liệu định hướng**: Bắt đầu bằng việc đọc [day24-track1-lab.pdf](file:///d:/VinAI-Lab/Day%2024%20Lab/day24-track1-lab.pdf) và [industry_risk_snapshot.md](file:///d:/VinAI-Lab/Day%2024%20Lab/industry_risk_snapshot.md) để có cái nhìn tổng quan.
2. **Khảo sát Case Studies**: Xem chi tiết từng trường hợp cụ thể để hiểu cách áp dụng khung phân tích rủi ro vào các dự án AI thực tế.
3. **So sánh & Rút ra bài học**: Tham khảo [group_comparison.md](file:///d:/VinAI-Lab/Day%2024%20Lab/group_comparison.md) để nắm được bức tranh toàn cảnh về thiết kế hệ thống AI an toàn và các rào cản kỹ thuật/quy trình cần thiết trước khi triển khai sản phẩm AI ra thị trường.
