# 请求参数和返回字段的类型声明





# scrollview结构

![image-20220722102531386](../typora-user-images/image-20220722102531386.png)



index页面的user_list类型

![image-20220722102648909](../typora-user-images/image-20220722102648909.png)





index

@change="changeChild"   改名	swichcurrentuser



给ui  问接不接受名称过长显示

解决方案：四个字：诸葛村夫，五个字：诸葛村…

![image-20220722103406458](../typora-user-images/image-20220722103406458.png)



ellipse 改在buyhistory   问ui能不能写死  不动态

![image-20220722103600671](../typora-user-images/image-20220722103600671.png)



把跳转的命名to……改为go……





exist多余结构删除

![image-20220722105453002](../typora-user-images/image-20220722105453002.png)



数据处理放在js中

过滤器处理

没返回就显示0或者过期

类型转为number

![image-20220722105949467](../typora-user-images/image-20220722105949467.png)







把分割线尽量变为边框

使用更少的dom实现更精简更合理的结构









在模板上少用数据处理，放在js过滤器中



进度条的处理

```js
(pkg_remaining_list[index].remainingTime /
 pkg_remaining_list[index].availableTime) *
    100
```







test命名未改

![image-20220722110726532](../typora-user-images/image-20220722110726532.png)









miss命名缺省页 包括class的miss   改为default

分别命名套餐和用户的缺省页

![image-20220722110854020](../typora-user-images/image-20220722110854020.png)











不要空盒子包裹空盒子











两边距离不一样，和ui沟通一下

可以用列表遍历渲染

![image-20220722111654695](../typora-user-images/image-20220722111654695.png)



![image-20220722111701716](../typora-user-images/image-20220722111701716.png)











scrollview放在allcombo外面

![image-20220722111929134](../typora-user-images/image-20220722111929134.png)















多余的

![image-20220722112505363](../typora-user-images/image-20220722112505363.png)

![image-20220722112450011](../typora-user-images/image-20220722112450011.png)











确定不同套餐的icon区分依据











多余的

![image-20220722112907672](../typora-user-images/image-20220722112907672.png)











js过滤器处理

![image-20220722113130273](../typora-user-images/image-20220722113130273.png)













多余

![image-20220722113709683](../typora-user-images/image-20220722113709683.png)







configmap多余的

![image-20220722114307604](../typora-user-images/image-20220722114307604.png)











调试分页的数据

![image-20220722114610067](../typora-user-images/image-20220722114610067.png)







删掉这种多余的参数

![image-20220722114736762](../typora-user-images/image-20220722114736762.png)







多余的，直接从当前用户上取

![image-20220722114834665](../typora-user-images/image-20220722114834665.png)









**确认下拉刷新，刷新什么具体内容**

下拉刷新和上拉加载更多函数里删除多余的操作、









删掉调试代码，打印代码。







删除currentkey  改名test2

![image-20220722115427347](../typora-user-images/image-20220722115427347.png)







tc删除 打印、注释删除

![image-20220722115604820](../typora-user-images/image-20220722115604820.png)







所有的页面跳转用到的事件传值，全部改为vuex

![image-20220722115650289](../typora-user-images/image-20220722115650289.png)











## 删除bankno…………





## 存储vuex没必要为了一条数据存储一整个数组再传index这种方式





## asc  awi 阻塞问题



​	







