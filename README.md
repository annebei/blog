# 角落  
`人如果没有梦想`    
`那和咸鱼有什么区别`


****
## 目录
* [JAVA](#)    
    * JAVA基础    
    * STRUTS    
    * SPRING    
* [数据库](#)
* [前端](#)    
    * Javascript    
    * Jquery    
* [中间件](#)    
    * Weblogic    
    * Tomcat    
* [Axure](#)

### 横线
-----------
***、---、___可以显示横线效果

***
---
___



标题
------

# 一级标题  
## 二级标题  
### 三级标题  
#### 四级标题  
##### 五级标题  
###### 六级标题  


文本
------
### 普通文本
这是一段普通的文本
### 单行文本
            Hello。    
在一行开头加入1个Tab或者4个空格。
### 文本块
#### 语法1
在连续几行的文本开头加入1个Tab或者4个空格。

    欢迎到访
    很高兴见到您
    祝您，早上好，中午好，下午好，晚安

#### 语法2
使用一对各三个的反引号：
```
欢迎到访
人如果没有梦想    
那和咸鱼有什么区别
```
该语法也可以实现代码高亮，见[代码高亮](#代码高亮)
### 文字高亮
文字高亮功能能使行内部分文字高亮，使用一对反引号。
语法：
```
`linux` `网络编程` `socket` `epoll` 
```
效果：`linux` `网络编程` `socket` `epoll`

也适合做一篇文章的tag
#### 换行
直接回车不能换行，  
可以在上一行文本后面补两个空格，  
这样下一行的文本就换行了。

或者就是在两行文本直接加一个空行。

也能实现换行效果，不过这个行间距有点大。
#### 斜体、粗体、删除线

|语法|效果|
|----|-----|
|`*斜体1*`|*斜体1*|
|`_斜体2_`| _斜体2_|
|`**粗体1**`|**粗体1**|
|`__粗体2__`|__粗体2__|
|`这是一个 ~~删除线~~`|这是一个 ~~删除线~~|
|`***斜粗体1***`|***斜粗体1***|
|`___斜粗体2___`|___斜粗体2___|
|`***~~斜粗体删除线1~~***`|***~~斜粗体删除线1~~***|
|`~~***斜粗体删除线2***~~`|~~***斜粗体删除线2***~~|

    斜体、粗体、删除线可混合使用

图片
------
基本格式：
```
![alt](URL title)
```
alt和title即对应HTML中的alt和title属性（都可省略）：
- alt表示图片显示失败时的替换文本
- title表示鼠标悬停在图片时的显示文本（注意这里要加引号）

URL即图片的url地址，如果引用本仓库中的图片，直接使用**相对路径**就可了，如果引用其他github仓库中的图片要注意格式，即：`仓库地址/raw/分支名/图片路径`，如：
```
https://github.com/annebei/blog/image/foryou.jpg
```

|#|语法|效果|
|---|---|----
|1|`![baidu](http://www.baidu.com/img/bdlogo.gif "百度logo")`|![baidu](http://www.baidu.com/img/bdlogo.gif "百度logo")
|2|`![][foryou]`|![][foryou]

注意例2的写法使用了**URL标识符**的形式，在[链接](#链接)一节有介绍。
>在文末有foryou的定义：
```
[foryou]:https://github.com/annebei/blog/image/foryou.jpg
```

代码高亮
----------
在三个反引号后面加上编程语言的名字，另起一行开始写代码，最后一行再加上三个反引号。
```Java
public static void main(String[]args){} //Java
```
```c
int main(int argc, char *argv[]) //C
```
```Bash
echo "hello GitHub" #Bash
```
```javascript
document.getElementById("myH1").innerHTML="Welcome to my Homepage"; //javascipt
```
```cpp
string &operator+(const string& A,const string& B) //cpp
```
表格
--------

表头1  | 表头2|
--------- | --------|
表格单元  | 表格单元 |
表格单元  | 表格单元 |

| 表头1  | 表头2|
| ---------- | -----------|
| 表格单元   | 表格单元   |
| 表格单元   | 表格单元   |

### 对齐
表格可以指定对齐方式

| 左对齐 | 居中  | 右对齐 |
| :------------ |:---------------:| -----:|
| col 3 is      | some wordy text | $1600 |
| col 2 is      | centered        |   $12 |
| zebra stripes | are neat        |    $1 |

### 混合其他语法
表格单元中的内容可以和其他大多数GFM语法配合使用，如：  
#### 使用普通文本的删除线，斜体等效果

| 名字 | 描述 |
| ------------- | ----------- |
| Help      | ~~Display the~~ help window.|
| Close     | _Closes_ a window     |

#### 表格中嵌入图片（链接）
其实前面介绍图片显示、图片链接的时候为了清晰就是放在在表格中显示的。

| 图片 | 描述 |
| ---- | ---- |
|![baidu][baidu-logo] | 百度|

表情
----------
Github的Markdown语法支持添加emoji表情，输入不同的符号码（两个冒号包围的字符）可以显示出不同的表情。

比如`:blush:`，可以显示:blush:。

具体每一个表情的符号码，可以查询GitHub的官方网页[http://www.emoji-cheat-sheet.com](http://www.emoji-cheat-sheet.com)。

diff语法
---------
版本控制的系统中都少不了diff的功能，即展示一个文件内容的增加与删除。
GFM中可以显示的展示diff效果。使用绿色表示新增，红色表示删除。

其语法与代码高亮类似，只是在三个反引号后面写diff，
并且其内容中，以 `+ `开头表示新增，`- `开头表示删除。

效果如下：

```diff
+ 明月林间照，清泉石上流
- 明月松间照，清泉石上流
```






