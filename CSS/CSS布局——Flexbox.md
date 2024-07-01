<a name="ItXMA"></a>
### 基础概念
<a name="p4Qsg"></a>
#### Flexbox布局的概念
Flexbox布局是一种布局的模式，用来在一个维度上为项目设置布局
<a name="amxio"></a>
#### 容器
在HTML中大多数元素例如`div`、`ul`、`main`块元素，`span`、`em`、`i`行内元素都可以作为Flex容器，它的作用是开启一个Flex布局模式，你只需要在元素上面设置`display: flex`即可开启一个Flex布局容器。
<a name="sF6cG"></a>
#### 项目
当开启一个Flex布局的时候，容器中的一个个元素`::before`、`::after`、文本、dom元素就是项目，这些项目是容器的子元素，他们之间是父子关系，子元素也可以开启自己独立的Flex布局，他不会继承父元素的flex属性。
```html
<div class="container">
  <div>1</div>
  <div>1</div>
  <div>1</div>
  <div>1</div>
</div>
<!-- 开启Flex布局 -->
.container {
  display: flex; 
  width: 300px;
  height: 200px;
  background-color: #8a8282;
}
```
<a name="QNv7u"></a>
#### 主轴、侧轴
在Flex中容器有两个轴分别是**主轴**和**侧轴**，默认情况下主轴沿着行的方向分布，侧轴沿着列的方向分布。有一点需要注意，主轴和侧轴的方向并不是固定不变的而是要受到`flex-direction`和`writing-mode`或者`direction `阅读模式的影响
<a name="YexfD"></a>
#### 容器大小：主轴尺寸、侧轴尺寸
Flex容器的大小是由主轴尺寸或者侧轴尺寸决定的，主轴的尺寸：主轴开始位置到主轴结束位置的距离，侧抽尺寸：侧轴的开始位置到侧轴的结束位置的距离。
<a name="bCFhP"></a>
#### flex-direction控制项目的方向
flex-direction属性用来控制主轴上项目的排布方向，默认是`row`即按照行内的方式在一行排列，如果想让元素按照块的方式在一列显示则可以设置`flex-direction: column``row-reverse`和`column-reverse`可以使主轴（或者侧轴）的起点和终点位置互换<br />![](https://cdn.nlark.com/yuque/0/2023/jpeg/36013995/1701876085791-876abe46-b21a-4b47-be90-d4dcec4ae530.jpeg)<br />![image.png](https://cdn.nlark.com/yuque/0/2023/png/36013995/1701924852577-9fd51c69-e6a2-43d7-9f20-2e8a531c50cc.png#averageHue=%23e0f6e7&clientId=u9ff1f43e-0e68-4&from=paste&height=229&id=u2c838227&originHeight=229&originWidth=486&originalType=binary&ratio=1&rotation=0&showTitle=false&size=8912&status=done&style=none&taskId=ubc541e98-468e-4927-9550-7815c35a3d7&title=&width=486)<br />![image.png](https://cdn.nlark.com/yuque/0/2023/png/36013995/1701925070945-a55acf8e-fb22-4277-8bf3-64bd14eab1a6.png#averageHue=%23fbdcc8&clientId=u9ff1f43e-0e68-4&from=paste&height=394&id=ud931396b&originHeight=394&originWidth=435&originalType=binary&ratio=1&rotation=0&showTitle=false&size=10648&status=done&style=none&taskId=ua892181a-6ff8-4341-8023-7830dae8da5&title=&width=435)<br />flex-wrap控制项目换行<br />order 项目排序<br />gap项目之间的间距
