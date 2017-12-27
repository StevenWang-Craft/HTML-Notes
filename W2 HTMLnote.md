# HTML 预习
## Index 
1. [Basic](#basic)
2. [Element](#element)
3. [Attributes](#attributes)
4. [Headings](#headings)
5. [Paragraphs](#paragraphs)
6. [Styles](#styles)
7. [Formatting](#formatting)
8. [Quotations](#quotations)
9. [Comments](#comments)
10. [Colors](#colors)
11. [CSS](#css)
12. [Links](#links)
13. [Images](#images)
14. [Tables](#tables)
15. [Lists](#lists)
16. [Blocks](#blocks)
17. [Classes](#classes)
18. [Iframe](#iframe)
19. [HTML Javascript](#js)
20. [File Paths](#paths)
21. [Head](#head)
22. [Layout](#layout)
23. [Responsive](#responsive)
24. [Computercode](#computercode)
25. [Entities](#entities)
26. 
---
<a name="basic"></a>

## 1. Basic
---
<a name="element"></a>

## 2. Element
---
<a name="attributes"></a>

## 3. Attributes
---
<a name="headings"></a>

## 4. Headings

    ~~~html
    <h1>..<h6>
    ~~~
---
<a name="paragraphs"></a>

## 5. Paragraphs
---
<a name="styles"></a>

## 6. Styles
---
<a name="formatting"></a>

## 7. Formatting
---
<a name="quotations"></a>

## 8. Quotations
---
<a name="comments"></a>

## 9. Comments
---
<a name="colors"></a>

## 10. Colors
---
<a name="css"></a>

## 11. CSS
---
<a name="links"></a>

## 12. Links
---
<a name="images"></a>

## 13. Images
---
<a name="tables"></a>

## <b>14. Tables</b>
### Syntax    
~~~html
<table>
    <tr>
        <th>..</th>
        <th>..</th> <!--th for header, header for the col-->
    </tr>
    <tr>
        <th>..</th> <!--header for the row-->
        <td>..</td> <!--td for data-->
    </tr>
</table>
~~~
### Attribute
#### Border/ Collapsed Borders
~~~html
<style>
    table, th, td{
        border：1px solid black; <!--每个元素上都有边界-->
        border-collapse: collapes; <!-- 边界合并-->
    }
</style>
~~~
#### Cell Padding
~~~html
<style>
    th, td{
        padding: 15px;
    }
</style>
~~~
#### Headings alignment
~~~html
<style>
    th{
        text-align: right; 
    }
</style>
~~~
#### Border Spacing
~~~html
<style>
    table{
        border-spacing: ..px; 
    }
</style>
~~~
#### Span
~~~html
<table>
    <tr>
        <th colspan="2">
    </tr>
    <tr>
        <td>data1</td>
        <td>data2</td>
    </tr>
</table>

<table>
    <tr>
        <th>..
        <td>..
    </tr>
    <tr>
        <th rowspan="2">Telephone</th>
        <td>data1</td>
    </tr>
    <tr>
        <td>data2</td>
    </tr>
</table>
~~~
#### Caption
~~~html
<table>
    <caption>xxxx</caption>
    <tr>
        ...
    </tr>
</table>
~~~
#### Style attribute
~~~html
    <style>
        <!--针对整行节点，附加：非表头-->
        table#t01 tr:nth-child(even){
        }
        
        <!--针对“表头”节点--->
        table#t01 th {
        }

        <!--针对整个表-->
        table#t01 {
            width:
            background-color:
        } 
    </style>
~~~
---
<a name="lists"></a>

## <b>15. Lists</b>
### Syntax
* Unordered
    ~~~html
    <ul>
        <li>...</li>
    </ul>
    ~~~
    * Attribute: type
    ~~~html
    <ul style="list-style-type:disc">

    </ul>
    ~~~
    |Marker|Display
    |-|-
    |disc|bullet
    |circle| circle
    |square| square
    |none| not be marked

* Ordered
    ~~~html
    <ol>
        <li>...</li>
    </ol>
    ~~~
    * Attribute: type
    ~~~html
    <ol type="1">
    
    </ol>
    ~~~ 
    | Marker |         Display          |
    | ------ | ------------------------ |
    | 1      | numbers                  |
    | A      | letters                  |
    | a      | letters - lowercase      |
    | I      | roman number - uppercase |
    | i      | roman number - lowercase |

* Description List
    ~~~html
    <dl>
        <dt>data term</dt>
        <dd>- data description</dd>
    </dl>
    ~~~
### Nested HTML Lists

### Horizontal Lists
* Using CSS , to list horizontally, to create a `menu`
---
<a name="blocks"></a>

## <b>16. Blocks</b>
### Blocks
* start a new line + take up the full width
* common used tags:
    ~~~html
    <address>
    <div>
    <p>
    <ol>
    ~~~
### Inline
* not new line + takes up as necessary
* common used tags
    ~~~html
    <span>
    <a>
    <br>
    <img>
    ~~~
### \<div>
* `container` of other elements
* common attributes:
    * `style`
    * `class`
### \<span>
* `container` of other elements
* common attributes:
    * `style`
    * `class`
---
<a name="classes"></a>

## <b>17. Classes</b>
THis is attribute for all element. THe class attribute specifies one or more class names for an HTML element.

THe class name can be sed by CSS and JavaScript to perform certain tasks for elements with the specified class name.
### Syntax
~~~html
<tag class="">...</tag>
~~~~
Different tags can have same tags
~~~html
<tag1 class=""></tag1>
<tag2 class=""></tag2>
~~~
CSS usage
~~~html
<style>
    .city{
        background-color:
        color:
        padding:
    }
</style>
~~~
---
<a name="iframe"></a>

## <b>18. Iframe</b>
Display a web page within a web page
### Syntax
~~~html
<iframe src=""></iframe>
~~~
### height & width
~~~html
<iframe src="" height="" width=""></iframe>
~~~
### remove the border
~~~html
<iframe scr="" style="border:none;"></iframe>
~~~
### target for a link
`The link will be opened in the iframe window`
~~~html
<iframe src="" name="iframe_a"></iframe>
<p><a href="html://...." target="iframe_a"...></a></p>
~~~
---
<a name="js"></a>

## <b>19. HTML Javascript</b>
### tags
~~~html
1. <script></script>

2. <noscript></noscript>
~~~
---
<a name="paths"></a>

## <b>20. File Paths</b>
1. Absolute File Paths
2. Relative File Paths
    * images folder -> root of the curent web
    * images folder -> current folder
    * images folder -> one level up of current folder
---
<a name="head"></a>

## <b>21. Head</b>
Head is a element for metadata. Metadata includes:
~~~html
1. <title>
2. <style>
3. <meta>
4. <link>
5. <script>
6. <base>
~~~
### \<title>
### \<style>
### \<link>
### \<meta>
* charset
* name="description" content=""
* name="keywords" content=""
* name="author" content=""
* http-equiv="refresh" content=""
* name="viewport" content=""
### \<script>
`<head> can be omitted`
---
<a name="layout"></a>

## <b>22. Layout</b>
### HTML5 Layout Element
![image](https://user-images.githubusercontent.com/8587006/34369144-a91bc098-eb0d-11e7-8c26-62e20b91bc05.png)
### HTML Layout Techniques
* HTML tables (never use for layout)
* CSS float property
    * `pros`: easy learn: float and clear property
    * `cons`: tied to the document flow. harm the flexibility
* Flexbox
    * `pros`: good for different screen size
    * `cons`: not work in IE10 and earlier
---
<a name="responsive"></a>

## <b>23. Responsive</b>
### Whole page
* Viewport
### Image
* width property
* max-width property
* \<picture> element for multi-pics
### Text Size
* font-size property, `vw` unit
### Judge and Dicision
* Media Queries
~~~css
@media (max-width:800px){
    .left, .main, .right{
        width:100%
    }
}
~~~
### Frameworks that offer RWD
* W3.CSS
* Bootstrap
---
<a name="computercode"></a>

## <b>24. Computercode</b>
### Keyboard Input
~~~html
<kbd>Ctrl + s</kbd>
~~~
### Program Output
~~~html
<samp>error!</samp>
~~~
### Code
~~~html
<pre>
<code>
x = 5;
y = 6;
z = x + y;
</code>
</pre>
~~~
### Vasriables
~~~html
<var>E</var> = <var>mc</var><sup>2</sup>.
~~~
<math>
	<var>E</var> = <var>mc</var><sup>2</sup>.
</math>

---
<a name="entities"></a>

## <b>25. Entities</b>
### Character Entities
![image](https://user-images.githubusercontent.com/8587006/34370131-acd66b68-eb15-11e7-8d8d-34055a52679c.png)

### Diacritical Marks
![image](https://user-images.githubusercontent.com/8587006/34370146-cbecc25e-eb15-11e7-8c52-075615b3bbc3.png)

### Symbols Entities
* Mathematical Symbols
![image](https://user-images.githubusercontent.com/8587006/34370199-2960494c-eb16-11e7-8c8c-9cc65f8893d1.png)
* Greek Letters
![image](https://user-images.githubusercontent.com/8587006/34370215-402171ba-eb16-11e7-9689-932efd30ac11.png)
* Other Entities
![image](https://user-images.githubusercontent.com/8587006/34370221-4b01dc00-eb16-11e7-9051-c39fbc5cd2c9.png)

<a href="https://www.w3schools.com/charsets/ref_utf_currency.asp">Full Currency Reference</a><br>
<a href="https://www.w3schools.com/charsets/ref_utf_arrows.asp">Full Arrows Reference</a><br>
<a href="https://www.w3schools.com/charsets/ref_utf_symbols.asp">Full Symbols Reference</a>

---
<a name="url-encoding"></a>

## <b>26. URL Encoding</b>

---
## -- The End --