﻿<html>
<head>
<title>Системное событие&nbsp; SQL</title>
</head>

<body>

<p><font size="4" face="Arial"><strong>Событие SQL<br>
<br>
</strong></font><font face="Arial"><a href="../scriptstproced.html">См. 
также</a>&nbsp; <a href="../Examples/E_SQL.html">Пример</a>&nbsp; <a
href="../Defs/Data.html">Применяется к</a></font></p>

<p class="label"><font face="Arial">Происходит перед открытием 
источника данных, динамически формируя SQL запрос. Вид запроса формируется в 
зависимости от количества параметров, переданных в источник данных. 
Активизируется также после вызова методов <a
href="../Functions/ASDATA/OpenCursor.html">OpenCursor</a> и <a
href="../Functions/FrmPttel/Update.html">Update</a>. Последовательность генерации 
системных событий для источника данных приведена здесь <a href="Events_Sequence_Data.html"><img
src="../../../IMAGES/More.gif" width="12" height="12" alt="More.gif (304 bytes)"
border="0"></a>.</font></p>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Синтаксис</b></font></p>

<p><font face="Arial">Sub <strong>SQL</strong> (ByRef <em>sSQL</em>, 
ByRef <em>sUpdate</em>)<br>
<em>&nbsp;&nbsp; statements</em><br>
End Sub</font></p>

<p><font face="Arial">Синтаксис события <strong>SQL</strong>
состоит из следующих частей:</font></p>

<table border="1" cellPadding="5" cols="2" frame="below" rules="rows">
<TBODY>
  <tr vAlign="top">
    <td class="label" width="29%"><font face="Arial"><b>Параметр</b></font></td>
    <td class="label" width="71%"><font face="Arial"><strong>Описание</strong></font></td>
  </tr>
  <tr>
    <td width="29%"><em><font face="Arial">sSQL</font></em></td>
    <td width="71%"><font face="Arial">строковое выражение, 
	определяющее SQL запрос к базе данных </font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>sUpdate</em></font></td>
    <td width="71%"><font face="Arial">строковое выражение, 
	определяющее SQL запрос к базе данных после обновления данных</font></td>
  </tr>
</table>
</body>
</html>