#Oracle<br>
=  实验一：分析SQL执行计划，执行SQL语句的优化指导<br>
-  实验内容：<br>
对Oracle12c中的HR人力资源管理系统中的表进行查询与分析。
首先运行和分析教材中的样例：本训练任务目的是查询两个部门('IT'和'Sales')的部门总人数和平均工资，以下两个查询的结果是一样的。但效率不相同。
设计自己的查询语句，并作相应的分析，查询语句不能太简单，<br>
- 教材中的查询语句<br>
查询一：
![](https://github.com/Litianweii/Oracle/blob/master/test1/_%5D7%7D0%40NKNQBIPP12N4%40W6%7B5.png)<br>
查询二：
![](https://github.com/Litianweii/Oracle/blob/master/test1/3XGZ%40BNZ%25XRM~%24E39L%24%40%5D3L.png)<br>
我认为查询一比查询二优，因为查询1除了“consistent gets=10”比查询二的“consistent gets=9”稍差，其他参数都优于查询二。从分析两个SQL语句可以看出，查询1是先过滤后汇总。参与汇总与计算的数据量少。而查询2是先汇总后过滤，参与汇总与计算的数据量多。<br>
 自定义查询语句：<br>
 查询所有工资大于8000的工作单位名称和职位<br>
![](https://github.com/Litianweii/Oracle/blob/master/test1/MPB8FZJXKFOM9S~T%7BE%40XU1K.png)
