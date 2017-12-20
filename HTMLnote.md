# HTML 预习
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