## 6/1/2024: Buổi học 1: Tổng quan Data Science
### Giới thiệu data science

Là lĩnh vực liên ngành: toán, thống kê, khoa học máy tính, trí tuệ nhân tạo, machine learning 

Xử lý trên dữ liệu phức tạp và đa dạng: có cấu trúc, bán cấu trúc và phi cấu trúc

Dữ liệu xử lý là Big Data, dữ liệu lớn, phức tạp 

**3 nhóm kiến thức nền tảng**
+ mathematics (toán + thống kê)
+ domain expertise (hiểu được bối cảnh và nhu cầu cụ thể của ngành để khai thác dữ liệu)
+ computer science (thuật toán, kỹ thuật lập trình) -> giúp hiểu và thiết kế được hệ thống có khả năng lưu trữ, xử lý dữ liệu lớn, phát triển thuật toán

Dữ liệu càng nhiều thì mô hình thuật toán càng học tốt -> đưa ra những dự đoán chính xác hơn
**Các kỹ năng data science**
+ Kỹ năng lập trình và xử lý dữ liệu với Python
+ Trực quan hoá dữ liệu (Matplotlib, Seaborn, Tableau, PowerBI,...)
+ Toán - Thống kê và ứng dụng
+ Machine learning
+ Phân tích dữ liệu lớn (Scalable Big Data analysis) (Adobe, Spark, SQL. Oracle,..)
+ Kỹ năng giao tiếp với dữ liệu

### Khác biệt giữa data science và data analytics
1. Phân tích mô tả (Descriptive Analytics)

Hiểu dữ liệu trong quá khứ và hiện tại, phân tích những gì ĐÃ xảy ra. Vd: phân tích doanh thu, lượng truy cập web,..)

Chủ yếu sử dụng biểu đồ, tổng hợp dữ liệu tạo thành dashboard

2. Phân tích chuẩn đoán (Diagnostic Analytics)

Tìm hiểu nguyên nhân của hiện tượng cụ thể xảy ra. Vd: tìm hiểu nguyên nhân doanh số giảm trong quý

3. Phân tích dự đoán (Predictive Analytics)

Sử dụng mô hình thống kê, máy học từ dữ liệu hiện tại, quá khứ để đưa ra những dự đoán tương lai

4. Phân tích tiên lượng (Prescriptive Analytics)

Giúp đưa ra các chiến lược, khuyến nghị trong tương lai 

+ Data Analytics: tập trung hiểu, xử lý và diễn giải dữ liệu trong quá khứ và hiện tại
+ Data Science: xử lý dữ liệu phức tạp với quy mô lớn hơn, tập trung vô xây dựng mô hình để đưa ra quyết định dựa trên dữ liệu cho tương lai

### Quy trình thực hiện dự án data science
<img width="1094" alt="Ảnh chụp Màn hình 2024-01-07 lúc 00 59 03" src="https://github.com/berylhoang2501/Data-Manipulation-and-Visualization-with-Python/assets/152646327/0dc7a414-a8b2-4858-ad6f-7a1f3d35de45">

