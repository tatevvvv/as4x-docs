<html>
<head>
<title>GetAccKey</title>
</head>

<body>

<p><strong><font size="4" face="Arial">Функция GetAccKey</font></strong></p>

<p class="label"><font face="Arial">Возвращает контрольный ключ для 
банковского счета.<br>
<br>
Возвращаемое значение строковое.</font></p>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Синтаксис</b></font></p>

<p><font face="Arial"><strong>GetAccKey</strong>(<em>cBank</em>,<em> 
SmallCod</em>)</font></p>

<p><font face="Arial">Синтаксис функции <b>GetAccKey</b>
состоит из следующих частей:</font></p>

<table border="1" cellPadding="5" cols="2" frame="below" rules="rows">
<TBODY>
  <tr vAlign="top">
    <td class="label" width="29%"><font face="Arial"><b>Параметр</b></font></td>
    <td class="label" width="71%"><font face="Arial"><strong>Описание</strong></font></td>
  </tr>
  <tr vAlign="top">
    <td width="29%"><font face="Arial"><em>cBank</em></font></td>
    <td width="71%"><font face="Arial">строковое выражение, 
	определяющее код банка, где находится банковский счет</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>SmallCod</em></font></td>
    <td width="71%"><font face="Arial">строковое выражение, 
	определяющее банковский счет</font></td>
  </tr>
</TBODY>
</table>

<p class="label"><br>
</p>

<p class="label"><font face="Arial"><b>Примечание</b></font></p>

<p class="label"><a href="../../functions.html"><font face="Arial">См. 
также</font></a></p>

<p class="label">&nbsp;</p>

<h1><font size="3" face="Arial"><strong>Пример свойства GetAccKey</strong></font></h1>

<p><font face="Arial"><font size="3">Реквизиту CODE </font>
присваивается значение контрольного ключа для текущего набранного банковского 
счета в банке Param(&quot;CODBANK&quot;).<br>
</font></p>

<p><font face="Arial"><a href="../ASDOC/Rekv.html">doc(&quot;CODE&quot;)</a>=GetAccKey(<a href="ParameterManagment/Param.html">Param</a>(&quot;CODBANK&quot;), 
doc(&quot;CODE&quot;))&nbsp;&nbsp;&nbsp; <br>
</font></p>
</body>
</html>