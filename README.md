# 🌐 AI-Trending-In-Other-Countries: Phân Tích Xu Hướng Phát Triển AI & Tác Động Toàn Cầu



Dự án nghiên cứu và trực quan hóa dữ liệu toàn diện về **sự bùng nổ của Trí tuệ Nhân tạo (AI)**, vị thế nghiên cứu giữa các quốc gia hàng đầu, sự tiến hóa của các mô hình học máy (AI Models), đánh giá hiệu năng (Benchmarks) và **tác động sâu sắc của AI đến thị trường việc làm toàn cầu hướng tới năm 2030**.

---

## 📌 Mục Lục
1. [Giới Thiệu Dự Án](#-giới-thiệu-dự-án)
2. [Cấu Trúc Thư Mục & Tệp Dữ Liệu](#-cấu-trúc-thư-mục--tệp-dữ-liệu)
3. [Mô Tả Chi Tiết Các Bộ Dữ Liệu](#-mô-tả-chi-tiết-các-bộ-dữ-liệu)
4. [Các Phát Hiện & Thông Điệp Chính (Key Insights)](#-các-phát-hiện--thông-điệp-chính-key-insights)
5. [Báo Cáo Trực Quan Hóa (Power BI & Presentation)](#-báo-cáo-trực-quan-hóa-power-bi--presentation)
6. [Hướng Dẫn Sử Dụng & Đóng Góp](#-hướng-dẫn-sử-dụng--đóng-góp)

---

## 📖 Giới Thiệu Dự Án

Trí tuệ nhân tạo (AI) đã chuyển mình mạnh mẽ trong thập kỷ qua nhờ vào ba trụ cột cốt lõi:
- **Dữ liệu lớn (Big Data):** Đóng vai trò là "nhiên liệu" chính yếu thúc đẩy các mô hình học sâu.
- **Hạ tầng tính toán & Phần cứng (GPU/TPU/Cloud Computing):** Cắt giảm chi phí và thời gian huấn luyện.
- **Đột phá thuật toán:** Sự ra đời của kiến trúc **Transformer**, nền tảng cho sự bùng nổ của các mô hình ngôn ngữ lớn (LLMs).

Dự án này tổng hợp, làm sạch và trực quan hóa các dữ liệu đa chiều nhằm trả lời các câu hỏi lớn:
1. *Cuộc đua AI diễn ra như thế nào giữa các cường quốc công nghệ (Mỹ, Trung Quốc, EU, Ấn Độ,...)?*
2. *Lĩnh vực AI nào đang chiếm tỉ trọng nghiên cứu và mô hình hóa cao nhất?*
3. *AI đang tái định hình cơ cấu việc làm ra sao và nhóm ngành nào chịu rủi ro tự động hóa cao nhất vào năm 2030?*

---

## 📂 Cấu Trúc Thư Mục & Tệp Dữ Liệu

```text
AI-Trending-In-Other-Countries/
│
├── AI_Impact_on_Jobs.xlsx                         # Bộ dữ liệu tác động của AI đến 3.000 mẫu việc làm (xác suất tự động hóa 2030)
├── cleaned_ai_models.csv                          # Dữ liệu 3.209 mô hình AI đã được chuẩn hóa (Domain, Task, Parameter,...)
├── benchmarks_runs.csv                            # Kết quả đánh giá hiệu năng/benchmarks thực tế của các mô hình AI tiên tiến
├── Các quốc gia hàng đầu về AI theo thời gian.xlsx # Chuỗi thời gian các công bố khoa học AI phân theo quốc gia/vùng lãnh thổ
├── Visualization.pbix                             # Báo cáo trực quan hóa Dashboard đa chiều trên Microsoft Power BI
├── trực quan hóa dữ liệu.pptx                     # Slide thuyết trình phân tích kết quả & tổng kết nghiên cứu
└── README.md                                      # Tài liệu tổng quan dự án
```

---

## 📊 Mô Tả Chi Tiết Các Bộ Dữ Liệu

### 1. `AI_Impact_on_Jobs.xlsx`
- **Quy mô:** 3.000 bản ghi, 18 trường thông tin.
- **Nội dung:** Khảo sát mức độ ảnh hưởng của AI tới các vị trí việc làm.
  - `Job_Title`: Vị trí công việc (Software Engineer, Security Guard, Retail Worker, Data Scientist,...).
  - `Average_Salary`, `Years_Experience`, `Education_Level`: Thông tin nhân khẩu học và thu nhập.
  - `AI_Exposure_Index`: Chỉ số mức độ tiếp xúc/ảnh hưởng của AI đối với công việc.
  - `Tech_Growth_Factor`: Hệ số tăng trưởng công nghệ tác động đến ngành.
  - `Automation_Probability_2030`: Xác suất công việc bị tự động hóa hoàn toàn vào năm 2030.
  - `Risk_Category`: Phân nhóm mức độ rủi ro (**Low** ~24.63%, **Medium** ~50.7%, **High** ~24.67%).
  - `Skill_1` đến `Skill_10`: Trọng số các kỹ năng chuyên môn liên quan.

### 2. `cleaned_ai_models.csv`
- **Quy mô:** 3.209 mô hình AI được thống kê chi tiết.
- **Nội dung:** Sự phát triển của các mô hình AI từ năm 2000 đến nay.
  - `Model`: Tên định danh mô hình.
  - `Publication date`: Ngày công bố mô hình.
  - `Organization`: Tổ chức phát triển (OpenAI, Google, Meta, Microsoft, DeepSeek, Anthropic,...).
  - `Domain`: Lĩnh vực chính (Language, Vision, Biology, Multimodal, Speech, Robotics,...).
  - `Task`: Tác vụ chuyên biệt (Language modeling, Text generation, Chat, Image generation,...).
  - `log_parameters`: Quy mô tham số mô hình (Logarithmic scale).

### 3. `benchmarks_runs.csv`
- **Quy mô:** 661 lượt thử nghiệm benchmark trên các nhiệm vụ tính toán chuyên sâu.
- **Nội dung:** Đo lường năng lực và điểm số của các mô hình hàng đầu (ví dụ: GPT-5, DeepSeek, Claude,...) trên các bộ bài toán khắt khe như FrontierMath, Coding, Lý luận logic.
  - `task`, `model`, `Best score (across scorers)`, `Scores`, `started_at`, `Status`, `task version`.

### 4. `Các quốc gia hàng đầu về AI theo thời gian.xlsx`
- **Quy mô:** 260 bản ghi chuỗi thời gian (giai đoạn 2000 - nay).
- **Nội dung:** Tổng số lượng công bố khoa học và nghiên cứu về AI phân theo quốc gia/vùng lãnh thổ:
  - Các quốc gia tiêu biểu: Trung Quốc (`CHN`), Hoa Kỳ (`USA`), Ấn Độ (`IND`), Nhật Bản (`JPN`), các nước EU,...
  - `impact_level`, `pub_type`, `publications`, `year`.

---

## 🔍 Các Phát Hiện & Thông Điệp Chính (Key Insights)

1. **Cuộc đua song mã giữa các siêu cường công nghệ:**
   - Trung Quốc (**CHN** ~33.42%) và Hoa Kỳ (**USA** ~23.8%) chiếm hơn một nửa tổng số ấn phẩm nghiên cứu AI toàn cầu, theo sau là Ấn Độ (**IND** ~10.5%) và Nhật Bản (**JPN** ~6.87%).
2. **Sự bùng nổ theo hàm mũ của các mô hình AI:**
   - Số lượng mô hình AI bắt đầu tăng vọt từ năm 2017 và đạt đỉnh điểm bùng nổ từ 2022 trở đi với sự trỗi dậy của Generative AI và LLMs.
   - **Language (Xử lý ngôn ngữ tự nhiên)** là lĩnh vực thống trị số lượng mô hình, tiếp theo là **Biology** (sinh học phân tử/protein folding) và **Vision** (thị giác máy tính).
3. **Tác động đến thị trường lao động (Automation 2030):**
   - **Nhóm nguy cơ cao (High Risk):** Các công việc có tính chất lặp đi lặp lại hoặc thủ công (Retail Worker, Construction Worker, Security Guard, Truck Driver,...).
   - **Nhóm nguy cơ thấp / Thích ứng cao (Low Risk):** Các công việc đòi hỏi tư duy trừu tượng, sáng tạo, giải quyết vấn đề phức tạp (Software Engineer, Research Scientist, Data Scientist,...).
   - **Xu hướng:** AI không chỉ thay thế cơ học một số vị trí mà còn kích thích sự ra đời của các nghề mới như *AI Engineer, ML Engineer, Prompt Engineer, AI Ethics Specialist*.

---

## 📈 Báo Cáo Trực Quan Hóa (Power BI & Presentation)

File báo cáo **`Visualization.pbix`** và slide **`trực quan hóa dữ liệu.pptx`** cung cấp 3 góc nhìn Dashboard tương tác chính:
- **Trang 1: Tổng quan xu hướng AI theo các quốc gia:** Trực quan hóa thị phần công bố nghiên cứu, tiến trình thời gian từ năm 2000 đến nay.
- **Trang 2: Xu hướng phát triển AI theo mô hình & lĩnh vực:** Phân bổ Domain, quy mô tham số (`log_parameters`) và dòng thời gian xuất hiện các mô hình đột phá.
- **Trang 3: Tác động của AI đến nghề nghiệp:** Phân bố xác suất tự động hóa 2030, mối liên hệ giữa kinh nghiệm, trình độ học vấn, thu nhập và mức độ rủi ro công việc.


---

## 🚀 Hướng Dẫn Sử Dụng

### Yêu cầu môi trường:
- **Xem Dashboard:** Cài đặt [Microsoft Power BI Desktop](https://powerbi.microsoft.com/desktop/) để mở tệp `Visualization.pbix`.
- **Xem Slide:** Sử dụng Microsoft PowerPoint hoặc Google Slides để xem `trực quan hóa dữ liệu.pptx`.
- **Phân tích dữ liệu (Python):**
  ```bash
  pip install pandas openpyxl matplotlib seaborn
  ```

---
*Dự án phục vụ mục đích nghiên cứu học thuật và tham khảo xu hướng công nghệ.*
