# What the different between Put and Patch ?
Put is used to update objects.
Patches are used to update fields in objects.

# Compare between param and path variable ?
Param and path pass do parameters through URLs
    The difference is : param will be passed after the question mark and declared along with the variable name.
                Path variable: passed through parameters after splash


# Khi sử dụng JPA/Hibernate, bạn hay dùng các method được provide sẵn hay sử dụng @Query annotation?
Tùy theo ngữ cảnh của data mà API đó mong muốn nếu là một api đơn giản chỉ làm việc trên 1 entity và khôi có nhiều điều kiện thì tôi sẽ sử dụng method provide của Hibernate
Nhưng data mà api mong muốn là data chứng dữ liệu của các nhiều bảng được join với nhau thì tôi sẽ thực hiện native query thông qua annotation @Query


Based on the context of the data required by the API, if it is a simple API that only works on one entity and has multiple conditions, I will use Hibernate's provide method.
But the data that the API wants is proof of data from multiple tables connected together, and I will execute the native query through annotation @ Query.

