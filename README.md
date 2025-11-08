# QR Maker — Static (No DB) cho GitHub Pages

Website tạo mã QR **thuần static** (không DB, không backend), tối ưu mobile, có **nút In**. Hỗ trợ:
- URL/Text, Wi‑Fi, Email, SMS, vCard
- File (APK): dùng **URL có sẵn** hoặc **file cục bộ** (Object URL — *chỉ dùng trên máy bạn*).

## Cách đưa lên GitHub Pages
1. Tạo repo mới (public), ví dụ `qr-maker`.
2. Upload file `index.html` (thư mục này).
3. Vào **Settings → Pages → Build and deployment**:
   - Source: **Deploy from a branch**
   - Branch: `main` (hoặc `master`) / root (`/`)
4. Chờ build xong, site sẽ ở: `https://<username>.github.io/<repo>/`

> Nếu muốn custom domain: **Settings → Pages → Custom domain** (tạo bản ghi CNAME về `username.github.io`).

## Ghi chú
- Tính năng File cục bộ sử dụng **Object URL** → chỉ quét được trên thiết bị đang mở trang. Nếu cần chia sẻ cho mọi người, hãy tự upload file lên nơi công khai (GitHub Releases, Google Drive public, S3/R2, v.v.) rồi dùng **URL** đó để tạo QR.
- Khi in, dùng nút **In** trên trang để có layout gọn, QR ~80mm.
- Logo lớn ⇒ nên chọn ECC = **H** để đảm bảo máy quét tốt.
# QR-generate