Business understanding: hiểu vấn đề, lựa ra hướng phân tích và tiếp cận -> Analytics approach -> Data requirements -> Data collection -> Data understanding -> Data preparation (chiếm rất nhiều tgian, nếu k xử lý dl tốt thì mô hình sẽ chạy không hiệu quả) 
### Python và các thư viện mở rộng 
### Thiết lập môi trường làm việc
### Ngôn ngữ Markdown 
- Chèn link: [nội dung mô tả](địa chỉ trang web)
- Chèn hình ảnh: ![chú thích](link)
- Block quotes: >
- Cú pháp danh sách: * nội dung
- Danh sách có số thứ tự: 1. nội dung
- Vẽ đường nằm ngang: ---
- Nhấn mạnh đoạn code: `nội dung`
- Nhấn mạnh nguyên đoạn code: dùng 3 dấu ``` để mở và đóng đoạn code
- [Tham khảo cú pháp markdown](https://www.markdownguide.org/cheat-sheet/),(https://www.markdowntutorial.com/lesson/1/)

## 6/1/2024: Buổi học 2: Thư viện Numpy
### Giới thiệu 
- Numpy (Numerical Python)
- Thư viện chuyên xử lý dữ liệu số
- Là nền tảng của nhiều thư viện khác: pandas (series-dựa trên cấu trúc mảng 1 chiều và data frame-dựa trên mảng nhiều chiều), SciPy, Scikit-learn, PyTorch

**So sánh list và numpy array**
- List: 

Cho phép lưu trữ nhiều kiểu dữ liệu khác nhau

Chiếm dung lượng bộ nhớ nhiều hơn hẳn Numpy

Tính toán sử dụng vòng lặp

- Numpy array:

Đồng bộ về cùng 1 kiểu dữ liệu

Tính toán trực tiếp

## 11/1/2024: Buổi học 3: Thư viện Numpy
### Mảng một chiều

Mảng một chiều là một cấu trúc dữ liệu trong lập trình máy tính được sử dụng để lưu trữ một tập hợp các phần tử có cùng kiểu dữ liệu. Mỗi phần tử trong mảng được xác định bằng một chỉ số (index) duy nhất. Mảng một chiều còn được gọi là vector.

Mảng một chiều thường dùng để đọc file txt 

1. Tạo mảng một chiều
- Cú pháp tạo mảng: numpy.array(object, dtype)

object là đối tượng dạng danh sách (list, tuple, array,..). 

dtype: kiểu dữ liệu của các phần tử trong mảng (sẽ theo ptu có kích thước lớn nhất)

Nếu không có tham số dtype thì sẽ theo kiểu dữ liệu lớn nhất của object.

2. Thuộc tính của mạng
- Đối tượng mảng có 2 thành phần : thuộc tính , phương thức(hàm)
- Truy xuất:

tenmang.thuoctinh

tenmang.phuongthuc()

- Một số thuộc tính khác:
<img width="927" alt="Ảnh chụp Màn hình 2024-01-13 lúc 00 16 19" src="https://github.com/berylhoang2501/Data-Manipulation-and-Visualization-with-Python/assets/152646327/644b4176-d99f-4491-9819-fd57689615e8">

- Note: sử dụng dtype khi muốn lấy kiểu dữ liệu khác với kiểu dữ liệu của object, nếu không cần thì khỏi truyền dtype
3. Tạo mảng bằng các hàm tiện ích
  <img width="707" alt="Ảnh chụp Màn hình 2024-01-13 lúc 01 04 09" src="https://github.com/berylhoang2501/Data-Manipulation-and-Visualization-with-Python/assets/152646327/cd7cfe5e-2c55-4b66-a856-66ba3e08873e">

*Hàm sắp xếp phần tử*
- np.arange([start,]stop[,step,]
- np.linspace(start,stop,num,endpoint)

nếu endpoint = True => bins = (stop - start)/(num - 1) không lấy stop

nếu endpoint = False => bins = (stop - start)/num lấy stop

* Tạo mảng bằng cách đọc vào tập tin txt

4. Truy xuất phần tử trong mảng
- Đối với truy xuất thì luôn luôn dùng ngoặc vuông
<img width="631" alt="Ảnh chụp Màn hình 2024-01-11 lúc 18 56 46" src="https://github.com/berylhoang2501/Data-Manipulation-and-Visualization-with-Python/assets/152646327/463c968c-0134-45cd-900f-972a2db570a8">

5. Cập nhật dữ liệu mảng (thêm, xoá, sửa)
- Thêm phần tử vào cuối mảng: np.concatenate[array,[value]])
- Chèn phần tử vào mảng 1 chiều: np.insert(arrld,position[s],value[s]) (lần lượt là #mảng cần chèn, vị trí index, giá trị cần chèn)
- Xoá phần tử: np.delete(arrld,position[s]) #position hiểu là index
- Sửa giá trị phần tử trong mảng

Bước 1: Truy xuất

Bước 2: Gán giá trị mới 
### Mảng nhiều chiều



