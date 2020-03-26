# CheeChanChu
记录我的程序生涯点点滴滴
#study_day9_notes
一.元素类型
    css是显示对标签分类:
        块状元素
        内联元素        (行内元素)  (内联块元素)
        第三类：
                a:可变元素      （有争议点）
                b:行内块元素


        A.元素类型每个类型的特点:
            块状元素:
            1.在页面中以矩形区域显示
            2.自上而下排列,独占一行
            3.可以直接添加宽高
            4.一般情况下,作为其他元素或内容的容器

        B.内联元素特点:
            1.在页面中给最小单位也是矩形
            2.在一行内逐个排列
            3.不可以直接添加宽和高,大小有内容撑开
            4.内联元素也符合盒模型的规则,但是个别属性会出现问题
                (padding-top/bottom)
                (margin-top/bottom)
            5.内联元素在一行内排列的时候,之间有间距
                如何消除间距呢?
                    a:添加浮动
                    b:把结构写在一行        (span /span span /span span /span )
        
        C.可变元素
            根据上下文显示,来确定这个元素是块状元素还是内联元素
                eg: button 


        那么哪些标签属于块状元素,哪些是内联元素呢?

            A:块状元素
            div  ul   dl   from  li   h1-h6   hr   ol   p   等等

            B:内联元素
            a  b  br  i  em  input  label  span  strong  sup  sub
            u  等等


二.元素类型转换         (重点!)
        display:;   
        作用:检索或者设置元素生成盒模型类型

        常用属性:
            a:  display:    block;
                作用:将元素转成块状元素,拥有块状元素的特点
                补充:大部分块状元素默认的display的值为block
                        个别除外,比如table.  

            b:  display:    inline;
                作用:将元素转成内联元素,拥有内联元素的特点
                补充:大部分内联元素默认display的值是inline

            c:  display     none;
                作用:隐藏,不占空间
