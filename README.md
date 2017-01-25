# ColorDocument v0.9.1 Beta
=================================================

>    本工具用来集中管理项目中LESS/SASS样式文件内容的颜色值，使用本工具可以
>将样式文件中的颜色值转换为引用统一颜色字典的易维护颜色的文件。
>    注意：请不要在LESS样式文件中使用相似十六进制的元素ID标识，例如
>#f-e-8、#a669、#abc等。为避免相似元素ID标识可以以下划线开头(#_fc、#_
>abc)。

* 环境要求：
    NodeJS v6.3.0
    NodeJS bower
    NodeJS express (可以用其它web host代替)


* 如何对项目进行颜色字典化处理：

1.创建配置启动文件(例：runColorDict.js);

2.备份项目的文件，以便在工具处理异常时恢复;

3.在命令行或git-bash中运行 node runColorDict.js

4.在所有项目样式文件中引入字典变量文件;

5.验证结果是否符合预期


* 如何以文档形式查看字典信息：

1.更新colorDoc文件夹下的config.json中的字典路径

2.运行start.js(需要安装express);

3.打开浏览器，访问：127.0.0.1:1166/colorDoc.html