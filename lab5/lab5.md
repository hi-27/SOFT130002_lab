### 设计文档
#### 第一部分
获取url的value；使用RegExp进行匹配；在url_result中填入参数值。<br>
RegExp的正则匹配，尝试了很多种，但是总还是有等号留着，后来用substr把等号去掉了。
#### 第二部分
在mouse over时在mul中填入初始值1，新建date，使用getSecond获取当前时间的秒数。根据大小判断使用哪一种方案。<br>
if else语句分别使用setInterval来完成梅5妙进行value值的翻倍。<br>
完成之后clearInterval停下value翻倍。
#### 第三部分
获取输入的字符串，用split将字符串拆开。在找到0号位置的字母，与后面的字母比对，count计数。<br>
完成之后，将字符串中第一个字母全部去掉，形成新的字符串。<br>
重复以上行为，直到字符串为空。<br>
将每一个字母和它的count分别计入数组。<br>
找出数组中数字最大的和它的index，到字符数组中找出字母。<br>
填入result的value。<br>
提交截图：<br>
![img](image/提交.jpg)
网页效果截图：<br>
![img](image/网页效果.jpg)
