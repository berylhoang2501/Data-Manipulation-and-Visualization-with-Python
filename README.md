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

2. Thuộc tính của mảng
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

6. Các phép toán số học

7. Các hàm toán học
![Ảnh chụp Màn hình 2024-01-19 lúc 00 53 11](https://github.com/berylhoang2501/Data-Manipulation-and-Visualization-with-Python/assets/152646327/0700fe39-38b5-4e4c-8dd5-b306f4d91160)

8. Các hàm thống kê
<img width="676" alt="Ảnh chụp Màn hình 2024-01-19 lúc 00 57 57" src="https://github.com/berylhoang2501/Data-Manipulation-and-Visualization-with-Python/assets/152646327/84a94577-c3d1-4621-aacc-70d08500e651">

9. Sắp xếp mảng
- Sắp xếp tăng dần: np.sort(arr1)
- Sắp xếp giảm dần: np.sort(arr1)[::-1]

10. Chuyển đổi kiểu dữ liệu

array,astype()

## 13/1/2024: Buổi học 4: Thư viện Numpy
### Mảng nhiều chiều
1. Tạo mảng nhiều chiều

Cú pháp: numpy.array(object,dtype) 

Nếu có 2 cặp dấu ngoặc vuông ở đầu và 2 cặp dấu ngoặc vuông ở cuối thì là => mảng 2 chiều 

<img width="595" alt="Ảnh chụp Màn hình 2024-01-26 lúc 14 42 04" src="https://github.com/berylhoang2501/Data-Manipulation-and-Visualization-with-Python/assets/152646327/5237e0d8-9004-4683-a80d-ea3365844f04">

Đối với ví dụ trên thì chúng ta sẽ tạo ra 1 mảng có shape(4,5) tương ứng với 4 dòng và 5 cột 

4 list con tương ứng với 4 dòng, mỗi 1 list con có 5 phần tử, 5 phần tử trong list tương ứng với 5 cột 

2. Thuộc tính của mảng
<img width="678" alt="Ảnh chụp Màn hình 2024-01-26 lúc 14 52 54" src="https://github.com/berylhoang2501/Data-Manipulation-and-Visualization-with-Python/assets/152646327/0fd4a6d1-f065-41ac-9acc-5ff5afa5be3b">

3. Tạo mảng bằng các hàm tiện ích

lúc truyền dữ liệu phải truyền theo dạng shape(a,b) đầy đủ các thông số chứ không thể ghi 1 thông số như mảng 1 chiều 

<img width="671" alt="Ảnh chụp Màn hình 2024-01-26 lúc 15 01 12" src="https://github.com/berylhoang2501/Data-Manipulation-and-Visualization-with-Python/assets/152646327/972940fe-c3d6-4a98-a9c1-ee2577fa90da">

4. Truy xuất phần tử trong mảng
<img width="685" alt="Ảnh chụp Màn hình 2024-01-30 lúc 00 40 08" src="https://github.com/berylhoang2501/Data-Manipulation-and-Visualization-with-Python/assets/152646327/bf5a659d-c8e7-40e2-9d1a-eceac2a6c6cc">

5. Cập nhật dữ liệu mảng (thêm, xoá, sửa)

- Thêm: đối với mảng 2 chiều thì không thể thêm vào chỉ 1 phần tử vì sẽ làm phá vỡ cấu trúc của mảng 2 chiều. Chỉ được thêm nguyên dòng hoặc nguyên cột

np.concatenate([chuỗi muốn thêm vào,chuỗi sẽ thêm vào ], axis=0) #thêm dòng #axis=0 mặc định cho trục dọc (dòng) #có thể truyền nhiều list vào chuỗi cần thêm vào (thêm nhiều chuỗi cùng 1 lúc)

np.concatenate([chuỗi muốn thêm vào,chuỗi sẽ thêm vào ], axis=1) #thêm cột #axis=1 mặc định cho trục ngang (cột) #có thể truyền nhiều list vào chuỗi cần thêm vào (thêm nhiều chuỗi cùng 1 lúc)

- Chèn: 
np.insert(arr2d, position[s], new_row[s] là chuỗi cần chèn, axis=0) #thêm dòng #axis=0 mặc định cho trục dọc (dòng)

np.insert(arr2d, position[s], new_col[s] là chuỗi cần chèn, axis=1) #thêm cột #axis=1 mặc định cho trục ngang (cột)

- Xoá:

- Sửa giá trị phần tử trong mảng:

Bước 1: Truy xuất

Bước 2: Gán giá trị mới (truy xuất ra bao nhiêu số thì gán đủ lại bấy nhiêu số)

6. Thực hiện phép toán số học từng phần trên mảng

![Ảnh chụp Màn hình 2024-02-10 lúc 17 57 40](https://github.com/berylhoang2501/Data-Manipulation-and-Visualization-with-Python/assets/152646327/d3791d2d-edc5-41ec-8ca5-72c93a7e49f1)

7. Các hàm thống kê cơ bản

<img width="970" alt="Ảnh chụp Màn hình 2024-02-10 lúc 17 59 41" src="https://github.com/berylhoang2501/Data-Manipulation-and-Visualization-with-Python/assets/152646327/c8be4b91-978f-4995-a276-187017782d33">

axis=0: thống kê các dòng trong cột
axis=1: thống kê các cột trong dòng

8. Hệ số tương quan Peason: np.corrcoef (correlation coefficients)
- strong negative correlation (<0.7): Nếu một biến tăng, thì biến còn lại giảm, và ngược lại.

<img width="347" alt="Ảnh chụp Màn hình 2024-02-10 lúc 18 57 31" src="https://github.com/berylhoang2501/Data-Manipulation-and-Visualization-with-Python/assets/152646327/1b9690ed-f6f4-49f5-9355-4197cb5834b0">

- weak correlation (0-0.2)

<img width="278" alt="Ảnh chụp Màn hình 2024-02-13 lúc 00 18 03" src="https://github.com/berylhoang2501/Data-Manipulation-and-Visualization-with-Python/assets/152646327/618d167b-5e80-4206-b680-84c88a82668b">

- strong positive correlation (>0.7): Nếu một biến tăng, thì biến còn lại cũng tăng, và ngược lại.

<img width="292" alt="Ảnh chụp Màn hình 2024-02-13 lúc 00 18 21" src="https://github.com/berylhoang2501/Data-Manipulation-and-Visualization-with-Python/assets/152646327/867d2fc4-4017-4ff8-afa9-edbee594a9b5">

9. Sắp xếp mảng:

np.sort(arr, axis = 0 nếu theo cột và = 1 nếu theo dòng)

10. Biến đổi mảng (reshape): thay đổi kích thước mảng, chiều của mảng (thay đổi số dòng, số cột)

Biến đổi mảng 2 chiều thành mảng 1 chiều: arr2.reshape(-1)

Chuyển vị: np.transpose() hoặc arr.T (chuyển dòng thành cột, cột thành dòng)

11. Kết hợp mảng

Tìm phần tử chung giữa 2 mảng: np.intersectld(_,_)
Phần tử chỉ xuất hiện ở 1 mảng: np.setdiffld(_,_)

**Một số hàm hay dùng**
- Làm tròn 2 chữ số thập phân: np.round
- Tính trung bình: np.mean

## 14/1/2024: Buổi học 5: Thư viện Pandas
### Giới thiệu

Thư viện Pandas giúp cho chúng ta xử lý dữ liệu, dữ liệu chủ yếu là dữ liệu có cấu trúc: dạng bảng như tập tim Excel, tập tim .csv, tập tin.txt, view từ CSDL 

Dùng để: khám phá, làm sạch, phân tích và trực quan hoá

Tốc độ xử lý cao, dễ thao tác

Có 2 kiểu cấu trúc dữ liệu: Series (dựa trên cấu trúc mảng 1 chiều) và DataFrame (dựa trên cấu trúc mảng 2 chiều

### Series

- Là  cấu trúc dữ liệu 1 chiều có gán nhãn. Mỗi phần tử trong Series gồm value (data) và index (label)
- Đặc điểm:

Index ngầm định (không hiển thị ra bên ngoài, lấy theo numpy) vs. index tường minh (label - thấy được ở bên ngoài - có thể tự đặc)

Các phần tử trong Series phải có cùng kiểu dữ liệu

***1. Phương thức tạo series***

- pandas.Series (data [,index] [,dtype])

[,index] nếu không truyền vào thì sẽ là dạng tường minh 0 base từ 0 -> n - 1

[,dtype] mặc định lấy theo kiểu dữ liệu lớn nhất của data

[,index] tường minh là index có thể thấy được, người dùng tự xác định giá trị index, index có thể là số và là chuỗi 

[,index] ngầm định là index không hiển thị ra bên ngoài (lấy theo numpy, index dương và index âm)

load.txt giống genfromtxt nhưng load.txt chỉ đọc được file txt còn genfromtxt đọc được cả file csv

***2. Thuộc tính***
<img width="905" alt="Ảnh chụp Màn hình 2024-02-19 lúc 23 06 00" src="https://github.com/berylhoang2501/Data-Manipulation-and-Visualization-with-Python/assets/152646327/53d68f18-308c-408f-a3d7-55cf91cec030">

cách in thuộc tính thì chỉ cần .thuộc tính

***3. Phương thức***
<img width="652" alt="Ảnh chụp Màn hình 2024-02-18 lúc 15 26 37" src="https://github.com/berylhoang2501/Data-Manipulation-and-Visualization-with-Python/assets/152646327/13f1111c-0366-4d2e-8bd2-ea9dbbc0d6ca">

- .info(): hiển thị thông tin sơ bộ của dữ liệu
- .head(n): hiển thị 5 dòng đầu, n mặc định là 5, có thể truyền thông số khác 5 vào
- .describe(): thông tin thống kê chung

***4. Truy xuất***

<img width="977" alt="Ảnh chụp Màn hình 2024-02-19 lúc 23 33 01" src="https://github.com/berylhoang2501/Data-Manipulation-and-Visualization-with-Python/assets/152646327/071805f7-d09e-4442-9418-87cd0c57a1f6">

(luôn luôn sử dụng dấu ngoặc vuông)

- Đối với truy xuất 1 phần tử

ser.loc[<lable>] -> tương đương với index tường minh

ser.iloc[<index>] -> tương đương với 2 index ngầm định

- Đối với truy xuất nhiều phần tử

ser.loc[list of lable] -> không quy tắc

ser.iloc[start:stop:step] -> có quy tắc

- Đối với truy xuất theo điều kiện: sử dụng các biểu thức điều kiện giống trong mảng numpy

***5. Phát hiện dữ liệu trùng (duplicate)***

- ser.duplicated([keep]) # mặc định keep=first

- ser.drop_duplicates(keep=False,inplace=True) #inplace = True thì thông tin mới được cập nhật trên chuỗi

### DataFrame   
- Là cấu trúc dữ liệu 2 chiều, được tổ chức theo dòng và cột

***1. Phương thức tạo DataFrame***

pandas. DataFrame (data (, index] [, columns])

- data: dữ liệu (list, dict, ndarray, series, dataframe)
- index: danh sách nhãn dòng; index = ['tên dòng 1', 'tên dòng 2',...], nếu không truyền dữ liệu vào thì sẽ mặc định từ 0 -> n-1
- columns: danh sách nhãn cột; columns = ['tên cột 1', 'tên cột 2',...], nếu không truyền dữ liệu vào thì sẽ mặc định từ 0 -> m-1

### Làm sạch dữ liệu
1. Thay thế giá trị

Thay thế trên 1 cột: df['tên cột'].replace(giá_trị_cũ, giá_trị_mới)

### Cập nhật và xử lý dữ liệu



