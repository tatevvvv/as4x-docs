﻿<html>

<head><META HTTP-EQUIV="Content-Type" CONTENT="text/html; charset=utf-8">
<meta name="GENERATOR" content="Microsoft FrontPage 12.0">
<title>NumPair()</title>
</head>

<body>

<p><strong><font size="4" face="Arial">Тип данных NumPair( )</font></strong></p>

<p class="label"><font face="Arial">Тип числовая пара. Она состоит из 
двух чисел разделенных заданным символом разделителя, т.е. типа &quot;число1 / 
число2&quot;. Например: 80.23 / 1000. Данный тип может использоваться в <a href="../Defs/doc.html">
описании реквизитов документа</a> и <a href="../Defs/Data.html">колонок источника 
данных</a>. В описании типов <a
href="../Defs/doc.html">колонок грид-таблицы документа</a>
она использоваться не может. Возможность ввода нулевых значений контролируется 
через свойства <a
href="../Functions/ASDOC/Control.htm#ZeroNumber1">ZeroNumber1</a>, <a
href="../Functions/ASDOC/Control.htm#ZeroNumber2">ZeroNumber2</a>.</font></p>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Синтаксис</b></font></p>

<p><font face="Arial"><strong>NumPair</strong>(<em>Type1, Type2, </em>
[<em>Comment</em>], [<em>Label</em>]<em>, </em>[<em>EComment</em>], [<em>ELabel</em>])</font></p>

<p><font face="Arial">Синтаксис типа <strong>NumPair</strong>() 
состоит из следующих частей:</font></p>

<table border="1" cellPadding="5" cols="2" frame="below" rules="rows">
<TBODY>
  <tr vAlign="top">
    <td class="label" width="29%"><font face="Arial"><b>Параметр</b></font></td>
    <td class="label" width="71%"><font face="Arial"><strong>Описание</strong></font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>Type1</em></font></td>
    <td width="71%"><font face="Arial">числовой тип данных <a
    href="Np().html">NP()</a> или <a href="N().html">N()</a>, определяющий тип 
	значения первой суммы. При использовании других типов сгенерируется ошибка.</font></td>
  </tr>
</TBODY>
  <tr>
    <td width="29%"><em><font face="Arial">Type2</font></em></td>
    <td width="71%"><font face="Arial">числовой тип данных <a
    href="Np().html">NP()</a> или <a href="N().html">N()</a>, определяющий тип 
	значения второй суммы. При использовании других типов сгенерируется ошибка.</font></td>
  </tr>
  <tr>
    <td width="29%"><em><font face="Arial">Comment</font></em></td>
    <td width="71%"><font face="Arial">необязательное строковое 
	выражение, определяющее разделитель двух сумм. По умолчанию принимается &quot;/&quot;.</font></td>
  </tr>
  <tr>
    <td width="29%"><em><font face="Arial">Label</font></em></td>
    <td width="71%"><font face="Arial">необязательное строковое 
	выражение длиной до 10 символов, определяющее метку.</font></td>
  </tr>
  <tr>
    <td width="29%"><em><font face="Arial">EComment</font></em></td>
    <td width="71%"><font face="Arial">необязательное строковое 
	выражение, определяющее разделитель двух сумм на иностранном языке. По 
	умолчанию принимается значение <strong><em>Comment</em></strong>.</font></td>
  </tr>
  <tr>
    <td width="29%"><em><font face="Arial">ELabel</font></em></td>
    <td width="71%"><font face="Arial">необязательное строковое 
	выражение длиной до 10 символов, определяющее метку на иностранном языке. По 
	умолчанию принимается значение <strong><em>Label</em></strong>.</font></td>
  </tr>
</table>

<p class="label"><font face="Arial"><a href="../types.html">См. также</a></font></p>

<p class="label">&nbsp;</p>

<p><font size="3" face="Arial"><strong>Пример использования типа </strong></font></p>

<p><font face="Arial">Экземпляр типа <strong>NumPair</strong>
(NP(7,3), NP(6,0), &quot; за &quot;) определяет курс валюты.</font></p>
</body>
</html>