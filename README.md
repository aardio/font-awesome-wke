# Font Awesome for WKE( web.kit )

[Font Awesome 4.7.0](https://cdn.jsdelivr.net/npm/font-awesome@4.7.0/) 专用于 aardio web.kit 扩展库的版本。  

```javascript
import win.ui;
/*DSG{{*/
var winform = win.form(text="FontAwesome 图标字体演示";right=759;bottom=469)
/*}}*/

import web.kit.form;
var wb = web.kit.form( winform );

wb.html = /**
<head>
<link href="https://cdn.jsdelivr.net/gh/aardio/font-awesome-wke/font-awesome.min.css" rel="stylesheet">
</head>
<body>

<i class="fa fa-film  fa-3x" ></i>
<span class="sr-only">Loading...</span>
<pre>

注意：
1、WKE 内核使用 SVG 字体，如果遇到不能正常显示的图标字体，可尝试用 FontForge 打开重新生成一次即可。
2、字体是禁止跨域链接的，不要链接不同域名下的字体。
</pre>
</body>
**/
winform.show();

win.loopMessage();
```