# BÀI LÀM PHA 2 – HACKATHON 02

- **Mã đề:** 06
- **Họ tên:*Hồ Gia Bảo*
- **Lớp:*K26-HCM-CNTT1*
- **Link repository Pha2:**
- **Công cụ AI đã dùng (ChatGPT/Claude/Gemini):** ChatGPT

> Pha 2 (20 phút cuối). Mỗi mục: mở cuộc trò chuyện mới, gửi nguyên văn prompt đã viết trong bai_lam_pha1.md, dán câu trả lời và link chia sẻ vào đây. Xong, kéo thả file này vào repository Pha2.

## 4.2. Trích xuất tin nhắn đặt bàn ra JSON

**KET QUA AI**

```text
[
  {
    "ma_buffet": "NUONG",
    "ngay_dat": "2026-12-19",
    "nguoi_lon": 2,
    "tre_em": 1,
    "khu_vuc": "trong_nha",
    "ghi_chu": null
  },
  {
    "ma_buffet": "HAISAN",
    "ngay_dat": "2027-01-03",
    "nguoi_lon": 3,
    "tre_em": 0,
    "khu_vuc": null,
    "ghi_chu": "1 người dị ứng sữa"
  },
  {
    "ma_buffet": "LAU",
    "ngay_dat": "2026-12-25",
    "nguoi_lon": 4,
    "tre_em": 0,
    "khu_vuc": "san_vuon",
    "ghi_chu": "ông ngoại đi xe lăn"
  }
]
```

**Link trò chuyện:**

## 4.3. Báo giá bằng Chain-of-Thought

**KET QUA AI**

```text
Tiền buffet người lớn:
10 người lớn x 399.000 đồng = 3.990.000 đồng.

Tiền trẻ em:
- 3 trẻ em cao từ 1 m đến 1,4 m, mỗi trẻ: 399.000 x 50% = 199.500 đồng.
- Tổng trẻ em: 3 x 199.500 = 598.500 đồng.
- 1 bé cao 0,8 m miễn phí.

Tổng tiền buffet trước giảm:
3.990.000 + 598.500 = 4.588.500 đồng.

Mức giảm do có 10 người lớn:
4.588.500 x 5% = 229.425 đồng.

Tiền buffet sau giảm:
4.588.500 - 229.425 = 4.359.075 đồng.

Phụ thu phòng riêng:
500.000 đồng.

Tổng tiền = 4.359.075 + 500.000 = 4.859.075 đồng.

Tổng tiền cần thanh toán: 4.859.075 đồng.
```

**Link trò chuyện:**

### b) Kiểm tra kết quả AI

Kết luận: AI đúng.

Các bước tính đều chính xác:
- Người lớn: 10 x 399.000 = 3.990.000 đồng.
- 3 trẻ em: 3 x (399.000 x 50%) = 598.500 đồng.
- Bé 0,8 m: miễn phí.
- Tổng trước giảm: 4.588.500 đồng.
- Giảm 5%: 229.425 đồng.
- Sau giảm: 4.359.075 đồng.
- Cộng phòng riêng: 500.000 đồng.
- Tổng đúng: 4.859.075 đồng.

## 4.4. Dây chuyền xử lý khiếu nại – kết quả Trạm 1

**KET QUA AI**

```text
{"loai_su_co":"thieu_mon","so_khach":5,"so_mon_bi_thieu":2,"tom_tat":"Tôm hùm và cua hết; gia đình chờ hai lần bổ sung không có"}
```

**Link trò chuyện:**

## 4.5. Prompt chấm bài theo Rubric

**KET QUA AI**

```text
Đúng thông tin: 0/5
Giải thích: Giá buffet lẩu sai (279.000 đồng thay vì 299.000 đồng) và quy định giữ bàn sai; với trễ 40 phút, nhà hàng huỷ bàn chứ không giữ bàn.

Đầy đủ: 1/3
Giải thích: Bài có đề cập hai câu hỏi của khách, nhưng không mời khách cung cấp ngày, giờ đến và số khách để đặt bàn.

Giọng điệu: 1/2
Giải thích: Câu trả lời thân thiện nhưng chưa chuyên nghiệp do dùng giọng suồng sã, cụ thể là “ngon bá cháy” và cách xưng hô “chị/em”.

Tổng: 2/10

Nhận xét: Bài sai thông tin quan trọng về giá và quy định giữ bàn. Bài chưa mời khách cung cấp đầy đủ thông tin đặt bàn và giọng điệu chưa phù hợp với tư vấn chuyên nghiệp.
```

**Link trò chuyện:**
