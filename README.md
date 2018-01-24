## 水平垂直居中


### flex
设为`flex`布局后，子元素的`float`、`clear`、`vertical-align`属性将失效

* flex水平居中和垂直居中
`flex + justify-content + align-items`

只需设置父节点属性，无需设置子元素

### 水平居中

* 对于行内元素（inline）**父元素**：`text-align: center`;
* 对于块级元素（block）：该元素设置宽度和 `margin: 0 auto`
* 对于多个块状元素： 对父元素设置 `text-align:center;` 对子元素设置`display:inline-block` 或者是 `flex布局`

### 垂直居中
* 对于行内元素（inline）
  - 单行： 设置上下 `pandding` 相等；或者设置 `line-height` 和 `height` 相等
  - 多行：设置上下 `pandding` 相等；或者设置 `display: table-cell;` 和 `vertical-align: middle;`；或者使用 `flex` 布局；或者使用`伪元素`
* 对于块状元素（block）
  - 已知高度：子元素使用绝对布局 `top: 50%;`，再用`负的 margin-top` (子元素高度的一半)
  - 未知高度：子元素使用绝对布局 `position: absolute; top: 50%; transform: translateY(-50%);`



### 参考： 
- [关于css水平垂直居中的总结](https://github.com/hawx1993/tech-blog/issues/12)
- 颜大大 [yanhaijing/vertical-center](https://github.com/yanhaijing/vertical-center)