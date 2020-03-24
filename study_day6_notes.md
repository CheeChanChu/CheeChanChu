# CheeChanChu
记录我的程序生涯点点滴滴
#study_day6
一.浮动
    属性:float:;
    属性值: left   ,    right   ,   none    

    注意:只要元素右浮动,父元素必须添加高度,否则会出现bug(父元素塌陷,但是后面学习定位的时候会修复这个bug)


二.页面布局2.0
    1.设计图:
        版式宽度一般为  1920px  1680px....
        网页的版心: 900-1200px

    2.结构规划:
        a.id名称:网页外围结构 100%
        b.pc端版心宽度不用百分比
        c.让版心左右居中,添加   margin:0 auto;

三.css列表属性.         (在html中,列表属性右,ul,ol,dl,无序,有序,自定义列表)
    1.属性: list-style-type:;  常用none（清除列表符号）
        属性值:  square（方）   cir（圆）    none（常用）
    
    2.list-style-image:;    (把一张图片当作列表)
    3.list-style-position:;     
                inside    (内容区域里面)
                outside   (内容区域外面)
    4.list-style:;   none（常用）  也是重点!!!


四.css边框属性.          border:10px solid red;   (边框线为10px的红色)
    Q1:边框长在那里??
    A:边框在元素的高度之外

    border:10px solid red; （简写\复合式写法）
        
    border-width:10px;
    border-style:solid;
    border-color:red;

    常用线条类型: solid(实线)   dashed(虚线)    dotted(点状线)
                 double(双线)  none(没有线条,清除线条)
                 transparent(颜色透明)

    Q2:给单一方向添加线条边框
        border-left:10px solid red;     左
        border-right:;                  右
        border-top:;                    上
        border-bottom:;                 底

    4.border-width:;  border-style:;  border-color
        a.这三个属性可以单独进行设置。
        b.最多能接收4个属性值

        eg:border: 10px solid
           border-color: ;  (1~4个属性值)
           当1个属性值的时候,代表四周都有颜色
           2个属性值的时候: 上下    左右
           3个属性值的时候: 上  左右  下
           4个属性值的时候: 上  右  下  左

    5.用css实现一个三角形
        颜色值为透明: transparent


五.背景         background:;            复合属性(可以通过简写进行)
            简写顺序(颜色,背景图,是否铺平,位置)
            1.背景颜色:
                background-color:;
            2.背景图:
                background-image:url(路径)
                背景图显示状态:
                a:背景图不占据空间
                b:背景图大小小于容器大小时候,平铺到满为止
                    等于的时候正好显示一张
                    大于的时候显示一部分

            3.控制背景图是否平铺
                background-repeat:;
                    属性值：     repeat      平铺
                                no-repeat   不平铺
                                repeat-x    横向平铺
                                repeat-y    纵向平铺
            4.控制背景图的位置:
                background-position:;
                    属性值:
                        水平的位置(x轴) 和 垂直的位置(y轴)
                        eg:left bottom      (左下角对齐)

            5.背景图的固定
                background-attachment:;
                    属性值: fixed/scroll

            6.背景图 与 html的 images的差别
                背景图:网页渲染,不占据空间
                img:html的结构,占据空间

                Q:什么时候用img,什么时候用背景图呢?
                    网页上看到的大图,都是用img导入的,小图标等是用css样式导入


六.盒模型
    css盒模型:  是王爷布局的基石!从里到外包括什么呢?
            内容区  ->  填充区  ->  盒子边框    ->  外边距
          (content)   (padding)    (border)      (margin)

          A.padding的用法
            1.padding是长在内容和盒子之间的,在盒子内部
            2.padding是为了调整  子元素  和  父元素 里面位置关系
            3.padding的特点:    padding 会把盒子撑大
            4.如果想让盒子保持原来大小,需要宽高的基础上-padding值才可以
            5.给单一方向设置判定值
                padding-left/right/top/bottom
            6.padding   设置方法:
                padding:一个值      (四周都有表现)
                        两个值      (上下,左右)
                        三个值      (上,左右,下)
                        四个值      (上,右,下,左)

            7.padding   不能设置负值
            8.padding   不会对背景图造成影响
            9.如果一个盒子没有设置固定的宽高,添加padding是不用减的
