# Quá trình khởi tạo kernel

Chương này bao gồm các bài viết mô tả một quá trình khởi tạo đầy đủ của kernel, từ bước đầu tiên sau khi kernel được giải nén cho tới khi process đầu tiên được kernel khởi chạy.

*Lưu ý* rằng ở đây sẽ không mô tả tất tần tật các chi tiết trong quá trình khởi tạo kernel. Chương này chỉ mô tả các bước trong phần code của kernel nói chung, không bao gồm các tác vụ như xử lý ngắt, ACPI và nhiều phần khác. Những phần không được mô tả ở đây sẽ được đề cập đến trong các chương khác.

* [Những bước đầu tiên sau khi giải nén kernel](linux-initialization-1.md) - Mô tả những bước đầu tiên trong kernel.
* [Xử lý ngắt và ngoại lệ trong thời gian đầu](linux-initialization-2.md) - Mô tả quá trình khởi tạo ngắt và xử lý page fault trong những thời điểm đầu tiên.
* [Bước chuẩn bị cuối cùng trước điểm khởi đầu kernel](linux-initialization-3.md) - Mô tả các bước chuẩn bị cuối cùng trước khi gọi hàm `start_kernel`.
* [Điểm khởi đầu (entry point) của kernel](linux-initialization-4.md) - Mô tả các bước đầu tiên trong kernel nói chung.
* [Tiếp tục khởi tạo các thành phần tùy thuộc kiến trúc](linux-initialization-5.md) - Mô tả việc khởi tạo các phần riêng đi theo từng kiến trúc.
* [Vẫn tiếp tục khởi tạo các thành phần tùy thuộc kiến trúc ...](linux-initialization-6.md) - Mô tả các bước tiếp theo trong việc khởi tạo các phần riêng đi theo từng kiến trúc.
* [(Tạm) kết thúc phần khởi tạo tùy thuộc kiến trúc](linux-initialization-7.md) - mô tả phần cuối của `setup_arch`.
* [Khởi tạo bộ lập lịch (scheduler)](linux-initialization-8.md) - Mô tả các quá trình chuẩn bị cho khởi tạo, cũng như quá trình khởi tạo bộ lập lịch.
* [Khởi tạo RCU](linux-initialization-9.md) - Mô tả việc khởi tạo [RCU](http://en.wikipedia.org/wiki/Read-copy-update).
* [Kết thúc quá trình khởi tạo](linux-initialization-10.md) - phần cuối cùng trong quá trình khởi tạo Linux kernel.
