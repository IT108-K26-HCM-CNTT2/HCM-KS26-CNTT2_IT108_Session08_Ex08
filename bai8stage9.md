

## PHẦN 1: ĐIỀN KHUYẾT VÀ GIẢI THÍCH CHI TIẾT

Dưới đây là các chỗ trống `____` trong đề bài và cú pháp Markdown chính xác được điền vào:

1. **Chỗ trống số 1 (`# ____  Ứng dụng...`)**
   - **Điền:** `SmartCampus` (Tên dự án)
   - **Giải thích:** Sau ký hiệu tiêu đề `<h1>` (`#`) và khoảng trắng, ta đặt tên chính thức của dự án đi kèm emoji.

2. **Chỗ trống số 2 và 3 (`____bash` và `____`)**
   - **Điền:** ` ``` ` (3 dấu backtick ở đầu để mở block và 3 dấu backtick ở cuối để đóng block).
   - **Giải thích:** Khối mã nguồn (Code Block) bắt buộc phải được bao quanh bởi 3 dấu backtick, kèm theo tên ngôn ngữ `bash` ở đầu để hệ thống hỗ trợ tô màu cú pháp (Syntax Highlighting).

3. **Chỗ trống số 4, 5, 6 (`____ [x]`, `____ [ ]`, `____ [x]`)**
   - **Điền:** `- ` (Dấu gạch ngang kết hợp một khoảng trắng).
   - **Giải thích:** Cấu trúc danh sách công việc (Task List) chuẩn trong Markdown bắt đầu bằng dấu `-`, tiếp theo là khoảng trắng rồi đến cặp ngoặc vuông `[x]` hoặc `[ ]`.

4. **Chỗ trống số 7, 8, 9 (`| ____ | ____ | ____ |`)**
   - **Điền:** `| :--- | :--- | :--- |` (hoặc `| --- | --- | --- |`).
   - **Giải thích:** Hàng phân cách giữa tiêu đề bảng và nội dung bảng trong Markdown bắt buộc phải có để trình biên dịch nhận diện cấu trúc Table.

---

## PHẦN 2: HOÀN THIỆN FILE `README.md`

Dưới đây là toàn bộ mã nguồn file `README.md` sau khi đã điền đầy đủ và chuẩn xác:

```markdown
# SmartCampus Ứng dụng Quản lý Lịch Học Cá nhân

Ứng dụng giúp sinh viên **lên kế hoạch học tập** hiệu quả.

## Hướng dẫn Cài đặt

```bash
git clone https://github.com/nhom5/lich-hoc-app
cd lich-hoc-app
```

## Tính năng đã hoàn thành

- [x] Đăng ký / Đăng nhập tài khoản
- [ ] Nhắc nhở lịch học qua email
- [x] Xuất lịch ra file PDF

## Bảng So sánh Công nghệ

| Công nghệ | Mục đích | Phiên bản |
| :--- | :--- | :--- |
| Python | Backend xử lý dữ liệu | 3.11 |
| Markdown | Viết tài liệu README | - |
```

---

## PHẦN 3: GIẢI ĐÁP BẪY DỮ LIỆU

* **Câu hỏi:** Nếu hàng phân cách bảng (dòng `| --- | --- | --- |`) bị xóa, bảng sẽ hiển thị như thế nào? Tại sao?
* **Trả lời:**
  1. **Hiện tượng hiển thị:** Trang web sẽ **không hiển thị dữ liệu dưới dạng bảng (table)** nữa. Thay vào đó, trình biên dịch (Markdown Parser) sẽ hiểu nhầm hàng tiêu đề và các hàng dữ liệu bên dưới chỉ là các dòng văn bản thông thường hoặc chuỗi ký tự chứa dấu gạch đứng (`|`).
  2. **Nguyên nhân:** Trình phân tích cú pháp của Markdown nhận diện và tạo khung bảng dựa vào sự tồn tại bắt buộc của hàng phân cách (`---`) nằm ngay bên dưới hàng tiêu đề. Khi thiếu dòng này, cấu trúc bảng bị hỏng hoàn toàn.