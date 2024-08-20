# < Head>:
- 类似于C++ 的include；
- < title>： title of the whole html file
- < meta> : describe data eg. <meta charset="utf-8" />
- 许多 `<meta>` 元素包含了 `name` 和 `content` 属性：

- `name` 指定了 meta 元素的类型；说明该元素包含了什么类型的信息。
- `content` 指定了实际的元数据内容。
- 搜索引擎也会利用这些信息
```html
<meta name="author" content="Chris Mills" />
<meta
  name="description"
  content="The MDN Web Docs Learning Area aims to provide
complete beginners to the Web with all they need to know to get
started with developing web sites and applications." />

```

- 总之不同的元数据协议（不同公司/组织提供）可以实现特定功能
```html
<link rel="icon" href="favicon.ico" type="image/x-icon" />

```
This is an example of adding icon to a web

- - [`<link>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/link) 元素经常位于文档的头部，它有 2 个属性，`rel="stylesheet"` 表明这是文档的样式表，而 `href` 包含了样式表文件的路径：
    ```html
    <link rel="stylesheet" href="my-css-file.css" />
    ```
- [`<script>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/script) 元素也应当放在文档的头部，并包含 `src` 属性来指向需要加载的 JavaScript 文件路径，加上 `defer` 以告诉浏览器在解析完成 HTML 后再加载 JavaScript。
    ```html
    <script src="my-js-file.js" defer></script>
    ```

 - 你还可以将文档的分段设置为不同的语言。例如，我们可以把日语部分设置为日语，如下所示：< span>


```html
<p>Japanese example: <span lang="ja">ご飯が熱い。</span>.</p>
```
# text edit
- < p>: paragraph
-  < h1> - < h6> levelled head title like # - ###### 
- List:  < ol>, < ul> ordered/unordered list
``` html
<ul>          
<li> item</li>
...
<ul>
```
- to emphasis: < em>,  < strong>
-  [`<i>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/i) 被用来传达传统上用斜体
- [`<b>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/b) 粗体
- [`<u>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/u) 下划线

# hyper link

```html
<p>
  我创建了一个指向
  <a href="https://www.mozilla.org/zh-CN/">Mozilla 主页</a>的链接。
</p>
```

- title属性， 当鼠标指针悬停在链接上时，标题将作为提示信息出现```
 title="了解 Mozilla 使命以及如何参与贡献的最佳站点。"

- Uniform Resource Locator，URL
- 超链接除了可以链接到文档外，也可以链接到 HTML 文档的特定部分（被称为**文档片段**）
- ![[Pasted image 20240820170141.png]]添加 id 属性可以定位所需要链接的位置 ： 比如点击网页某个链接可能跳转到标题
-  downlaod 属性：
```html 
<a
  href="https://download.mozilla.org/?product=firefox-latest-ssl&os=win64&lang=zh-CN"
  download="firefox-latest-64bit-installer.exe">
  下载最新的 Firefox 中文版 - Windows（64 位）
</a>

```
-  < mailto> send email 

# more techniques of text edit:
- 描述列表 使用与其他列表类型不同的闭合标签——[`<dl>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/dl)；此外，每一项都用 [`<dt>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/dt)（description term）元素闭合。每个描述都用 [`<dd>`](https://developer.mozilla.org/zh-CN/docs/Web/HTML/Element/dd)（description definition）元素闭合。
- 