# AI Support Log — Phan Duy Thành (2A202602930)

## AI đã giúp tôi ở đâu?

- Đã tham vấn AI về việc lựa chọn Persona Freelance Designer, định nghĩa Core Action (Export Design Pack) thay cho nút Render, và xây dựng khung Metric NSM kèm Counter-metric.
- Claude Code dựng khung `metrics-pack.html` và điền nội dung từ các quyết định tôi đưa ra; AI đề xuất thêm quality threshold của NSM (sau đó tôi thay bằng tiêu chí Client-Readiness), 3 leading indicators (giữ lại "activation trong 48 giờ", bỏ 2 cái còn lại) và event `account_created`.
- AI phản biện bản nháp theo các gate (breadth trùng volume, threshold trùng completion rule, số liệu 20%/35% không có nguồn, hai leading indicator trùng nhau) và đồng bộ các chỉnh sửa cuối vào file.

## AI sai, hời hợt hoặc đề xuất metric sai nature ở đâu?
1. Nhầm giữa "Độ rộng" với "Số lượng" (Mục 03 - Engagement Breadth)

Bản cũ viết: "Số phòng xuất trong tháng".

Vì sao cấn: Cái này là đếm số lượng (Volume), trùng luôn với chỉ số chính (North Star). Độ rộng (Breadth) phải là xem khách có dùng nhiều ngóc ngách của app không.

Sửa lại cho chuẩn (bản cuối): Tỉ lệ designer xử lý từ 2 loại không gian khác nhau trở lên trong tháng. Phương án "dùng cả Dựng 3D và Moodboard" bị bỏ vì Design Pack đạt chuẩn luôn có đủ cả hai, nên chỉ số sẽ luôn 100%.

2. Bắt người ta làm thật nhanh là sai tâm lý (Mục 03 - Leading indicator 3)

Bản cũ viết: "Thời gian từ lúc up ảnh đến lúc xuất file càng ngắn càng tốt".

Vì sao cấn: Designer nghiêm túc họ phải ngồi săm soi, chỉnh cái đèn, đổi màu rèm 15–20 phút mới ưng. Bắt họ làm thật nhanh thì chỉ có mấy ông bấm nghịch cho vui mới làm thế.

Sửa lại cho chuẩn (bản cuối): Tỉ lệ dự án có ≥ 2 phòng được tạo trong tuần đầu sau khi kích hoạt. Phương án "AI trả preview dưới 30 giây" bị bỏ vì đó là độ trễ hệ thống, không phải hành vi của designer.

## Tôi đã tự sửa hoặc quyết định lại điều gì?
- **Mục 03 (Engagement Breadth):** Đổi từ "Số phòng/dự án xuất trong tháng" (bẫy Volume trùng NSM) thành "Tỉ lệ designer xử lý ≥ 2 loại không gian khác nhau trong tháng" (đo đúng độ rộng tương tác).
- **Mục 03 (Leading Indicator 3):** Đổi từ "Thời gian từ upload tới export ngắn" (sai lệch bản chất chăm chút của designer) thành "Tỉ lệ dự án có ≥ 2 phòng được tạo trong tuần đầu" (dự báo việc đưa app vào workflow căn hộ thật).
- **Mục 03 (NSM Quality Threshold):** Chuẩn hóa thành tiêu chí Client-Readiness (tối thiểu 2 góc phối cảnh + bảng vật liệu có định danh sơ bộ) thay vì ép buộc sửa tay hoặc chỉ nói "không lỗi".
- **Mục 05 (Metric Hypothesis):** Hoàn thành giả thuyết tác động của Loop lên M1 Retention Rate (tăng từ 20% lên >35%).