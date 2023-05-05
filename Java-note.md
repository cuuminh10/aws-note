# introduce about your sel?
Hello everyone, my name is Minh Hoang, I have 5 years of experience, my strongest technology is Java with Spring framework, also I can do well with other backend languages ​​like nodejs and python, how about FE I can do well with ReactJS and AngularJS languages, the databases that I have worked on are PostgresSQL, Oracle, MySQL and I also have cloud knowledge AWS and Azure



# What the different between Put and Patch ?
Put is used to update objects.
Patches are used to update fields in objects.

# Compare between param and path variable ?
The parameters and path variables are passed values through urls. 
The difference is: the param will pass behind the question mark and declare along with the variable name. Path variable: passed through parameters after splash



# Khi sử dụng JPA/Hibernate, bạn hay dùng các method được provide sẵn hay sử dụng @Query annotation?
Tùy theo ngữ cảnh của data mà API đó mong muốn nếu là một api đơn giản chỉ làm việc trên 1 entity và khôi có nhiều điều kiện thì tôi sẽ sử dụng method provide của Hibernate
Nhưng data mà api mong muốn là data chứng dữ liệu của các nhiều bảng được join với nhau thì tôi sẽ thực hiện native query thông qua annotation @Query


Based on the context of the data required by the API, if it is a simple API that only works on one entity and has multiple conditions, I will use Hibernate's provide method.
But the data that the API wants is proof of data from multiple tables connected together, and I will execute the native query through annotation @ Query.

# Khi dùng @Query annotation, bạn sử dụng dưới dạng native query hay hql/jpql?
Khi dùng @Query annotation tôi hay sử dụng native query
When using annotation @Query I usually use native query

# Giải quyết bài toán n+1 trong Hibernate như thế nào?
Tôi sẽ giải quyết bằng cách sử dụng  JOIN FETCH trong câu lệnh query của JPQL/HQL, 
và còn 1 cách nữa là sử dụng  @Fetch(FetchMode.SUBSELECT) với field của entity đó

I will solve by using JOIN FETCH JPQL/HQL query statement,
and one more way is to use @Fetch(FetchMode.SUBSELECT) with the field of that entity

# Khi viết unit test thì bạn viết cấu trúc ntn?
Khi tôi viết Unittest tôi sẽ phải xác định mục đích mỗi case mình sẽ test, nếu tôi có các object có thể reused lại nhiều lần tôi sẽ sử dụng @beforeAll
còn nếu với mỗi case tôi sẽ có 1 object khác nhau tôi sẽ sửng dụng beforeEach, và tương tự với nó tôi sẽ có @AfterAll, @AfterEach
với mỗi case test tôi sẽ khai báo nói bằng @Test annotations.
và trong mỗi case tôi sẽ so sánh gía trị trả về bằng phương thức assertEquals, nếu là boolean thì assertTrue

When I write Unittest I will have to define the purpose of each case I will test, if I have objects that can be reused many times I will use @beforeAll
but if for each case i will have a different object i will use beforeEach, and similar to it i will have @AfterAll, @AfterEach
For each test case I will declare it with @Test annotations.
and in each case i will compare the return value by assertEquals method, if it is boolean then assertTrue

# Khi viết unit test thì bạn có tiêu chí nào để đánh giá hiệu quả không? 
tôi sẽ cover hết toàn bộ các line code của mình theo đúng bussiness, và coverrage ít nhất là 80% line code mà tôi đã sửa đổi cho services đó 

I will cover all my line coding arcoding to right bussiness, and coverrage at least is 80%  of the line code that i modifed to that services

# Khi done 1 API thì làm sao để bạn bàn giao lại cho bên FE ? Theo cách thức như nào ?

when i did an API i will start to write a document about Explain the detail of API including the header, method HTTP,  payload, and response model beside have any error status code if the request data from the client is invalid

# Khi bạn triển khai 1 project mà có sự thay đổi vào DB thì bạn làm như nào ?
In that case, it will two solutions 
first we can config in application flag that ddl-auto is an update for each change from the entity it  will map with database those changes and after that avoid missing those changes we must write a script sql in the package have name migration so that when DevOps they deploy will not miss those changes
and the second if we won't ORM handle to those changes , we should set ddl-auto is none , and write script in package migration

