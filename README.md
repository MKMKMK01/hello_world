# hello_world
first commit 
2thd

theme: jekyll-theme-cayman
Hello
Chạy thử chương trình:
 
Đọc code assembly ta thấy chương trình cho người dùng nhập name và lưu name vào vùng nhớ có địa chỉ buf 
![image](https://user-images.githubusercontent.com/62017752/121049879-51922280-c7e2-11eb-8e9c-bc0d493b0eef.png)

 
Nhập thử name quynh và pass là 123 để debug 
Chương trình lưu chuỗi “Hello ” vào vùng nhớ có địa chỉ welcome 402094, sau đó lưu giá trị Name ở buf vào vùng nhớ có địa chỉ 40209A như hình :

![image](https://user-images.githubusercontent.com/62017752/121050116-82725780-c7e2-11eb-8ca4-b272fbb7510a.png)

Phân tích code kết hợp debug quan sát giá trị các thanh ghi, ta thấy ban đầu r15 chứa giá trị là độ dài của chuỗi pass, r14 = r15 +5 (bỏ qua chuỗi “Hello ”), chương trình thực hiện so sánh (giá trị tại địa chỉ byte_402073[r15]) +5 (vùng nhớ tại địa chỉ 402074 lưu chuỗi pass) với giá trị tại địa chỉ welcome[r14], tức là so sánh kí tự cuối của pass với kí tự tiếp cách 5 trong bảng mã ASCII của kí tự cuối của Name. Sau đó giảm r15 và lặp lại quá trình trên tới khi r15=0.
Vậy suy ra độ dài pass bằng Name và pass[i]= chr (ord(Name[i])+5).
 

Sẽ có rất nhiều nghiệm. Chọn Name là ab và Pass là fg
Kiểm tra
![image](https://user-images.githubusercontent.com/62017752/121050161-8bfbbf80-c7e2-11eb-99e5-7a90c72abc45.png)

theme: jekyll-theme-cayman
 
