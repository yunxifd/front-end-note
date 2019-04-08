css (cascading style sheet) 层叠样式表

## css选择器

css 基本语法
```
选择器 {
    属性1: 值;
    属性2: 值;
}
```
css 常用选择器 用于匹配html元素  

### 分类
- 元素选择器 body a div
- 伪元素选择器 ::before ::after
- 类选择器 .container .nav
- 属性选择器 [type=radio]
- 伪类选择器 :hover
- id选择器 #id
- 组合选择器 div+a [type=checkbox]+label
- 否定选择器 :not(.link)
- 通用选择器 *

参考 http://www.w3school.com.cn/cssref/css_selectors.asp

#### 伪元素 与 伪类的区别？  
伪元素 是虽在在 html和dom中不存在，但是在界面上是真实存在的   
伪类 表示一种状态  

### 选择器权重

- ID选择器 100
- 类 属性 伪类 10
- 元素 伪元素 1
- 其他选择器 0

> 不进位计算 10个类选择器的优先级也没有一个ID选择器的优先级高

其他影响选择器权重的因素

- `!important` 优先级最高
- 内联样式 优先级高
- 相同权重 后写的生效

### 解析方式
浏览器解析css选择器的方式是 **从右向左**的

以下面css代码为例
```css
body div a {
    color: red;
}
```

```
a div body
```

## 非布局样式

### 字体
- 字体族 

    一系列字体的组合 不能用引号裹起来，代表一系列字体，当设置字体族的时候，会在其字体族中找一种字体来渲染，不能保重用哪种字体
- 多字体 fallback

    可以设置多种字体，如果第一个字体找不到，就匹配第二种字体 ，以此类推

- 网络字体、自定义字体
- iconfont 原理就是 自定义字体
    
> 字体 可以用引号裹起来，字体族 不能用引号裹起来

### 行高

参考 https://www.jianshu.com/p/fd42b7491b79

inline元素 默认是以基线对其的; 

图片下面出现`3px`间距解决方法？  
- 设置成 display:block;
- 调整对其方式 vertical-align: bottom;

### 背景

- 背景颜色
- 渐变色北京
- 多背景叠加
- 背景图片和属性 雪碧图
- base64 
- 多分辨率适配


雪碧图的作用？
- 减少http请求数量
- 加速网页内容显示

base64图片，虽然减少了http请求数，但是
- 增大了css文件大小
- 增加了解析图片的开销

### 边框

- 线型 大小 颜色
- 边框背景图
- 边框衔接 三角形

### 滚动条

### 文字折行

- overflow-wrap 通用换行控制 
- word-break 支队多字节文字
- white-sapce 空白处是否断行
