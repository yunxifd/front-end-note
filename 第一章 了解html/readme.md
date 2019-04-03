## 常见 html 标签 及分类

参考：https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element

- html

  - head
    - title
    - meta 定义一些 元数据 用来描述 文档 ，详细使用参考 [meta](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/meta)
    - base
    - link
    - script
    - style
  - body

    - div /section/ article / aside / header /footer

      主要用来布局，但是 `div` 表意不明，没有语义

    - p 段落
    - span / em / strong
    - table / thead/ tbody / tr/ td 表格
    - ul/ ol/ li 无序/有序 列表
    - dl dt dd 定义列表
    - a 链接
    - form / input / select / textarea / button / label/ select 表单元素

一些常用 html 标签讲解

### meta
 `<meta charset="UTF-8">`

用来设置文档编码

 `<meta name="viewport" content="width=device-width, initial-scale=1.0,user-scalable=no">`

主要用来适配移动端

### [a 标签](http://www.w3school.com.cn/tags/att_a_target.asp)

**a** 标签的 `target` 属性主要用来，规定在何处打开链接文档。

| 值        | 描述                                                                                                 |
| --------- | ---------------------------------------------------------------------------------------------------- |
| \_blank   | 在新窗口中打开被链接文档。                                                                           |
| \_self    | 默认。在相同的框架中打开被链接文档。                                                                 |
| \_parent  | 在父框架集中打开被链接文档。                                                                         |
| \_top     | 在整个窗口中打开被链接文档。                                                                         |
| framename | 在指定的框架或窗口中打开被链接文档，如果窗口不存在，则新建窗口。否则在指定窗口重新加载href指定的文档 |

