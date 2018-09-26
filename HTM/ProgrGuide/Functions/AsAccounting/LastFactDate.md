﻿<html>
<head>
<title>Учет\LastFactDate</title>
</head>

<body>

<p><font face="Arial"><font size="4"><strong>Свойство LastFactDate<br>
<br>
</strong></font><a href="../AsAccounting.html">См. также</a>&nbsp; <a
href="../../Examples/E_AsAccounting.html">Пример</a>&nbsp; <a
href="../AsAccounting.html">Применяется к</a></font></p>

<p><font face="Arial">Возвращает дату последней проводки в учете.</font></p>

<p class="label"><font face="Arial">Если проводка не найдена, то 
возвращается Null.</font></p>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Синтаксис</b></font></p>

<p><font face="Arial"><em>object</em><strong>.LastFactDate (</strong><em>nISN, </em>
[<em>UpToDate</em>]<strong>,
</strong>[<em>Op</em>]<strong>)</strong></font></p>

<p><font face="Arial">Синтаксис свойства <strong>LastFactDate</strong>
состоит из следующих частей:</font></p>

<table border="1" cellPadding="5" cols="2" frame="below" rules="rows">
<TBODY>
  <tr vAlign="top">
    <td class="label" width="29%"><font face="Arial"><b>Параметр</b></font></td>
    <td class="label" width="71%"><font face="Arial"><strong>Описание</strong></font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>object</em></font></td>
    <td width="71%"><font face="Arial">строковое выражение, являющееся 
	ссылкой на объект типа учет</font></td>
  </tr>
</TBODY>
  <tr>
    <td width="29%"><font face="Arial"><em>nISN</em></font></td>
    <td width="71%"><font face="Arial">численное выражение типа Long, 
	определяющее ISN объекта учета для которого приводится дата</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>UpToDate</em></font></td>
    <td width="71%"><font face="Arial">необязательное выражение типа 
	даты, указывающее дату до которой производится поиск. Если параметр опущен, 
	то возвращается дата самой последней проводки в данном учете.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>Op</em></font></td>
    <td width="71%"><font face="Arial">необязательное строковое 
	выражение, определяющее код операции, указывающий на поиск операции именно с 
	таким кодом.</font></td>
  </tr>
</table>

<p>&nbsp;</p>

<p><font face="Arial"><strong>Тип данных</strong></font></p>

<p><font face="Arial">Дата</font></p>
</body>
</html>