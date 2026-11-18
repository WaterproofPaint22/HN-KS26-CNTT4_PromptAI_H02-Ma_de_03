# BÀI LÀM PHA 2 – HACKATHON 02

- **Mã đề:** 03
- **Họ tên:**
- **Lớp:**
- **Link repository Pha2:**
- **Công cụ AI đã dùng (ChatGPT/Claude/Gemini):**

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

## 4.2. Trích xuất tin nhắn đăng ký khoá học ra JSON

**KET QUA AI**

```text
[
  {
    "ma_khoa": "NP12",
    "ngay_khai_giang": "2026-12-08",
    "hoc_vien_lon": 2,
    "hoc_vien_nho": 1,
    "hinh_thuc": "offline",
    "ghi_chu": null
  },
  {
    "ma_khoa": "IE55",
    "ngay_khai_giang": "2027-01-06",
    "hoc_vien_lon": 3,
    "hoc_vien_nho": 0,
    "hinh_thuc": null,
    "ghi_chu": "một bạn bị khiếm thính nhẹ"
  },
  {
    "ma_khoa": "GT01",
    "ngay_khai_giang": null,
    "hoc_vien_lon": 4,
    "hoc_vien_nho": 0,
    "hinh_thuc": "offline",
    "ghi_chu": "một bạn đi nạng"
  }
]
```

**Link trò chuyện:** https://share.gemini.google/HcLwzN6zj4AN

## 4.3. Báo giá bằng Chain-of-Thought

**KET QUA AI**

```text
**1. Tiền học viên lớn**

* Khóa NP12 có học phí gốc là 2.400.000 đồng/học viên.
* Phép tính: $4 \times 2.400.000 = 9.600.000$ đồng.

**2. Tiền học viên nhỏ tuổi**

* 2 học viên nhỏ tuổi (11 tuổi và 14 tuổi, thuộc nhóm từ 10 đến 15 tuổi) tính 60% học phí học viên lớn: $2.400.000 \times 60\% = 1.440.000$ đồng/học viên.
* 1 bé 8 tuổi (dưới 10 tuổi) học dự thính cùng phụ huynh được miễn phí ($0$ đồng).
* Phép tính: $2 \times 1.440.000 + 0 = 2.880.000$ đồng.

**3. Tiền học phí**

* Tổng tiền học phí của học viên lớn và học viên nhỏ tuổi:
* Phép tính: $9.600.000 + 2.880.000 = 12.480.000$ đồng.

**4. Giảm giá nhóm**

* Nhóm có 4 học viên lớn (đạt điều kiện từ 4 học viên lớn trở lên) nên được giảm 10% trên tiền học phí:
* Phép tính giảm giá: $12.480.000 \times 10\% = 1.248.000$ đồng.
* Tiền học phí sau giảm: $12.480.000 - 1.248.000 = 11.232.000$ đồng.

**5. Phí giáo trình**

* Nhóm mua 3 bộ giáo trình bản in với đơn giá 250.000 đồng/bộ (không áp dụng giảm giá):
* Phép tính: $3 \times 250.000 = 750.000$ đồng.

**6. Tổng tiền**

* Tổng tiền thanh toán = tiền học phí sau giảm + phí giáo trình:
* Phép tính: $11.232.000 + 750.000 = 11.982.000$ đồng.

[RESULT: 11.982.000 đồng]
```

**Link trò chuyện:** https://share.gemini.google/DDNuoNhxqc2U

### b) Kiểm tra kết quả AI

Kết quả của AI đúng.

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```text
(Dán câu trả lời của AI vào đây (bấm nút Copy dưới câu trả lời) – xoá dòng này)
```

**Link trò chuyện:**

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

```text
Tiêu chí	Điểm	Minh chứng	Đề xuất sửa
Đúng thông tin (50%)	0 / 5	Lỗi 1 — Câu bị lỗi: "IELTS 5.5 bên em 6.900.000đ thôi chị, học xong là chắc đậu luôn ạ." — Lý do sai: Báo sai mức học phí chuẩn của công ty (7.500.000 đồng/học viên lớn) và tự ý đưa ra cam kết đậu đầu ra không có trong thông tin chuẩn. Lỗi 2 — Câu bị lỗi: "Chị học 6 buổi rồi rút thì vẫn được hoàn một nửa nha chị." — Lý do sai: Tư vấn sai chính sách hoàn học phí (theo quy định, hoàn 50% chỉ áp dụng khi rút sau buổi 1 đến hết buổi 5; từ buổi 6 trở đi không hoàn học phí).	Sửa lỗi 1: "Hiện tại học phí khoá IELTS 5.5 dành cho học viên lớn bên em là 7.500.000 đồng ạ." Sửa lỗi 2: "Về chính sách hoàn học phí, bên em hoàn 100% nếu chị rút trước buổi học đầu tiên và hoàn 50% nếu rút sau buổi 1 đến hết buổi 5; trường hợp chị đã học 6 buổi thì sẽ không được hoàn học phí ạ."
Đầy đủ (30%)	1 / 3	Lỗi thiếu ý — Câu bị lỗi: "Có gì chị nhắn em nhé!" — Lý do sai: Nhân viên đã trả lời đủ cả 2 câu hỏi của khách hàng (đạt 1 điểm), nhưng bỏ sót hoàn toàn 2 yêu cầu bắt buộc ở phần kết là mời khách cho biết hình thức học (online/offline) và ngày muốn khai giảng.	Sửa phần kết thúc: "Để em tư vấn lộ trình và xếp lớp phù hợp nhất, chị cho em biết mình muốn học theo hình thức online hay offline và dự kiến khai giảng vào ngày nào nhé ạ!"
Giọng điệu (20%)	1 / 2	Lỗi 1 — Câu bị lỗi: "Chị học 6 buổi rồi rút thì vẫn được hoàn một nửa nha chị." — Lý do sai: Dùng từ ngữ suồng sã ("nha chị"), thiếu sự trang trọng cần thiết khi tư vấn. Lỗi 2 — Câu bị lỗi: "Có gì chị nhắn em nhé!" — Lý do sai: Cách kết thúc câu quá suồng sã, thiếu chuyên nghiệp trong giao tiếp với khách hàng.	Sửa lỗi 1: Thay cụm "nha chị" bằng "ạ" để câu trang trọng hơn ("...thì sẽ không được hoàn học phí ạ."). Sửa lỗi 2: Thay bằng lời mời hỗ trợ lịch sự, chuyên nghiệp: "Nếu cần thêm thông tin chi tiết, chị cứ phản hồi để em hỗ trợ ngay cho mình ạ."
Tổng điểm	2 / 10	Sai toàn bộ thông tin trọng yếu (học phí, chính sách hoàn tiền), thiếu câu hỏi khai thác nhu cầu và còn dùng từ ngữ suồng sã.	Rà soát kỹ thông tin sản phẩm và chính sách hoàn phí, bổ sung đủ câu hỏi về hình thức học (online/offline) cùng ngày khai giảng, đồng thời điều chỉnh văn phong chuẩn mực hơn.
```

**Link trò chuyện:** https://share.gemini.google/TEtD3A1AUwdr
