# 📊 BÁO CÁO THU HOẠCH NGHIỆM THU BÀI LAB 3 (BƯỚC 3 — SUBMISSION ARTIFACT)

> **Họ và Tên Học viên:** Nguyễn Thành Tiến 
> **Mã Sinh Viên / Mã Học viên:** 2A202603003
> **Chủ đề Lựa chọn:** Trợ lý Học vụ & Tra cứu Lịch thi VinUni:\* Tra cứu điểm GPA, lịch thi và đặt lịch tư vấn học vụ với Cố vấn.

---

## 1. BẢNG CHẤM ĐIỂM AGENTIC FIT SCORING MATRIX (ĐÁNH GIÁ CHỦ ĐỀ)

| Tiêu chí Đánh giá           | Mức độ (1 - 5) | Giải trình chi tiết lý do chọn điểm                                      |
| :-------------------------- | :------------: | :----------------------------------------------------------------------- |
| **1. Multi-step Reasoning** |      4/ 5      | Bài toán có yêu cầu chia nhỏ nhiều bước suy luận nối tiếp nhau không?    |
| **2. Tool Interaction**     |      5/ 5      | Hệ thống có cần kết nối với MCP Server / Cơ sở dữ liệu bên ngoài không?  |
| **3. Dynamic Decision**     |      4/ 5      | Bước tiếp theo có phụ thuộc vào kết quả quan sát bước trước không?       |
| **4. Long Horizon Goal**    |      4/ 5      | Hệ thống có phải giữ mục tiêu xuyên suốt qua nhiều lượt xử lý không?     |
| **TỔNG ĐIỂM AGENTIC FIT**   |   **17/ 20**   | _Nếu tổng điểm > 12/20: Bài toán rất phù hợp triển khai Agentic System._ |

---

## 2. TRÍCH XUẤT KẾT QUẢ WATERFALL TRACE LOG (SAU KHI CHẠY TEST SUITE TRÊN API THẬT)

> ⚠️ **YÊU CẦU NGHIỆM THU:** Mở tệp `.env` điền `GEMINI_API_KEY` (hoặc `OPENAI_API_KEY`) để kết nối LLM thật trước khi thực thi `python src/app.py --all`. Bài nộp chỉ dùng Mock Offline Provider sẽ không đạt điểm nghiệm thực tế.

Dán 1 đoạn trích xuất log tiêu biểu từ file `docs/trace_waterfall.json` sinh ra từ phản hồi LLM API thật:

```json
[
  {
    "step": 1,
    "query": "Trường đại học Vinuni thành lập năm bao nhiêu",
    "action_type": "FINAL_ANSWER",
    "thought": "Gemini phản hồi trực tiếp bằng văn bản (không cần gọi công cụ).",
    "output": "Trường Đại học VinUni (VinUniversity) được chính thức phê duyệt thành lập theo Quyết định số 1829/QĐ-TTg của Thủ tướng Chính phủ vào **ngày 17 tháng 12 năm 2019** và chính thức khai giảng khóa đầu tiên vào **năm 2020** (ngày 17/10/2020).",
    "latency_ms": 3363.51
  }
]
```

---

## 3. TỔNG KẾT KẾT QUẢ NGHIỆM THU & NỘP BÀI

- [ ] Đã điền API Key thật trong `.env` và xác nhận Agent chạy mượt mà trên LLM API thật (Gemini/OpenAI).
- **Tổng số Test Cases đã chạy thành công:** 5/ 5 test cases.
- **Số lượt gọi Tool qua MCP Server chính xác:** 5 lượt.
- **Kết quả đẩy Repo nộp bài:** [x] Đã Commit và Push mã nguồn thành công lên GitHub cá nhân.

---

> ✅ **HOÀN TẤT NỘP BÀI:** https://github.com/thanhtienpro123/K4B-DAY03-Nguyen_Thanh_Tien-2A202603003
