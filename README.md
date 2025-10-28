# form-leadmagnet-content-html-css-js-

Kho lưu trữ này chứa các mẫu form và banner làm bằng HTML, CSS và JavaScript cùng với các bài viết (content) được viết theo dạng có thể nhúng/nhập vào trang khác và vẫn hoạt động bình thường.

## Mục đích

Repository dùng để lưu trữ các mẫu (templates) lead magnet, form thu thập email, banner quảng bá, và bài viết kèm mã HTML/CSS/JS để bạn có thể copy — paste hoặc chèn (embed) trực tiếp vào website mà không làm mất chức năng.

## Nội dung chính

- `forms/` — mẫu form (HTML + CSS + JS) để thu thập thông tin/lead.
- `banners/` — mẫu banner/cta (call-to-action) có thể nhúng.
- `articles/` — các bài viết có mã nội tuyến hoặc hướng dẫn chèn.
- `assets/` — ảnh, font, script chung nếu có.

> Lưu ý: Mỗi mẫu nên là một file HTML độc lập (hoặc một thư mục với `index.html`), kèm theo CSS/JS cần thiết để khi mở trực tiếp bằng trình duyệt hoặc chèn vào trang khác vẫn hoạt động.

## Hướng dẫn xem trước (Preview)

- Mở trực tiếp file HTML trong trình duyệt: nhấp đúp vào file `index.html` hoặc `form-example.html`.
- Hoặc dùng extension Live Server (VS Code) để xem và test tương tác JS nhanh.

## Hướng dẫn nhúng vào trang khác

1. Nếu mẫu dùng CSS/JS riêng, copy toàn bộ phần `<style>` và `<script>` đi kèm vào trang đích, hoặc link đến file tĩnh trong `assets/`.
2. Nếu muốn nhúng dưới dạng iframe, upload file HTML và dùng `<iframe src="/path/to/template.html"></iframe>`.
3. Kiểm tra xung độtCSS: nếu chèn trực tiếp, cân nhắc bọc form/banner trong một class hoặc dùng tên lớp có tiền tố để tránh trùng tên.

Ví dụ đơn giản (nhúng trực tiếp):

```html
<!-- copy phần thân của file mẫu -->
<div class="lm-form-wrapper">
	<!-- HTML form ở đây -->
</div>
<style>
	/* CSS mẫu (copy) */
</style>
<script>
	// JS mẫu (copy)
</script>
```

## Quy ước cấu trúc đề xuất

- `forms/` — mỗi mẫu là một thư mục `forms/form-name/` chứa `index.html`, `styles.css`, `script.js` (hoặc một file HTML tự đủ).
- `banners/` — tương tự, mỗi banner là 1 file hoặc 1 thư mục.
- `articles/` — bài viết có thể đi kèm mã hoặc hướng dẫn chèn.

## Góp ý & Đóng góp

Nếu bạn muốn thêm mẫu mới hoặc sửa mẫu hiện có, hãy mở một Pull Request kèm mô tả ngắn: loại mẫu, cách preview, và cách nhúng.

## License

Mã nguồn trong repo này được đặt dưới [MIT License](LICENSE) (nếu bạn muốn license khác, hãy cập nhật file `LICENSE`).

## Liên hệ

Nếu cần hỗ trợ thêm cách nhúng hoặc muốn mẫu theo yêu cầu, mở Issue hoặc liên hệ qua thông tin trong profile.

---

_Gợi ý commit message:_ `docs: update README with repo purpose and embed/preview instructions`

