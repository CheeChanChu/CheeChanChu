# CheeChanChu
记录我的程序生涯点点滴滴
 #2020.3.18 notes
一:表格
    作用:显示数据
    标签:<table></table>
        <tr></tr> 代表 行
        <td></td> 代表 列

    1:html表格属性
            width=""                宽
            height=""               高
            border=""               边框
            bordercolor=""          边框颜色
            cellspacing=""          相邻单元格边框间距
            cellpadding=""          内容距离边框的间距

        A:文本对齐方式
            align="X"               水平方式
                X= "left"(左)   "center"(中)    "right"(右)
            
            valign="x"              垂直水平方式(一般很少用)
                x= "top"(顶端)  "middle"(中间)  "bottom"(底部)

        B:单元格合并        (跨行,合并行,跨列,合并列)

          a:合并行  rowspan="合并单元格数量"
            合并列  colspan+"合并单元格数量"
            注:无论合并行或列,首先操作合并的都是行 td

        C:单元格内部合并
            有合并行和列的情况，都是先合并列，再合并行（方便操作代码）


二:表单基础     
    作用:收集用户数据
    1:  表单标签:   <form></form>
            属性:   action="url"                ("url"表示路径，传输方式)
                method="常用get/post"       
                name="表单名称"

    2:  表单控件:   
            标签:   <input>             (单标签)
            属性:   type=""             (值input生成的类型,通常显示输入框,空按钮,密码框等)
                    type="属性值"
                    if type 属性值为:<input type="text">         (输入框)   
                                    <input type="password">     (密码框)
                                    <input type="submit">       (提交按钮)
                                    <input type="reset">        (重置按钮)  (意思为当前表单恢复到初始状态)
                                    <input type="button">       (空按钮)    (称之为万能按钮,后续功能可以自己编写)
                    value=""            (根据type类型不同,作用也会不同)
                    maxlength=""        (输入字符最大长度)
                    name=""             (当前表单名称)
                    size=""             (以字符为单位的,控制表单元素大小)

三:css基础  (层叠样式表)    最新版本为css3.0  所以很多时候也会显示 html+css3.0
    作用:渲染网页

    Q1:什么是样式表?
    A:一种将网页的内容和表示分离的网页设计形式

    Q2:为什么要用css来做呢?
    A:相比html操作元素的样式更加便利,功能性强大,有利于维护,也有利于结构和表现得分离
    
    1.css语法
        选择符{属性:属性值;}
        注:所有css都要放在css样式表里面!

    2.css语法说明:
        a.选择符选择得都是html的标签
        b.所有的css声明都要放在大括号 {} 里面
        c.css要有属性和属性值
        d.属性和属性值之间要用冒号 : 进行链接
        e.每条声明的最后必须加入分号 ; 结束
        f.如果一个属性有多个属性值时,属性与属性值要用空格 隔开

四:css样式表    /*  css的注悉方式  */
    A:内部样式表            （尽量放在head描述区里面）
        标签：<style></style>

    B:外部样式表             (创建一个后缀名为.css文件)
        a.外部样式表的导入
        第一种方法
            <link rel="stylesheet" href="url">
                 rel="stylesheet"   (建立关联性)
                 hrel="url"         (链接路径)
                 
        第二种方法
            <style>
                @import url("./css/text.css")   (括号里面显示的就是相对路径跟超链接内容相符合)
            </style>
    #补充说明下,    link外部导入方式 和 @import区别
            1:本质上区别:
                link 是属于 html的一个标签
                @import 是css提供的方式
            
            2:加载顺序:
                link导入的css 和 html结构同时加载
                @import 是先加载结构,后加载样式

            3:兼容性
                link兼容性相对会好很多
            
            4:js 操作 DOM样式的差别 (DOM表示标签和元素)
                if: 用 @import导入的css 是无法通过 js 做动态样式的修改的

    C:内联样式表             (行间样式,行内样式)
            语法:   <标签 style="内联样式"></标签>
            (这里大多是不会用到,但是除非项目特别紧急的情况下,为了方便直接渲染有时会用到) -->
