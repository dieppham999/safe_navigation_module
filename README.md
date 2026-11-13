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

## Giải thích và bảo vệ mã nguồn

### 1. Tại sao sử dụng `<ul>` thay vì `<ol>` để xây dựng Navigation Menu?

Trong HTML, `<ul>` và `<ol>` đều được sử dụng để tạo danh sách nhưng có ý nghĩa ngữ nghĩa khác nhau:

| Tiêu chí | `<ul>` | `<ol>` |
|---|---|---|
| Tên đầy đủ | Unordered List | Ordered List |
| Ý nghĩa | Danh sách không có thứ tự bắt buộc | Danh sách có thứ tự mang ý nghĩa |
| Hiển thị mặc định | Dấu đầu dòng | Số hoặc ký tự thứ tự |
| Trường hợp sử dụng | Menu điều hướng, danh mục sản phẩm | Các bước hướng dẫn, bảng xếp hạng |

**Lý do lựa chọn `<ul>`:**

- Các mục menu như Trang chủ, Sản phẩm, Dịch vụ, Giới thiệu và Liên hệ không cần tuân theo trình tự bắt buộc.
- Sử dụng `<ul>` kết hợp `<li>` giúp thể hiện đúng ngữ nghĩa HTML.
- Công nghệ hỗ trợ như Screen Reader có thể nhận diện cấu trúc danh sách và số lượng phần tử, tùy theo trình duyệt và công nghệ hỗ trợ.
- Thẻ `<nav>` giúp xác định khu vực điều hướng của trang web.

**Kết luận:** Sử dụng cấu trúc `<nav>` → `<ul>` → `<li>` → `<a>` là lựa chọn phù hợp cho menu điều hướng của dự án.

### 2. Điều gì xảy ra nếu checkout sang `main` khi chưa commit thay đổi trên `feature/nav-menu`?

Khi đang làm việc trên nhánh `feature/nav-menu`, nếu chỉnh sửa file nhưng chưa commit mà chuyển sang nhánh `main`, Git có thể xử lý theo hai trường hợp:

**Trường hợp 1: Không xảy ra xung đột**

- Git cho phép chuyển sang nhánh `main`.
- Các thay đổi chưa commit được giữ lại trong Working Directory.
- Những thay đổi này có thể xuất hiện khi đang ở nhánh `main`, dẫn đến nguy cơ commit nhầm nhánh.

**Trường hợp 2: Có nguy cơ ghi đè thay đổi**

- Git từ chối chuyển nhánh.
- Terminal có thể hiển thị thông báo `Your local changes to the following files would be overwritten by checkout`.
- Git yêu cầu xử lý các thay đổi trước khi chuyển nhánh để tránh mất dữ liệu.

**Giải pháp an toàn:**

- `git status`: Kiểm tra trạng thái Working Directory.
- `git add` và `git commit`: Lưu những thay đổi đã hoàn thành.
- `git stash`: Tạm cất các thay đổi chưa muốn commit.
- `git switch main`: Chuyển về nhánh chính sau khi đảm bảo trạng thái phù hợp.

**Kết luận:** Trước khi chuyển nhánh, cần kiểm tra trạng thái Git và chủ động commit hoặc stash thay đổi để tránh xung đột, mất dữ liệu hoặc commit nhầm nhánh.

### 3. Tại sao cần phát triển tính năng trên nhánh riêng thay vì trực tiếp trên `main`?

- **Bảo vệ mã nguồn:** Hạn chế ảnh hưởng đến phiên bản đang hoạt động ổn định.
- **Phát triển độc lập:** Cho phép thử nghiệm và chỉnh sửa tính năng mà không trực tiếp thay đổi `main`.
- **Code Review:** Dễ dàng kiểm tra các thay đổi trước khi hợp nhất.
- **Quản lý lịch sử:** Theo dõi các commit và quá trình phát triển từng tính năng.
- **Hỗ trợ làm việc nhóm:** Nhiều lập trình viên có thể phát triển các tính năng trên các nhánh riêng biệt.

**Kết luận:** Git Branching là một phương pháp quản lý mã nguồn quan trọng, giúp quy trình phát triển phần mềm an toàn, dễ kiểm soát và chuyên nghiệp hơn.