# Oracle
# 实验三：创建分区表
## 实验目的：<br>
掌握分区表的创建方法，掌握各种分区方式的使用场景。<br>
## 实验内容：<br>
本实验使用3个表空间：USERS,USERS02,USERS03。在表空间中创建两张表：订单表(orders)与订单详表(order_details)。<br>
使用你自己的账号创建本实验的表，表创建在上述3个分区，自定义分区策略。<br>
你需要使用system用户给你自己的账号分配上述分区的使用权限。你需要使用system用户给你的用户分配可以查询执行计划的权限。<br>
表创建成功后，插入数据，数据能并平均分布到各个分区。每个表的数据都应该大于1万行，对表进行联合查询。<br>
写出插入数据的语句和查询数据的语句，并分析语句的执行计划。<br>
进行分区与不分区的对比实验。<br>
![](https://github.com/Litianweii/Oracle/blob/master/test3/1.png) <br>
![](https://github.com/Litianweii/Oracle/blob/master/test3/2.png) <br>
![](https://github.com/Litianweii/Oracle/blob/master/test3/3.png) <br>
![](https://github.com/Litianweii/Oracle/blob/master/test3/4.png) <br>
![](https://github.com/Litianweii/Oracle/blob/master/test3/5.png) <br>
![](https://github.com/Litianweii/Oracle/blob/master/test3/6.png) <br>

## 区别
增加了三个逻辑表分区，在查询的时候就不用查询整张表，而是根据分区来查询，这样就会更省时间
