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
