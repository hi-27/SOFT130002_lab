#### cookie的作用
cookie是客户端浏览器用来记录用户信息从而实现客户端与服务器之间状态的保持，分为回话cookie和持久cookie两种。前者随着浏览器的关闭自
动销毁，而后者可以通过设置expire time来设定cookie留存的时长，此时cookie不会随着浏览器的关闭晓东销毁。
#### cookie的优缺点
优点：保存在客户端所以不需要服务器资源；有效时长可自定义。<br>
缺点：大小受到限制；可能被修改，不安全；有些浏览器不适用；需要字符串解析；速度慢。<br>
#### session的作用
作用和cookie基本一致，但是他的信息是存储在服务器的，但是会通过cookie将一个session_id发送到客户端。同时，session无法设置有效时长，
只能随着浏览器关闭销毁。
#### session的优缺点
优点：信息存在服务器，相对更加安全；可以存在内存和文件中，不容易丢失。<br>
缺点：无法自定义有效时长；难以起到负载均衡效果；可能会发生单点故障。<br>