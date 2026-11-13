# Vườn Mây Diệu Kỳ

Game trồng hoa trên tầng mây, chạy trực tiếp trên trình duyệt (HTML + JavaScript, không cần cài đặt).

## Tính năng
- Tầng mây xếp chồng (tối đa 6 tầng, 54 chậu), dây đậu thần, mở tầng theo cấp độ
- 14 loại hoa (11 hoa thường + 3 hoa Giáng Sinh), mỗi loại 3 giai đoạn: mầm → nụ → nở
- 15 chậu: đường nâng cấp Đất Nung → Ốc Vàng, 3 chậu nhiệm vụ ngày, 4 chậu Noel
- Hái trộm vườn hàng xóm (có chó canh), bắt bọ, nhiệm vụ hằng ngày
- Sự kiện Giáng Sinh: Kẹo Gậy, mốc quà tích lũy, cửa hàng đổi chậu, giao diện tuyết
- Hiệu ứng lấp lánh: vàng bay về ô tiền, vệt sáng trên chậu cao cấp, hào quang, pháo giấy

## Chạy thử
Mở `index.html` bằng trình duyệt, hoặc chạy một web server tĩnh:

```bash
python3 -m http.server 8000
# mở http://localhost:8000
```

Tiến trình chơi được lưu trong `localStorage` của trình duyệt.

## Cấu trúc
- `index.html` — toàn bộ code game
- `assets/` — hình WebP đã tách nền, dùng trong game
- `src/` — 10 bảng hình gốc (nền xanh) tạo bằng AI, dùng để cắt ra `assets/`
