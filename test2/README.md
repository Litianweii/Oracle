# 实验内容：<br>
Oracle有一个开发者角色resource，可以创建表、过程、触发器等对象，但是不能创建视图。本训练要求：<br>

在pdborcl插接式数据中创建一个新的本地角色con_res_view，该角色包含connect和resource角色，同时也包含CREATE VIEW权限，这样任何拥有con_res_view的用户就同时拥有这三种权限。
创建角色之后，再创建用户new_user，给用户分配表空间，设置限额为50M，授予con_res_view角色。
最后测试：用新用户new_user连接数据库、创建表，插入数据，创建视图，查询表和视图的数据。<br>
![](https://github.com/Litianweii/Oracle/blob/master/test2/20181029150454.png)<br>
![](https://github.com/Litianweii/Oracle/blob/master/test2/20181029150946.png)<br>
![](https://github.com/Litianweii/Oracle/blob/master/test2/20181029151036.png)<br>
![](https://github.com/Litianweii/Oracle/blob/master/test2/20181029151125.png)<br>
