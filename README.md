# Northstar Landing Page — tái cấu trúc CSS bằng Sass

Landing Page mẫu gồm navigation/header, sản phẩm nổi bật, số liệu thống kê và footer. Mã nguồn Sass được tổ chức theo partials và biên dịch thành `css/main.css`.

## Nền tảng tái sử dụng

Dự án dùng cấu trúc partial và các quy tắc Sass đã thực hành trong bài `sass-conversion`: biến màu nền/chữ, container co giãn, kiểu nút, box-shadow và CSS biên dịch. Các token đó được áp dụng cho một Landing Page mẫu hoàn chỉnh, vì các repository bài trước không chứa CSS/HTML Landing Page của bốn bài Template.

**Lưu ý:** đây là bản Landing Page dựng mới dựa trên kỹ thuật Sass đã học, không phải bản tái cấu trúc đã được đối chiếu pixel với thiết kế gốc của bài Template. Để xác nhận yêu cầu “giữ nguyên giao diện ban đầu”, cần có mã nguồn hoặc tài nguyên của Landing Page gốc.

## Cấu trúc

```text
landing-page-sass-refactor/
├── scss/
│   ├── abstracts/
│   ├── base/
│   ├── components/
│   ├── layout/
│   └── main.scss
├── css/
│   └── main.css
└── index.html
```

SCSS sử dụng variables cho màu/kích thước, mixins cho container/nút/breakpoint/shadow/focus, nesting cho các component và `@use` để nạp partial.

## Cài đặt và biên dịch

```powershell
npm install
npm run build
```

Theo dõi và tự biên dịch khi sửa SCSS:

```powershell
npm run watch
```

Mở `index.html` trong trình duyệt để xem trang.
