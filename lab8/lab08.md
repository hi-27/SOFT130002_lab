### 轮播
因为HTML里面直接是图片就没有弄images的文件夹。
为了让左右键按了有反应，添加了onclick。
还改了一点css，文字居中之类的。
有5个全局变量，其中3个用来获取dom元素，分别是container wrap和buttons下的span。另外两个是计时器和计数。
#### 第一部分
向右的箭头right()
先获取left的数值，判断是否处于5的位置，如果不在，就直接减600，获得目标位置记为变量x。如果是5，即此时left为-3600px，则将其目标位
置调为-1200px。
做了一个平移的动画，设置timer1作为临时的计时器，每5毫秒将现有的left数值减少3（1实在太慢了），直到达到目标位置x，停止计时器timer。
用来计数的count每调一次函数就加加一次，如果超过4就返回0。
函数showList()用来显示右下角的图标。首先，把所有span的class都去掉，再把count位调class命名为on，使它获得不同的css样式。
向左的箭头同理。
#### 第二部分
设定全局变量timer为每2000毫秒执行一次right()函数的计数器。
如果container onmouseover则清除timer，onmouseout则重新开始timer计时。
#### 第三部分
通过遍历，来获取被点击的span。改变left的值为，使图片跳转，其中为了让后面的图片动画顺利衔接，若span为5那么left为0，其余为-(span
-1)*600。
### 表格
在table上加了一个onclick函数，获取被点击的元素。判断元素是否为td，如果是则创建一个新的元素input，设置type为text，value为td中的
内容。将td中原有的内容删除，添加新元素input，使input被focus，且选中(0，0)位置，使光标出现在内容前面。当input被onblur时，将它的
value填入td中，再将其remove。

