# HTML 预习
[tables](#head1234)

## 1. Basic
## 2. Element
## 3. Attributes
## 4. Headings
    ~~~html
    <h1>..<h6>
    ~~~
## 5. Pragraphs
## 6. Styles
## 7. Formatting
## 8. Quotations
## 9. Comments
## 10. Colors
## 11. Css
## 12. Links
## 13. Images
## 14. Tables
<a name="head1234"></a>

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

## 15. Blocks
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

## 16. Classes
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

## 17. Iframe
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

## 18. HTML Javascript
### tags
~~~html
<script></script>
<noscript></noscript>
~~~
