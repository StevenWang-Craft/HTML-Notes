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

---
<a name="basic"></a>

## 1. Basic
<a name="element"></a>

## 2. Element
<a name="attributes"></a>

## 3. Attributes
<a name="headings"></a>

## 4. Headings

    ~~~html
    <h1>..<h6>
    ~~~
<a name="paragraphs"></a>

## 5. Paragraphs
<a name="styles"></a>

## 6. Styles
<a name="formatting"></a>

## 7. Formatting
<a name="quotations"></a>

## 8. Quotations
<a name="comments"></a>

## 9. Comments
<a name="colors"></a>

## 10. Colors
<a name="css"></a>

## 11. CSS
<a name="links"></a>

## 12. Links
<a name="images"></a>

## 13. Images
<a name="tables"></a>

## 14. Tables
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
<a name="lists"></a>

## 15. Lists
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

<a name="blocks"></a>

## 16. Blocks
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

<a name="classes"></a>

## 17. Classes
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
<a name="iframe"></a>

## 18. Iframe
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
<a name="js"></a>

## 19. HTML Javascript
### tags
~~~html
1. <script></script>

2. <noscript></noscript>
~~~

<a name="paths"></a>

## 20. File Paths
1. Absolute File Paths
2. Relative File Paths
    * images folder -> root of the curent web
    * images folder -> current folder
    * images folder -> one level up of current folder

<a name="head"></a>

## 21. Head
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