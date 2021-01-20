# SparkvaMapreduce

**Spark** : Nó là một khung dữ liệu lớn nguồn mở. Nó cung cấp một công
cụ xử lý dữ liệu có mục đích chung nhanh hơn và nhiều hơn. Spark về cơ
bản được thiết kế để tính toán nhanh. Nó cũng bao gồm một loạt các khối
lượng công việc - ví dụ, lô, tương tác, lặp và phát trực tuyến.

**Hadoop MapReduce** : ** **Đây cũng là một khung nguồn mở để viết các
ứng dụng. Nó cũng xử lý dữ liệu có cấu trúc và không cấu trúc được lưu
trữ trong HDFS. Hadoop MapReduce được thiết kế theo cách xử lý một khối
lượng lớn dữ liệu trên một cụm phần cứng hàng hóa. MapReduce có thể xử
lý dữ liệu trong chế độ hàng loạt.

**Xử lí dữ liệu**

**Spark** : Apache Spark phù hợp cho cả xử lý hàng loạt và xử lý luồng,
nghĩa là nó là khung xử lý kết hợp. **Spark tăng tốc xử lý hàng loạt
thông qua tính toán trong bộ nhớ và tối ưu hóa xử lý** . Đó là một lựa
chọn tốt để truyền tải khối lượng công việc, truy vấn tương tác và học
máy. Spark cũng có thể hoạt động với Hadoop và các mô-đun của nó. Khả
năng xử lý dữ liệu thời gian thực của nó khiến Spark trở thành lựa chọn
hàng đầu cho các phân tích dữ liệu lớn.

Bộ dữ liệu phân tán linh hoạt (RDD) của nó cho phép Spark lưu trữ dữ
liệu trong bộ nhớ một cách trong suốt và chỉ gửi vào đĩa những gì quan
trọng hoặc cần thiết. Kết quả là, rất nhiều thời gian dành cho việc đọc
và ghi trên đĩa được lưu lại.

**Hadoop** : Apache Hadoop cung cấp xử lý hàng loạt. Hadoop phát triển
rất nhiều trong việc tạo ra các thuật toán mới và ngăn xếp thành phần để
cải thiện quyền truy cập vào xử lý hàng loạt quy mô lớn.

MapReduce là công cụ xử lý hàng loạt riêng của Hadoop. Một số thành phần
hoặc lớp (như YARN, HDFS, v.v.) trong các phiên bản hiện đại của Hadoop
cho phép dễ dàng xử lý dữ liệu hàng loạt. Vì MapReduce là về lưu trữ
vĩnh viễn, **nó lưu trữ dữ liệu trên đĩa, có nghĩa là nó có thể xử lý
các bộ dữ liệu lớn** . MapReduce có khả năng mở rộng và đã chứng minh
hiệu quả của nó để đối phó với hàng chục ngàn nút. Tuy nhiên, quá trình
xử lý dữ liệu của Hadoop rất chậm do MapReduce hoạt động theo các bước
tuần tự khác nhau.

**Phân tích thời gian thực**

**Spark** : ** **Nó có thể xử lý dữ liệu thời gian thực, tức là dữ liệu
đến từ các luồng sự kiện thời gian thực với tốc độ hàng triệu sự kiện
mỗi giây, chẳng hạn như dữ liệu Twitter và Facebook. Sức mạnh của Spark
nằm ở khả năng xử lý luồng trực tiếp hiệu quả.

**Hadoop MapReduce** : MapReduce thất bại khi xử lý dữ liệu thời gian
thực, vì nó được thiết kế để thực hiện xử lý hàng loạt trên lượng dữ
liệu khổng lồ.

**Dễ sử dụng**

