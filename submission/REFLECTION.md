# Reflection

Một anti-pattern dễ gặp trong Lakehouse là dùng bảng dữ liệu thô trực tiếp
cho dashboard và truy vấn phân tích. Cách này khiến mỗi truy vấn phải tự
parse JSON, deduplicate và tính lại các metric, làm tăng chi phí đọc và
khiến kết quả khó nhất quán.

Pipeline Bronze–Silver–Gold giải quyết vấn đề này bằng cách giữ dữ liệu thô
ở Bronze, chuẩn hóa và deduplicate ở Silver, rồi tổng hợp metric phục vụ
dashboard ở Gold. Nhờ vậy dashboard đọc dữ liệu nhỏ hơn và có schema ổn
định hơn.

Trong lab, tôi dùng AI để hỗ trợ việc đọc hiểu các code và tóm tắt lại các yêu 
cầu đề bài cho. Tôi tự chạy notebook, kiểm tra kết quả thực tế và chịu trách nhiệm 
với các output đã nộp.