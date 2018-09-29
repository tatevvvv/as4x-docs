<html>
<head>
<title>DocParents</title>
</head>

<body>

<p><font size="4" face="Arial"><strong>Функция DocParents</strong></font></p>

<p><font face="Arial">Возвращает коллекцию родителей (значений ISN) 
для указанного документа. Если документ не имеет родителей, то функция 
возвращает Nothing. В коллекцию можно включить или исключить определенные типы 
документов родителей.</font></p>

<p>&nbsp;</p>

<p class="label"><font face="Arial"><b>Синтаксис</b></font></p>

<p><font face="Arial"><strong>DocParents (</strong><em>ISN, </em>[<em>DocType</em>]<strong>,
</strong>[<em>nOrder</em>]<strong>)</strong></font></p>

<p><font face="Arial">Синтаксис функции <strong>DocParents</strong>
состоит из следующих частей:</font></p>

<table border="1" cellPadding="5" cols="2" frame="below" rules="rows">
<TBODY>
  <tr vAlign="top">
    <td class="label" width="29%"><font face="Arial"><b>Параметр</b></font></td>
    <td class="label" width="71%"><font face="Arial"><strong>Описание</strong></font></td>
  </tr>
  <tr>
    <td class="label" width="29%"><font face="Arial"><em>ISN</em></font></td>
    <td class="label" width="71%"><font face="Arial">численное 
	выражение типа Long, определяющее внутрисистемный идентификационный код ISN 
	исходного документа, для которого приводятся родители.</font></td>
  </tr>
  <tr>
    <td class="label" width="29%"><font face="Arial"><em>DocType</em></font></td>
    <td class="label" width="71%"><font face="Arial">необязательное 
	строковое выражение, определяющее тип возвращаемых или исключаемых типов 
	документов родителей. Если параметр не задан, то приводятся коды ISN для 
	всех типов родителей. Для включения в коллекцию документов определенных 
	типов нужно перечислить типы документов через пробел и значение параметра 
	должно начинаться знаком &quot;+&quot;. Для исключения из коллекции документов 
	определенных типов нужно перечислить типы документов через пробел и значение 
	параметра должно начинаться знаком &quot;-&quot;. </font></td>
  </tr>
  <tr>
    <td class="label" width="29%"><font face="Arial"><em>nOrder</em></font></td>
    <td class="label" width="71%"><font face="Arial">необязательное 
	численное выражение, определяющее порядок сортировки. При значении 0 
	документы не упорядочены. При значении 1 упорядочены по убыванию ISN, а при 
	значении 2 - по возрастанию. По умолчанию принимает значение 0.</font></td>
  </tr>
	<tr>
    <td class="label" width="29%"><font face="Arial"><em>DocTypeLike</em></font></td>
    <td class="label" width="71%"><font face="Arial">необязательное 
	строковое выражение, определяющее шаблон для возвращаемых или исключаемых 
	типов документов родителей. Если параметр не задан, то приводятся&nbsp; коды ISN 
	для всех типов родителей. Для включения в коллекцию документов определенных 
	типов по шаблону нужно задать шаблон типов и значение параметра&nbsp; должно 
	начинаться знаком &quot;+&quot;.&nbsp; Если в коллекцию необходимо включить документы за 
	исключением некоторых типов по шаблону, тогда значение параметра должно 
	начинаться знаком &quot;-&quot; для задания списка исключений. Например &quot;-AccDoc%&quot;.</font></td>
  </tr>
</table>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Примечание<br>
<br>
</b>Интервал индексов элементов коллекции начинается с 1 до значения свойства 
Count коллекции.</font></p>

<p class="label"><a href="../../../functions.html"><font face="Arial">
См. также</font></a></p>
</body>
</html>