**Spark** : Spark dễ sử dụng hơn Hadoop, vì nó đi kèm với các API thân
thiện với người dùng cho Scala (ngôn ngữ gốc của nó), Java, Python và
Spark SQL. Vì Spark cung cấp một cách để thực hiện phát trực tuyến, xử
lý hàng loạt và học máy trong cùng một cụm, người dùng dễ dàng đơn giản
hóa cơ sở hạ tầng của mình để xử lý dữ liệu.
[*REPL*](https://en.wikipedia.org/wiki/Read%E2%80%93eval%E2%80%93print_loop)
tương tác  (Read-Eval-Print Loop) cho phép người dùng Spark nhận phản
hồi tức thì cho các lệnh.

**Hadoop** : Mặt khác, Hadoop, được viết bằng Java, rất khó lập trình và
đòi hỏi sự trừu tượng. Mặc dù không có chế độ tương tác có sẵn với
Hadoop MapReduce, các công cụ như Pig và Hive giúp người dùng dễ dàng
làm việc với nó hơn.

**Xử lý đồ thị**

**Spark** : Spark đi kèm với một thư viện tính toán đồ thị có tên là
GraphX ​​để làm cho mọi thứ trở nên đơn giản. Tính toán trong bộ nhớ kết
hợp với hỗ trợ đồ thị dựng sẵn cho phép thuật toán thực hiện tốt hơn
nhiều so với các chương trình MapReduce truyền thống. Netty và Akka giúp
Spark có thể phân phối tin nhắn trong toàn bộ những người thực thi.

**Hadoop** : Hầu hết các thuật toán xử lý, như PageRank, thực hiện nhiều
lần lặp trên cùng một dữ liệu. MapReduce đọc dữ liệu từ đĩa và sau một
lần lặp cụ thể, sẽ gửi kết quả đến HDFS, rồi lại đọc dữ liệu từ HDFS cho
lần lặp tiếp theo. Quá trình này làm tăng độ trễ và làm cho xử lý đồ thị
chậm.

Để đánh giá điểm của một nút cụ thể, việc truyền thông điệp cần phải
chứa điểm của các nút lân cận. Các tính toán này yêu cầu tin nhắn từ các
nước láng giềng, nhưng MapReduce không có bất kỳ cơ chế nào cho việc đó.
Mặc dù có các công cụ nhanh và có thể mở rộng như Pregel và GraphLab cho
các thuật toán xử lý đồ thị hiệu quả, nhưng chúng không phù hợp với các
thuật toán đa giai đoạn phức tạp.

**Dung sai lỗi**

**Spark** : Spark sử dụng RDD và các mô hình lưu trữ dữ liệu khác nhau
để chịu lỗi bằng cách giảm thiểu I / O mạng. Trong trường hợp mất phân
vùng của RDD, RDD sẽ xây dựng lại phân vùng đó thông qua thông tin mà nó
đã có. Vì vậy, Spark không sử dụng khái niệm nhân rộng cho khả năng chịu
lỗi.

**Hadoop** : Hadoop đạt được khả năng chịu lỗi thông qua sao chép.
MapReduce sử dụng TaskTracker và JobTracker cho khả năng chịu lỗi. Tuy
nhiên, TaskTracker và JobTracker đã được thay thế trong phiên bản thứ
hai của MapReduce bởi Node Manager và ResourceManager /
ApplicationMaster.

**Bảo vệ**

**Spark** : Bảo mật của Spark hiện đang ở giai đoạn đầu, chỉ cung cấp hỗ
trợ xác thực thông qua bí mật chung (xác thực mật khẩu). Tuy nhiên, các
tổ chức có thể chạy Spark trên HDFS để tận dụng các ACL HDFS và quyền
cấp độ tệp.

**Hadoop MapReduce** : Hadoop MapReduce có các tính năng bảo mật tốt hơn
Spark. Hadoop hỗ trợ xác thực Kerberos, đây là một tính năng bảo mật tốt
nhưng khó quản lý. Hadoop MapReduce cũng có thể tích hợp với các dự án
bảo mật của Hadoop, như Knox Gateway và Sentry. Các nhà cung cấp bên thứ
ba cũng cho phép các tổ chức sử dụng Active Directory Kerberos và LDAP
để xác thực. Hệ thống tệp phân tán của Hadoop tương thích với danh sách
kiểm soát truy cập (ACL) và mô hình cấp phép tệp truyền thống.

**Khả năng tương thích**

Cả Hadoop và Spark đều tương thích với nhau. Spark có thể tích hợp với
tất cả các nguồn dữ liệu và định dạng tệp được Hadoop hỗ trợ. Cả Hadoop
và Spark đều có thể mở rộng.

Sự khác biệt giữa Apache Spark so với Hadoop MapReduce cho thấy **Apache
Spark là công cụ tính toán cụm tiên tiến hơn nhiều so với MapReduce** .
Spark có thể xử lý bất kỳ loại yêu cầu nào (ví dụ: lô, tương tác, lặp,
phát trực tuyến, đồ thị) trong khi MapReduce giới hạn xử lý hàng loạt.
