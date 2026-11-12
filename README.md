# Phát triển Module điều hướng an toàn

## 1. Giới thiệu

Bài thực hành thuộc chương trình đào tạo **CodeGym**, tập trung vào việc xây dựng Menu điều hướng (Navigation Menu) bằng HTML Semantic và quản lý mã nguồn an toàn với Git Branching.

**Bối cảnh:** Trang chủ của công ty đang hoạt động ổn định trên nhánh `main`. Yêu cầu bổ sung Menu điều hướng mà không ảnh hưởng đến phiên bản hiện tại. Tính năng phải được phát triển trên nhánh riêng, kiểm thử và hợp nhất vào `main` sau khi hoàn thành.

## 2. Mục tiêu

- Phân biệt thẻ `<ul>` và `<ol>` trong HTML.
- Sử dụng `<nav>`, `<ul>`, `<li>`, `<a>` để xây dựng Menu điều hướng đúng ngữ nghĩa.
- Hiểu lợi ích của việc phát triển tính năng trên Git Branch riêng.
- Thực hành tạo nhánh, chuyển nhánh, commit và merge bằng Git.
- Nhận diện và xử lý Merge Conflict khi có xung đột mã nguồn.

## 3. Yêu cầu thực hiện

### Bước 1: Xây dựng ý tưởng

- Xác định các mục Menu: Trang chủ, Sản phẩm, Dịch vụ, Giới thiệu, Liên hệ.
- Tìm hiểu lợi ích của việc sử dụng danh sách `<ul>/<li>` trong Menu.
- Xác định tên nhánh phát triển: `feature/nav-menu`.

### Bước 2: Thiết kế

- Phác thảo cấu trúc HTML theo mô hình `<nav>` → `<ul>` → `<li>` → `<a>`.
- Lập kế hoạch Git Workflow.
- Xác định các commit cần thực hiện.

### Bước 3: Triển khai

- Khởi tạo Git Repository và nhánh `main`.
- Tạo file `index.html` chứa mã nguồn trang chủ ban đầu.
- Commit phiên bản gốc trên `main`.
- Tạo nhánh `feature/nav-menu`.
- Phát triển Menu điều hướng bằng HTML Semantic.
- Commit tính năng trên nhánh riêng.

### Bước 4: Vận hành

- Chuyển về nhánh `main`.
- Merge nhánh `feature/nav-menu` vào `main`.
- Xử lý Merge Conflict nếu phát sinh.
- Kiểm tra mã HTML và lịch sử Git.
- Xóa nhánh tính năng sau khi merge thành công.

## 4. Yêu cầu kỹ thuật

**HTML:**
- Sử dụng đúng cấu trúc `<nav> > <ul> > <li> > <a>`.
- Đảm bảo cấu trúc HTML hợp lệ, đúng ngữ nghĩa.
- Không lạm dụng thẻ `<div>`.

**Git:**
- Có tối thiểu hai nhánh trong quá trình phát triển: `main` và `feature/nav-menu`.
- Tính năng mới phải có commit riêng.
- Lịch sử Git thể hiện quá trình tách nhánh và hợp nhất.
- Repository ở trạng thái sạch sau khi hoàn thành.

## 5. Tiêu chí đánh giá

| Tiêu chí | Tỷ trọng |
|---|---:|
| Cấu trúc HTML Semantic | 25% |
| Lịch sử Git Branching & Merging | 25% |
| Giải thích và bảo vệ mã nguồn | 30% |
| Nhật ký tương tác với AI | 20% |
| **Tổng cộng** | **100%** |

**Điểm thưởng:** Sử dụng AI tạo tình huống Merge Conflict giả định và tự thực hành xử lý.

## 6. Sản phẩm bàn giao

1. **GitHub Repository:** Chứa mã nguồn `index.html` với Menu điều hướng hoàn chỉnh.
2. **Git History:** Chứng minh quá trình tạo nhánh, commit và merge.
3. **Prompt_Log.pdf:** Nhật ký tương tác với AI trong quá trình thực hành.

## 7. Kết quả mong đợi

Hoàn thành Menu điều hướng đúng chuẩn HTML Semantic, đồng thời vận dụng quy trình Git Branching để phát triển và tích hợp tính năng mới mà không làm ảnh hưởng đến mã nguồn ổn định trên nhánh `main`.