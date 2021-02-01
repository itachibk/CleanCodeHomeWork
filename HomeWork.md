# Tran The Hong
## Khoá học Clean Code - Luvina 2020


## Phần 1: Clean Code căn bản
1. 5 mục tiêu chính của Clean Code là
   - Mục tiêu 1 : Đặt tên dễ hiểu – tránh nhầm lẫn , dễ hiểu tránh nhầm lẫn
   không đặt trên chung chung khó hiểu => đặt tên đúng sẽ dễ đọc hiểu code, code sạch hơn.
   - Mục tiêu 2 : Hàm – Function / Method: Không quá dài ,làm nhiều nhiệm vụ( gọn gàng làm 1 việc,làm đúng tên mô tả,không tạo hiệu ứng phụ ),có nhiều tham số(ít hơn 3 tham số),
   trong hàm không dùng biến cờ rẽ nhánh nhiều việc trong 1 hàm.Không nên lạm dụng comment quá nhiều, không đúng mục đích.
   - Mục tiêu 3 : Thiết kế tốt ít sự phụ thuốc dễ dàng mở rộng, khi sửa ảnh hưởng ít đến các chức năng khác.
   - Mục tiêu 4 : Định dạng mã nguồn Code Format chuẩn , không có code trùng lặp 
   - Mục tiêu 5 : Cần áp dụng Kiểm thử - unit test để đảm bảo code chạy đúng theo trường hợp.

2. Đáp án của tôi là team C bởi vì:
   - Team C: Áp dụng Clean Code là một quá trình. Quy tắc nào dễ hiểu, dễ nhớ thì áp dụng trước. Những kỹ thuật phức tạp sẽ học và áp dụng trong tình huống phù hợp. Cân bằng giữa tiến độ và clean code.
   Vì việc áp dụng luôn Clean Code hoàn toàn 100% là điều rất khó với 1 team chưa có nhiều kinh nghiệm về CleanCode
   do đó việc dành 30% để đào tạo cleancode có rất nhiều rủi ro về deadline với KH. Thêm nữa việc ap dụng theo team A,B,C cũng tùy dự án,
   tùy từng hoàn cảnh mới có thể cân nhắc lựa chọn phương án nào. Nếu có nhiều thời gian với những dự án lớn  thì sẽ chọn phương án của team B, những dự án maintain chọn phương án team C.

3. Bạn là một team lead, khi bạn giới thiệu các quy tắc Clean Code cho các đồng đội trẻ. Có một số bạn cho rằng Clean Code chỉ làm phức tạp thêm vấn đề, và chậm lại hiệu suất làm việc của nhóm.
 Bạn sẽ trả lời họ thế nào?
  - Trước hết sẽ nêu ra nhưng điểm yếu khi không clean code , và nhưng điểm lợi khi clean code. Chỉ cho member thấy được việc áp dung clean code giúp cho việc code dễ đọc giúp chính họ hoặc 
  các member khác trong team dễ dàng hiểu được những dòng code họ viết ra.
  -Chỉ cho member thấy được: Việc dễ dàng mở rộng , bảo trì sau này.v.v cần có các ví dụ cụ thể để member có thể hiểu được.
  
4. Bob, Alice, Toàn, Vân được sếp giao cho viết một hàm tính lương tăng theo năm làm việc.
    Đề xuất của Vân float raise là thuộc tính trong class Salary rồi. 
     int calculateSalaryAfterYears(int initialSalary, int NthYear);

5.

public class User {
   private long id;
   private String fullName;
   private ArrayList<Post> posts;  //Một người có thể viết nhiều Post
   private ArrayList<Comment> comments; //Một người có thể bình luận nhiều Comment
   //---- Bổ xung method vào đây. Nhiệm vụ của các bạn đó !

   void writePost(Post post) { //ví dụ mẫu một phương thức nhé
      //Bổ xung logic vào đây
   }

   void deletePost(Post post) throws PostException {  //Nếu tác động lên dữ liệu nếu có lỗi thì hãy throw ra Exception

   }
}

public class Post {
   private long id;
   private String title;
   private String content;
   private User author; //Tác giả của bài viết
   private ArrayList<Comment> comments; //Một post chứa nhiều Comment
   //---- Bổ xung method vào đây. Nhiệm vụ của các bạn đó ! 
}

private class Comment{
   private long id;
   private String title;
   private Post post; //Bài viết mà comment gắn vào
   private User author; //Tác giả của comment
   //---- Bổ xung method vào đây. Nhiệm vụ của các bạn đó !
}
## Phần 2: OOP và SOLID
### 1. Hãy lập trình Java để thực hiện thiết kế như hình vẽ
https://github.com/itachibk/05OOP/tree/main/jungle/src/main/java/graphiceditor/after

### 2. Composition over Inheritance và DI
Gõ link đến mã nguồn bài này vào đây


## Phần 3: Thiết kế CSDL Quan hệ theo đặc tả

## Phần 4: Thiết kế RESTful API

## Phần 5: Lập trình Restful API

