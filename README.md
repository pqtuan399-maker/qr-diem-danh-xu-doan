# XD04 — Điểm danh Xứ Đoàn (GitHub Pages + PWA)

## Cấu trúc

```text
qr-diem-danh-xu-doan/
├── index.html
├── config.js
├── manifest.webmanifest
├── service-worker.js
├── README.md
├── VERSION.txt
└── icons/
    ├── icon-1024.png
    ├── icon-512.png
    ├── icon-192.png
    ├── icon-maskable-512.png
    ├── apple-touch-icon.png
    └── favicon-32.png
```

## Bước bắt buộc

Mở `config.js` và thay:

```js
OFFICIAL_APP_URL: 'PASTE_J3_WEB_APP_URL_HERE',
```

bằng link chính thức tại `CẤU HÌNH!J3`.

Ví dụ:

```js
OFFICIAL_APP_URL: 'https://script.google.com/macros/s/AKfy.../exec?app=scan',
```

Không dùng link `/dev`.

## Đưa lên GitHub

1. Dùng repository hiện tại `qr-diem-danh-xu-doan`.
2. Upload toàn bộ nội dung gói này vào thư mục gốc repository.
3. Vào `Settings` → `Pages`.
4. Source: `Deploy from a branch`.
5. Branch: `main`.
6. Folder: `/ (root)`.
7. Save và chờ Pages cập nhật.

## Cách hoạt động

- Mở GitHub/PWA trực tiếp: chỉ hiện launcher, không mở camera.
- Bấm icon PWA: mở launcher → vào link J3 → Apps Script xác thực Gmail/quyền lớp.
- CODE 4 mở lại GitHub bằng `nonce + return`: chuyển sang camera.
- Camera đọc QR và gửi về CODE 4 để ghi `NHẬT KÝ DUYỆT`.

## Cài icon

### Android / Chrome
Mở URL GitHub Pages → menu ⋮ → `Thêm vào màn hình chính` hoặc `Cài đặt ứng dụng`.

### iPhone / Safari
Mở URL GitHub Pages → Share → `Thêm vào MH chính`.

## Bảo mật

GitHub Pages chỉ dùng camera và đọc QR. GitHub không có quyền đọc/ghi Google Sheets.
Xác thực Gmail, phân quyền, chống trùng và ghi điểm danh vẫn do Apps Script CODE 4 xử lý.
