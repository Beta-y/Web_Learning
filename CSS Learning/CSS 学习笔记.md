1.层次样式表(Cascading Style Sheets,CSS)

    用于美化网页，做到结构 (HTML) 和表现 (CSS)分离。

2.CSS 引用方式（使用见 class_1）

    (1) 行间样式：直接在标签上书写

    (2) 内部样式：在 html 文件的 <head> 部分写出

    (3) 外部样式(link)：先创建一个 CSS 文件，然后在 html 文件的<head> 中使用 <link> 引入该文件

    (4) 导入外部样式(import)：先创建一个 CSS 文件，然后在 html 文件的<head> 中 style 属性中用 @import 导入该样式文件，并且必须放在 style 内的最前面

    link 和 @import 导入外部样式的区别（link 更好）：
        1. 1ink 引用CSs时，在页面载入时同时加载；@import 需要页面网页完全载入以后加载。
        2. 1ink 支持使用 Javascript 控制 DOM 去改变样式；而 @import 不支持。
        3.1ink 是 XHTML 标签，除了加载 CSS 外，还可以定义 RSS 等其他事务；@import 属于 CSS 范畴，只能加载 CSS。
        4.1ink 是 XHTML 标签，无兼容问题；@import 是在 CSS2.1 提出的，低版本的浏览器不支持。

3.基本语法规则（使用见 class_2）

    选择器 {
        属性: 属性  值;
    }

    选择器分类：
    1) * ：匹配所有元素，运行效率极低，不建议使用
    2) 标签选择器：用 标签名 来进行匹配
    3) 类选择器： 用class属性来进行匹配
    4) id 选择器：用 id 属性来进行匹配，优先级高于 class，且具有唯一性(一个id只能出现一次)
    5) 派生选择器：在基本选择器后再添加额外派生标签来进行匹配
    6) 伪类选择器：后面学
