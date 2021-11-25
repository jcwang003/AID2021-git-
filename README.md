## Markdown 语法的简要规则

### 标题

​	标题是每篇文章都需要也是最常用的格式，在 Markdown 中，如果一段文字被定义为标题，只要在这段文字前加 `#` 号即可。

​	`# 一级标题`

​	`## 二级标题`

​	`### 三级标题`

​	以此类推，总共六级标题，建议在井号后加一个空格，这是最标准的 Markdown 语法。

### 列表

​	熟悉 HTML 的同学肯定知道有序列表与无序列表的区别，在 Markdown 下，列表的显示只需要在文字前加上 `-` 或 `*` 即可变为无序列表，有序列表则直接在文字前加 `1.``2.``3.` 符号要和文字之间加上一个字符的空格。

​	![img](https://cdn.sspai.com/attachment/origin/2014/04/15/69493.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1)

### 引用

​	如果你需要引用一小段别处的句子，那么就要用引用的格式。

​	`> 例如这样`

​	只需要在文本前加入 `>` 这种尖括号（大于号）即可

​	![img](https://cdn.sspai.com/attachment/origin/2014/04/15/69494.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1)

### 图片与链接

​	插入链接与插入图片的语法很像，区别在一个 `!`号

​	插入图片的地址需要图床，这里推荐 [CloudApp](http://www.getcloudapp.com) 的服务，生成URL地址即可。

​	![img](https://cdn.sspai.com/attachment/origin/2014/04/15/69495.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1)

### 粗体与斜体

​	Markdown 的粗体和斜体也非常简单，用两个 `*` 包含一段文本就是粗体的语法，用一个 `*` 包含一段文本就是斜体的语法。

​	例如：**这里是粗体***这里是斜体*

### 表格

​	表格是我觉得 Markdown 比较累人的地方，例子如下：

```
	| Tables        | Are           | Cool  |
	| ------------- |:-------------:| -----:|
	| col 3 is      | right-aligned | $1600 |
	| col 2 is      | centered      |   $12 |
	| zebra stripes | are neat      |    $1 |
```

​	这种语法生成的表格如下：

| Tables        | Are           | Cool  |
| ------------- | ------------- | ----- |
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      | $12   |
| zebra stripes | are neat      | $1    |

### 代码框

​	如果你是个程序猿，需要在文章里优雅的引用代码框，在 Markdown 下实现也非常简单，只需要用两个 ` 把中间的代码包裹起来，如 ``code``。图例：

​	![img](https://cdn.sspai.com/attachment/origin/2014/04/15/69496.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1)

​	使用 `tab` 键即可缩进。

### 分割线

​	分割线的语法只需要另起一行，连续输入三个星号 `***` 即可。

### 小结

​	到这里，Markdown  的基本语法在日常的使用中基本就没什么大问题了，只要多加练习，配合好用的工具，写起东西来肯定会行云流水。更多的语法规则，其实 Mou 的 Help 文档例子很好，当你第一次使用 Mou 时，就会显示该文档，其次，你也可在撰写过程中，使用 `CMD+R` 快捷键来快速打开文档，以随时查阅和学习语法。

图灵社区发帖采用的是流行的Markdown语法，本文可供快速入门。

------

### 代码

```
单个回车
视为空格。

连续回车

才能分段。

行尾加两个空格，这里->  
即可段内换行。

*这些文字显示为斜体*

**这些文字显示为粗体**
```

### 效果

单个回车 视为空格。

连续回车

才能分段。

行尾加两个空格，这里->  
 即可段内换行。

*这些文字显示为斜体*

**这些文字显示为粗体**

------

### 代码

```
行的开头空4个空格，表示程序代码，例如：

C#:

    //这里显示一些代码，在正文显示中会自动识别语言，进行代码染色，这是一段C#代码
    public class Blog
    {
         public int Id { get; set; }
         public string Subject { get; set; }
    }

Python:

    keywords = ["dsaa","Asd","sadc","Gdfd","gdfdd","gaf","gabdddddd","eg"]
    print dict([(i[0],list(i[1])) for i in groupby(sorted(keywords),lambda    x:x[0].lower())])

Javascript:

    /**
     * nth element in the fibonacci series.
     * @param n >= 0
     * @return the nth element, >= 0.
     */
    function fib(n) {
        var a = 1, b = 1;
        var tmp;
        while (--n >= 0) {
            tmp = a;
            a += b;
           b = tmp;
        }
        return a;
    }

    document.write(fib(10));
```

### 效果

行的开头空4个空格，表示程序代码，例如：

C#:

```
//这里显示一些代码，在正文显示中会自动识别语言，进行代码染色，这是一段C#代码
public class Blog
{
     public int Id { get; set; }
     public string Subject { get; set; }
}
```

Python:

```
keywords = ["dsaa","Asd","sadc","Gdfd","gdfdd","gaf","gabdddddd","eg"]
print dict([(i[0],list(i[1])) for i in groupby(sorted(keywords),lambda    x:x[0].lower())])
```

Javascript:

```
/**
 * nth element in the fibonacci series.
 * @param n >= 0
 * @return the nth element, >= 0.
 */
function fib(n) {
    var a = 1, b = 1;
    var tmp;
    while (--n >= 0) {
        tmp = a;
        a += b;
       b = tmp;
    }
    return a;
}

document.write(fib(10));
```

------

### 代码

```
>表示引用文字内容。

#表示这是一级标题
##表示这是二级标题
###表示这是三级标题
……
###### 最小是六级标题

也可以这样表示大标题
=

这样表示小标题
-
```

### 效果

> 表示引用文字内容。

\#表示这是一级标题 ##表示这是二级标题 ###表示这是三级标题 ……

###### 最小是六级标题

# 也可以这样表示大标题

## 这样表示小标题

------

### 代码

```
---
上面是一条分隔线


- 这是无序列表项目
- 这是无序列表项目
- 这是无序列表项目

两个列表之间不能相邻，否则会解释为嵌套的列表

1. 这是有序列表项目
2. 这是有序列表项目
3. 这是有序列表项目

下面这个是嵌套的列表

- 外层列表项目
 + 内层列表项目
 + 内层无序列表项目
 + 内层列表项目
- 外层列表项目
```

### 效果

------

上面是一条分隔线

- 这是无序列表项目
- 这是无序列表项目
- 这是无序列表项目

两个列表之间不能相邻，否则会解释为嵌套的列表

1. 这是有序列表项目
2. 这是有序列表项目
3. 这是有序列表项目

下面这个是嵌套的列表

- 外层列表项目

- 内层列表项目
- 内层无序列表项目
- 内层列表项目

- 外层列表项目

------

### 代码

```
直接把一个URL显示为超级连接：

也可以这样：[图灵社区](http://www.ituring.com.cn)

图像和链接非常类似，区别在开头加一个惊叹号： ![这是一个Logo图像](http://www.turingbook.com/Content/img/Turing.Gif)

此外，还可以以索引方式把url都列在文章的最后，例如这样：

[图灵社区][1]
![图灵社区Logo][2]

[1]:http://www.ituring.com.cn
[2]:http://www.ituring.com.cn/Content/img/Turing.Gif
```

### 效果

直接把一个URL显示为超级连接：

也可以这样：[图灵社区](http://www.ituring.com.cn)

图像和链接非常类似，区别在开头加一个惊叹号： ![这是一个Logo图像](http://www.ituring.com.cn/Content/img/Turing.Gif)

此外，还可以以索引方式把url都列在文章的最后，例如这样：

[图灵社区](http://www.ituring.com.cn) ![图灵社区Logo][2]

------

### 进一步了解：

- [Markdown语法详解](https://www.ituring.com.cn/article/504)
- [Markdown之表格的处理](https://www.ituring.com.cn/article/3452)