## Trắc nghiệm
Điều nào không đúng khi nói về Design Pattern?
A. Là tập hợp các giải pháp có thể tái sử dụng cho các vấn đề thường xảy ra trong thiết kế phần mềm.
B. Được xây dựng dựa trên kiến thức và kinh nghiệm của các nhà chuyên gia phát triển phần mềm.
C. Đã được thiết kế và cài đặt ở mức chi tiết.
C. Giúp tăng tính gắn kết (high cohesion) và giảm sự phụ thuộc (low coupling) giữa các thành phần trong phần mềm.
Các OOP Design Pattern được chia làm mấy nhóm?
A. 2
B. 3
C. 4
D. 5
Các design pattern của nhóm Behavioral pattern có đặc điểm nào dưới đây?
A. Quan tâm đến cách các lớp và các đối tượng được tổ chức để trở thành một cấu trúc lớn hơn.
B. Cung cấp các cơ chế khởi tạo đối tượng khác nhau, làm tăng tính linh hoạt và tái sử dụng code.
C. Là các giải pháp để triển khai cho các hệ thống Microservice.
D. Quan tâm đến cách giao tiếp giữa các lớp và các đối tượng.
Trong trường hợp client muốn khởi tạo một đối tượng mà không cần quan tâm logic khởi tạo đối tượng hoặc không biết rõ lớp của đối tượng thì chúng ta nên áp dụng design pattern nào đã được học?
A. Builder
B. Singleton
C. Factory Method
D. Strategy
Cách cài đặt Bill Pugh của Singleton pattern có đảm bảo thread-safe hay không?
A. Có
B. Không
C. Một số trường hợp thì có, một số trường hợp thì không
Đối tượng được khởi tạo bằng Builder pattern có điểm gì khác biệt so với đối tượng được khởi tạo bằng cách thông thường (thông qua toán tử new, rồi sau đó set các giá trị thông qua setter method)?
A. Mutable
B. Immutable
Khi sử dụng annotation @Builder của Lombok thì đối tượng được khởi tạo có đảm bảo immutable hay không?
A. Không
B. Có
Trong design pattern Flyweight, chúng ta lưu trữ loại dữ liệu nào trong bộ nhớ cache (flyweight factory)?
A. Dữ liệu không thay đổi theo context
B. Dữ liệu thay đổi theo context
C. Cả A và B
Nếu có nhiều class chứa các thuật toán gần như giống hệt nhau và chỉ có một số ít khác biệt, thì chúng ta sẽ áp dụng design pattern nào đã được học để tránh bị lặp lại code, cũng như tốn ít công sức sửa code nếu có yêu cầu phải thay đổi tất cả các thuật toán?
A. Strategy
B. Template Method
C. Flyweight
D. Builder
Một tác vụ có nhiều thuật toán để xử lý. Để dễ dàng chuyển đổi thuật toán tại thời điểm chạy chương trình tùy theo request từ phía client, chúng ta sẽ áp dụng design pattern nào đã được học?
   A. Strategy
   B. Factory method
   C. Singleton
   D. Flyweight
REST là gì?
   A. Ngôn ngữ lập trình
   B. Kiểu kiến trúc phần mềm
   C. Giao thức
   D. Không đáp án nào chính xác
Đâu không phải là đặc điểm của một hệ thống RESTful?
   A. Client và server có thể xây dựng và phát triển một cách độc lập mà không ảnh hưởng đến nhau.
   B. Response của server có thể được lưu trong bộ nhớ cache để tăng hiệu năng.
   C. Server lưu trữ session và history của client.
   D. Hệ thống có thể chia thể chia thành nhiều layer.
Khi RESTful API có nhiệm vụ thêm mới một resource, chúng ta nên sử dụng HTTP method nào?
   A. PUT
   B. POST
   C. PATCH
   D. DELETE
HTTP method nào không đảm bảo idempotent trong tất cả các trường hợp?
   A. GET
   B. POST
   C. PUT
   D. B và C
Chúng ta nên sử dụng query parameter cho những trường hợp nào?
   A. Phân trang
   B. Sắp xếp
   C. Lọc
   D. Cả 3 đáp án trên
Các interface/class có nhiệm vụ thao tác với cơ sở dữ liệu được đặt ở layer nào?
   A. Service
   B. Repository
   C. Controller
Các bạn đã được tìm hiểu mấy phương pháp đánh version cho RESTful API trong khóa học?
   A. 1
   B. 2
   C. 3
   D. 4
Trong Spring Framework, phương pháp xử lý lỗi nào dưới đây cho phép chúng ta xử lý lỗi ở mức toàn ứng dụng (global)?
   A. Sử dụng @ControllerAdvice và @ExceptionHandler
   B. Chỉ sử dụng @ExceptionHandler
   C. Throw ResponseStatusException
Để thông báo cho người quản trị hệ thống biết một chức năng đã gặp lỗi, chúng ta nên sử dụng log level nào?
   A. INFO
   B. DEBUG
   C. ERROR
   D. WARNING
Để cảnh báo việc tiến trình có thể không chạy đúng với logic, nhưng ứng dụng vẫn có thể tiếp tục, chúng ta nên sử dụng log level nào?
   A. TRACE
   B. WARN
   C. INFO
   D. ERROR
Có phải method được đánh dấu annotation @Cacheable luôn được thực thi mỗi khi RESTful API được gọi?
   A. Có
   B. Không
Anti-pattern Jaywalking phù hợp trong trường hợp nào?
   A. Cần thống kê dễ dàng.
   B. Cần lưu một danh sách các phần tử dưới dạng phân cách nhau bởi ký tự đặc biệt và không cần truy vấn từng phần tử.
   C. A và B.
   D. Không có đáp án nào chính xác.
Đâu không phải là giải pháp phù hợp để thay thế cho anti-pattern Multi-column Attributes? Giả sử tôi cần lưu các tag của một article.
   A. Tạo một bảng trung gian (join table) giữa tag và article.
   B. Lưu giá trị của các tag vào N cột trong bảng article.
   C. Tạo một bảng riêng để lưu các tag của article.
Nếu sử dụng anti-pattern Entity-Value-Attribute, giả sử đối tượng có 5 thuộc tính, vậy tôi cần thực hiện tất cả bao nhiêu phép JOIN để lấy đủ thông tin của 5 thuộc tính?
   A. 1
   B. 3
   C. 5
   D. 6
Tree model nào không dễ để query child node ngay dưới?
   A. Adjacency list
   B. Path enumeration
   C. Nested Set
   D. Closure table