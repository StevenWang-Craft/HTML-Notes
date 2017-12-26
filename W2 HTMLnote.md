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
9. [Comments](#commnents)
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
## 1. Basic
<a name="basic"></a>

## 2. Element
<a name="element"></a>

## 3. Attributes
<a name="attributes"></a>

## 4. Headings
<a name="headings"></a>
    ~~~html
    <h1>..<h6>
    ~~~

## 5. Paragraphs
<a name="paragraphs"></a>

## 6. Styles
<a name="styles"></a>

## 7. Formatting
<a name="formatting"></a>

## 8. Quotations
<a name="quotations"></a>

## 9. Comments
<a name="comments"></a>

## 10. Colors
<a name="colors"></a>

## 11. CSS
<a name="css"></a>

## 12. Links
<a name="links"></a>

## 13. Images
<a name="images"></a>

## 14. Tables
<a name="tables"></a>

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

## 15. Lists
<a name="lists"></a>
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

<a name="head1234"></a>

## 16. Blocks
<a name="blocks"></a>

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

## 17. Classes
<a name="classes"></a>
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

## 18. Iframe
<a name="iframe"></a>

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
The link will be opened in the iframe window
~~~html
<iframe src="" name="iframe_a"></iframe>
<p><a href="html://...." target="iframe_a"...></a></p>
~~~

## 19. HTML Javascript
<a name="js"></a>

### tags
~~~html
<script></script>
<noscript></noscript>
~~~
