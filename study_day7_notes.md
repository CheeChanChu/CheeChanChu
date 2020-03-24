# CheeChanChu
记录我的程序生涯点点滴滴
#study_day7_notes
一.盒模型
    margin:;
    1.margin长在元素之外的
    2.margin控制的是元素与同级元素之间的位置关系
    3.margin不会对盒子本身的宽高造成影响
    4.给单一方向添加margin值    margin-left/right/top/bottom
    5.margin的设置方法: 与(padding的方式一样 )
    6.margin可以设置负值
    7.margin常出现的bug
        a: 当父元素和子元素 都没有设置浮动的情况,如果给第一个子元素添加margin-top   
           会错误把margin-top 加载父元素上面.但是左右不会
        b: 上下相邻两个元素之间的margin值 不会叠加,按照最大值来添加(左右没有问题)

    8.margin:0 auto;  让当前元素左右居中

二.网页部署
    规划:
        元素命名:
            id划分外围结构      ->      id选用驼峰式命名或者语义化
            class版心命名       ->      用连字符命名    (news-l)
            内部内容块命名      ->      下划线      (news_r)

            css外部样式表
                1.每个页面都需要属于自己的样式表     (index.css)
                2.一个网站都拥有公共样式表          (public.css)
                3.重置样式的样式表                  (reset.css)

            注意:如果版心两侧没有颜色平铺,可以直接写版心的样式!!!
            另外,如果单行文字上下误差通过   line-height:根据行高而定;   设置等于文字大小即可.
