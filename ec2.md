# Spot Instances

Tính chất
Khối lượng việc ngắn, giá rẻ, có thể mất instance
Giá thành rẻ hơn đến 90% so vơi On-Demand Instance
Chọn mức giá tối đa chúng ta sử dụng instance, nếu quá tự động terminate
Giá biến đối dựa trên nhà cung cấp và nhu cầu người dùng ( càng nhiều người muốn dùng thì nguy cơ tăng giá cao)
Sẽ thu hồi ngay 2 phút sau cảnh báo giá vượt mức max price.
 # Khi nào nên sử dụng Spot Instances
Chạy các batch jobs (hẹn giờ, lên lịch).
Chạy thống kê phân tích dữ liệu lớn (Big Data analysis)
Giờ cao điểm, nhiều user truy cập
Crawl dữ liệu
Tích hợp với các services như Auto Scaling, EMR, ECS, CloudFormation, Data Pipeline và AWS Batch.
