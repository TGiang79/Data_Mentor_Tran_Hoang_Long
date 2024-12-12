Lớp DA thầy Long
Lộ trình học 3 Level, Qua các level được làm task thật, data thật từ các công ty, và làm trên cơ sở hạ tầng thật (azure cloud , aws , oracle , big query ) do thầy Long cài cắm, giống với thực tế đi làm ở các doanh nghiệp khoảng 80%. Tất cả đều là dữ liệu thật, và real tasks từ các yêu cầu của công ty trong thực tế.

Level 1: Descriptive Analytics

Level 2: Diagnostic Analytics

Level 3: Predictive Analytics


### Level 1 Descriptive Analytics

Phân tích thống kê để làm báo cáo 
- Tool: **SQL**, Data Studio, Tableau, PBI
- Concepts: Database, DBMS, RDBMS, data warehouse, SQL query optimization, data partition, distribution, window function, pivot
- Statistics: Basic
  
⇒ Đầu ra học viên có thể làm được những tác vụ operational intelligence và business intelligence cơ bản , set up cơ sở hạ tầng ,triển khai DW cho doanh nghiệp.

Example 1: báo cáo nhóm khách hàng tiềm năng tháng 1 ,  đâu là 10 thằng khách hàng chi tiêu nhiều nhất trong quý 3 , đâu là 10 sản phẩm có nhiều người mua nhất

Các task mang tính reporting , hầu hết các công ty thường làm và không mang nặng insights & analytics, còn gọi là business intelligence, đa phần các cty vừa và nhỏ có làm analytics cũng chỉ cần như vậy.

Trong thực tế làm thì phải nắm được data model , kiến thức nghiệp vụ để làm được việc vì mỗi công ty có kiểu tổ chức dữ liệu khác nhau , và khái niệm khác nhau , cần phải có kỹ năng để xử lý.

Đôi khi phải hỗ trợ công ty thiết kế Data model , Data Warehouse luôn nếu công ty không có.

Example 2: Lấy ra tập khách hàng tiềm năng t1 2023 , biết khách hàng tiềm năng là người có các chỉ số A B C, A B C thì phải tính bằng X Y Z, X Y Z nằm ở các bảng , các bảng liên kết vs nhau ntn, data model ra làm sao, rồi áp dụng window function để làm ranking xem khách nào top 1 , top 2.

Thực tế đôi khi mình vào ngay cty chỉ có db , chưa có DW , mình cũng phải bắt tay vào thiết kế, có data thì mới làm analytics đc. Như olap vs oltp , chọn cái nào. Hay biết chọn sql, nosql , hiểu biết chút về dbms.

Một số người có thể tự tin biết sql ,pbi rồi, nhưng khi làm real task hoặc technical test thực tế của doanh nghiệp thì fail hết vì ko biết hạ tầng , fundamental knowledge , chỉ biết tool bề nổi. Cần phải học để biết:
- Tự set up 1 cái sql server , Biết access vào db là những cái cơ bản tối thiểu để làm việc chứ không phải tools về SQL , select * from where thôi là không đủ.
- Biết kỹ năng text to code , nhận yêu cầu , requirements và triển khai thành data model , data preparation.
- Phân biệt được các tech stack cơ bản.


### Level 2 Diagnostic Analytics
Phân tích chuyên sâu, nâng cao phần analytic model và visualize kết hợp với story telling, chủ yếu tập trung diagnostic analytics, phân tích bằng so sánh nhiều nguồn dữ liệu vs nhau coi nó có mối liên hệ nào, ẩn giấu quy luật gì, phân tích nguyên nhân kết quả, so sánh kết hợp các vấn đề liên quan.
- Tools: Tableau, PBI, Google Data Studio, SQL
- Concepts: Analytics model, domain knowledge, quantitative analytics & qualitative analytics, Root cause analysis , DAX
- Embedded Analytics , Realtime dashboard , Analytics Cloud Service , Data Model Optimizing
Các câu hỏi đặt ra ở LV2 nó sẽ phức tạp, , vĩ mô , cần có thời gian nghiên cứu, so sánh, kết hợp nhiều nguồn dữ liệu để tìm câu trả lời. Thường phải đặt ra giả thuyết (hypothesis) và tìm câu trả lời bằng dữ liệu để rút ra kết luận phù hợp.

Khi đó là “play with data”, data mining. Thường các công ty lớn Viettel, FPT, Momo , Zalo mới làm kiểu này, các công ty nhỏ thường không có nhu cầu giải quyết các bài toán phức tạp như vậy.

Ví dụ : Phân nhóm khách hàng trong tập khách hàng hiện tại thành các nhóm tiềm năng để care , tìm insights của các nhóm ( Bài Toán CRM )  , phân tích nguyên nhân dẫn đến retention rate của nhân viên , tìm insights dẫn đến retention rate ( HR  ) , Phân tích traffic performance , tìm ra insights , mỗi quan hệ giữa các channel ( SEO Analytics ) 

⇒ Câu hỏi nó không phải dễ trả lời ngay như lv1 , cần phải nghiên cứu , so sánh , kết hợp nhiều kết quả thống kê.


### Level 3 Predictive Analytics
Phân tích dự đoán
- Tools: 100% bằng Python
- Concepts: higher-level stats, Data Science Math, Machine Learning, text mining, ETL data ( basic Data Engineer)
- Làm các task có độ technical advanced
  
Example 1: Tới mùa World Cup, FPT cần dự đoán bao nhiêu người sẽ truy cập xem theo các rounds để chuẩn bị băng thông cho đủ. Băng thông ít gây giật lag, khách hàng bỏ đi, hủy dịch vụ. Băng thông nhiều thì vượt ngân sách, lỗ. Tất cả cần chứng minh (dự đoán) trước bằng data, toán, lập trình cho máy tính. ( Time series analytics ) 

Example 2: sales vs marketing kéo đc 1 tập 100k khách hàng , giờ chia ra thành nhóm (clustering ), thành bao nhiêu nhóm để team sale care cho hiệu quả. Lập trình cho máy tính chia. 

Example 3: Phân tích coi 100k comments của khách hàng tương tác trong một campaign nhất định ( NLP )

Example 4: Crawl data online rồi build 1 pipeline bắn data realtime, và thiết kế dashboard in realtime ( Streaming analytics )
