# interviewMap 之 CSS 知识点

# BFC

`BFC` 全称为 `block formatting context`, 中文为 '块级格式化上下文'

如果一个元素具有 `BFC`, 内部子元素再怎么折腾，都不会影响外部的元素。

触发 `BFC` 的情况:
* `html` 根元素
* `float` 的值不为 `none`
* `overflow` 的值为 `auto`,`scroll` 或 `hidden`
* `display` 的值为 `table-cell`、`table-caption` 和 `inline-block` 中的任何一个
* `position` 的值不为 `relative` 和 `static`


# 居中的几种方式

# 盒模型

# 清除浮动的几种方式

# !important

`!important` 提供了增加权重的方式，一旦为某条样式使用，那么基本上他的权重就是最高的了。

当然凡事都是有例外的

```css
div {
  width: 200px !important;
  height: 100px;
  background-color: red;
  max-width: 100px;
}
```

当你如上设置时，会发现加了 `!important`  的 ` width` 还是被 `max-width` 覆盖了，宽度变为了 100 。

如果你又设置了 `min-width` ，并且值比 `max-width` 大，那么你又会发现前者覆盖了后者。

# 单位

- px：这是一个相对单位，在 PC 中往往对应着一个物理像素，当你缩放页面的时候，会发现元素也会相应的缩放。在移动端中，因为视网膜屏的存在，px 得乘上 `devicePixelRatio` 才能得到对应的物理像素。
- em：相对于自身的 `font-size` 大小
- rem：相对于根元素的 `font-size` 大小
- vw：相对于 viewport 的宽度
- vh：相对于 viewport 的高度

# 像素与 viewport

# flex 布局

# grid 布局

# 画一条 0.5px 的线

# css 选择器

# em,rem,vh,vw

# 定位

# 伪元素

# Normalize.css 与 reset.css

# 文档流