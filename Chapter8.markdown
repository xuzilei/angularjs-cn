#备忘与诀窍

目前为止，之前的章节已经覆盖了Angular所有功能结构中的大多数，包括指令,服务,控制器,资源以及其它内容.但是我们知道有时候仅仅阅读是不够的.有时候，我们并不在乎那些功能机制是如果运行的,我们仅仅想知道如何用AngularJS去做实现一个具体功能。

在这一章中，我么视图给出完整的样例代码,并且对这些样例代码仅仅给出少量的信息和解释，这些代码解决是我们在大多数Web应用中碰到的通用问题.这些代码没有具体的先后次序,你尽可以跳到你关心的小节先睹为快或者按着本书内容顺序阅读,选那种阅读方式由你决定.

这一章中我们将要给出代码样例包括以下这些：

1、封装一个jQuery日期选择器(DatePicker)
2、团队成员列表应用:过滤器和控制器之间的通信
3、AngularJS中的文件上传
4、使用socket.IO
5、一个简单的分页服务.
6、与服务器后端的协作

##封装一个jQuery日期选择器

这个样例代码文件可以在我们GitHub页面的chatper8/datepicker目录中找到.

在我们开始实际代码之前，我们不得不做出一个设计决策：我们的这个组件的外观显示和交互设计应该是什么样子,假设我们想定义的的日期选择器在HTML里面使用像以下代码这样:

    <input datepicker ng-model="currentDate" select="updateMyText(date)" ></input>




