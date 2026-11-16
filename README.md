# 🚀 Vitara Data Platform - Thư Mục Triển Khai Vercel (demovercel)

Thư mục này được cấu trúc độc lập và tối giản, **chỉ gồm các tệp cần thiết nhất** để đưa lên **Vercel** hoạt động ngay mà không gặp bất kỳ lỗi nào.

---

## 📂 Danh Sách Các Tệp Trong `demovercel/`

| Tệp tin | Vai trò |
| :--- | :--- |
| **`index.html`** | Ứng dụng web hoàn chỉnh: Màn hình Hero 3D, Quy trình 5 Bước, Chốt chặn phê duyệt Bước 2 (HITL Gate), Chẩn đoán SLA Bước 3, Mô phỏng Bước 4, Báo cáo P&L 12 dòng cân bằng & 5 biểu đồ Chart.js ở Bước 5, Trợ lý AI Copilot. |
| **`sample_data.csv`** | Tệp dữ liệu mẫu doanh nghiệp chuỗi bán lẻ (15.000 dòng đối soát đa kênh) phục vụ người dùng tải về dùng thử trực tiếp trên Vercel. |
| **`vercel.json`** | Tệp cấu hình định tuyến tĩnh và chuẩn hóa URL sạch cho Vercel. |
| **`package.json`** | Khai báo metadata và script kiểm tra cấu trúc cho Vercel. |
| **`.gitignore`** | Loại bỏ các tệp rác hệ thống phát sinh ngoài ý muốn. |

---

## ⚡ Hướng Dẫn Đẩy Lên Vercel (Chọn 1 Trong 2 Cách)

### Cách 1: Đẩy thư mục này lên GitHub rồi Import vào Vercel (Khuyên dùng - 1 phút)
1. Mở terminal tại thư mục này:
   ```bash
   cd demovercel
   git init
   git branch -M main
   git add .
   git commit -m "feat: deploy Vitara platform to Vercel"
   git remote add origin https://github.com/<tai-khoan-github-cua-ban>/<ten-repo>.git
   git push -u origin main
   ```
2. Truy cập **[vercel.com/new](https://vercel.com/new)**:
   * Chọn repository vừa đẩy.
   * Bấm **Deploy**.
   * Sau 10 giây, Vercel cấp đường link trực tuyến công khai.

---

### Cách 2: Triển khai bằng Vercel CLI (Nếu máy có cài Vercel)
Chỉ cần chạy lệnh:
```bash
cd demovercel
npx vercel --prod
```
Làm theo hướng dẫn trên màn hình, hệ thống sẽ tải lên và cung cấp link `https://...vercel.app` ngay lập tức!
