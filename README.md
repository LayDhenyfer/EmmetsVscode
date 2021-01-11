# EmmetsVscode
Atalhos para melhorar sua produtividade 

Para usar o emmet no vscode digite o código e aperte enter, quando aparecer uma opção como essa.  

<a href="https://ibb.co/QKCxy43"><img src="https://i.ibb.co/S3dZFz4/emmet.png" alt="emmet" border="0"></a>

Caso não apareça, digite o código com emmet e em seguinda aperte ctrl+barra

                                                                                                                                                    
<img  src="https://media.giphy.com/media/Dex51nonSOTlXJDAvG/giphy.gif" width="700">

Child: >
```bash
- nav>ul>li

<nav>
    <ul>
        <li></li>
    </ul>
</nav>
```
Sibling: +
```bash
- div+p+bq

<div></div>
<p></p>
<blockquote></blockquote>
```
Climb-up: ^
```bash
- div+div>p>span+em^bq

<div></div>
<div>
    <p><span></span><em></em></p>
    <blockquote></blockquote>
</div>  

- div+div>p>span+em^^bq

<div></div>
<div>
    <p><span></span><em></em></p>
</div>
<blockquote></blockquote>
```
Grouping: ()
```bash
- div>(header>ul>li*2>a)+footer>p

<div>
    <header>
        <ul>
            <li><a href=""></a></li>
            <li><a href=""></a></li>
        </ul>
    </header>
    <footer>
        <p></p>
    </footer>
</div>

- (div>dl>(dt+dd)*3)+footer>p

<div>
    <dl>
        <dt></dt>
        <dd></dd>
        <dt></dt>
        <dd></dd>
        <dt></dt>
        <dd></dd>
    </dl>
</div>
<footer>
    <p></p>
</footer>
```
Multiplication: *
```bash
- ul>li*5

<ul>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
    <li></li>
</ul>
```
Item numbering: $
```bash

- ul>li.item$*5

<ul>
    <li class="item1"></li>
    <li class="item2"></li>
    <li class="item3"></li>
    <li class="item4"></li>
    <li class="item5"></li>
</ul>

- h$[title=item$]{Header $}*3

<h1 title="item1">Header 1</h1>
<h2 title="item2">Header 2</h2>
<h3 title="item3">Header 3</h3>

- ul>li.item$$$*5

<ul>
    <li class="item001"></li>
    <li class="item002"></li>
    <li class="item003"></li>
    <li class="item004"></li>
    <li class="item005"></li>
</ul>

- ul>li.item$@-*5

<ul>
    <li class="item5"></li>
    <li class="item4"></li>
    <li class="item3"></li>
    <li class="item2"></li>
    <li class="item1"></li>
</ul>

- ul>li.item$@3*5

<ul>
    <li class="item3"></li>
    <li class="item4"></li>
    <li class="item5"></li>
    <li class="item6"></li>
    <li class="item7"></li>
</ul>
```
ID and CLASS attributes
```bash
- #header

<div id="header"></div>

- .title

<div class="title"></div>

- form#search.wide

<form id="search" class="wide"></form>

- p.class1.class2.class3

<p class="class1 class2 class3"></p>
```
Custom attributes
```bash
- p[title="Hello world"]

<p title="Hello world"></p>

- td[rowspan=2 colspan=3 title]

<td rowspan="2" colspan="3" title=""></td>

- [a='value1' b="value2"]

<div a="value1" b="value2"></div>
```
Text: {}
```bash
- a{Click me}

<a href="">Click me</a>

- p>{Click }+a{here}+{ to continue}

<p>Click <a href="">here</a> to continue</p>
```
Implicit tag names
```bash 

- .class

<div class="class"></div>

- em>.class

<em><span class="class"></span></em>

- ul>.class

<ul>
    <li class="class"></li>
</ul>

- table>.row>.col

<table>
    <tr class="row">
        <td class="col"></td>
    </tr>
</table>
```
Links
```bash
link:css
<link rel="stylesheet" href="style.css" />

link:print
<link rel="stylesheet" href="print.css" media="print" />

link:favicon
<link rel="shortcut icon" type="image/x-icon" href="favicon.ico" />

link:touch
<link rel="apple-touch-icon" href="favicon.png" />

link:rss
<link rel="alternate" type="application/rss+xml" title="RSS" href="rss.xml" />

link:atom
<link rel="alternate" type="application/atom+xml" title="Atom" href="atom.xml" />

link:import, link:im
<link rel="import" href="component.html" />
```
Input
```bash
input:week
<input type="week" name="" id="" />

input:time
<input type="time" name="" id="" />

input:tel
<input type="tel" name="" id="" />

input:number
<input type="number" name="" id="" />

input:color
<input type="color" name="" id="" />

input:checkbox, input:c
<input type="checkbox" name="" id="" />

input:radio, input:r
<input type="radio" name="" id="" />

input:range
<input type="range" name="" id="" />

input:file, input:f
<input type="file" name="" id="" />

input:submit, input:s
<input type="submit" value="" />

input:image, input:i
<input type="image" src="" alt="" />

input:button, input:b
<input type="button" value="" />
```
Button
```bash
button:submit, button:s, btn:s
<button type="submit"></button>

button:reset, button:r, btn:r
<button type="reset"></button>

button:disabled, button:d, btn:d
<button disabled="disabled"></button>
```
Others
```bash
dl>dt+dd
<dl>
    <dt></dt>
    <dd></dd>
</dl>

map>area
<map name="">
    <area shape="" coords="" href="" alt="" />
</map>

table>tr>td
<table>
    <tr>
        <td></td>
    </tr>
</table>
```
