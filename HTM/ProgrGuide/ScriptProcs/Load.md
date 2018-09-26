﻿<html>
<head>
<title>Системное событие документа Load </title>
</head>

<body>

<p><strong><font size="4" face="Arial">Событие Load<br>
<br>
</font></strong><font face="Arial">
<a href="../Functions/Functions/CreateXArrayDB.html">См. также</a>&nbsp; <u>
Пример</u>&nbsp; <a href="../Functions/Asdata.html">Применяется к</a></font></p>

<p class="label"><font face="Arial">Генерируется если значение 
свойства ArrayBased равно единице. Служит для передачи ядру данных для 
заполнения&nbsp;объекта источник данных. Событие должно возвратить объект типа 
XArrayDB количество колонок равно количеству колонок в источнике данных, а 
строки соответствуют строкам в источнике данных.</font></p>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Синтаксис</b></font></p>

<p><font face="Arial">Function <b>Load</b> As <i>XArrayDB</i><br>
<br>
End Function </font></p>

<p class="label"><font face="Arial"><b>Примечание</b></font></p>

<p class="label"><font face="Arial">Объект типа XArrayDB необходимо 
создать при помощи вызова&nbsp; функции&nbsp;
<a href="../Functions/Functions/CreateXArrayDB.html">CreateXArrayDB</a>.</font></p>

<blockquote>

<p class="label"><font face="Arial">Public Function Load As XArrayDB<br>
&nbsp; Dim xArr As XArrayDB<br>
&nbsp; Set xArr = CreateXArrayDB<br>
&nbsp; xArr.ReDim 0, 0, 0, 1<br>
&nbsp; xArr.DeleteRows 0<br>
<br>
&nbsp; xArr.AppendRows<br>
&nbsp; xArr(0,0)=&quot;01&quot;<br>
&nbsp; xArr(0,1)=&quot;Caption 01&quot;<br>
<br>
&nbsp; xArr.AppendRows<br>
&nbsp; xArr(1,0)=&quot;02&quot;<br>
&nbsp; xArr(1,1)=&quot;Caption 02&quot;<br>
<br>
&nbsp; xArr.AppendRows<br>
&nbsp; xArr(2,0)=&quot;03&quot;<br>
&nbsp; xArr(2,1)=&quot;Caption 03&quot;<br>
<br>
&nbsp; Set Load=xArr<br>
End Function</font></p>

</blockquote>

<p>&nbsp;</p>

</body>
</html>