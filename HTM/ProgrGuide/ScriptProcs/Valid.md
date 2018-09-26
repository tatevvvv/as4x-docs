﻿<html>
<head>
<title>Системное событие документа Valid </title>
</head>

<body>

<p><strong><font size="4" face="Arial">Событие Valid<br>
<br>
</font></strong><font face="Arial"><a href="../scriptstproced.html">См.
также</a>&nbsp; <a href="../Examples/E_Valid.html">Пример</a>&nbsp; <a
href="../Defs/doc.html">Применяется к</a></font></p>

<p class="label"><font face="Arial">Генерируется при
попытке выхода из поля заполнения реквизита.
Служит для проверки введенных значений
реквизита на соответствие некоторому условию.<span lang="en-us"> </span><br>
Последовательность генерации системных событий
для документа приведена здесь <a href="Events_Sequence.html"><img
src="../../../IMAGES/More.gif" width="12" height="12" alt="More.gif (304 bytes)"
border="0"></a>.</font></p>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Синтаксис</b></font></p>

<p><font face="Arial">Sub <strong>Valid </strong>(<i>ByVal Rekv,</i> [<em><span lang="en-us">Old</span>Value</em>])<br>
&nbsp;&nbsp; <strong>Select Case</strong> <strong>Rekv</strong> <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <strong>Case</strong> <em>Rekv1</em><br>
<em>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp; statements1</em><br>
&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; <strong>Case</strong> <em>Rekv2</em><br>
<em>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp; statements2</em><br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; . . . . .<br>
</strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <strong>Case</strong> <em>RekvN</em><br>
<em>&nbsp;&nbsp; &nbsp; &nbsp;&nbsp;&nbsp;&nbsp; statementsN</em><br>
<strong>&nbsp;&nbsp;&nbsp; End Select&nbsp; </strong>&nbsp;&nbsp; <br>
End Sub</font></p>

<p>&nbsp;</p>

<p><font face="Arial">Синтаксис события <strong>Valid</strong>
состоит из следующих частей:</font></p>

<table border="1" cellPadding="5" cols="2" frame="below" rules="rows">
<TBODY>
  <tr vAlign="top">
    <td class="label" width="29%"><font face="Arial"><b>Параметр</b></font></td>
    <td class="label" width="71%"><font face="Arial"><strong>Описание</strong></font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>RekvI</em></font></td>
    <td width="71%"><font face="Arial">строковое выражение,
    определяющее идентификатор реквизита в
    документе. </font></td>
  </tr>
  <tr>
    <td width="29%" height="18"><font face="Arial"><em><span lang="en-us">Old</span>Value</em></font></td>
    <td width="71%" height="18"><font face="Arial">необязательное
    выражение, содержащее старое значение данного
      реквизита.</font></td>
  </tr>
</table>

<p class="label"><font face="Arial"><b>Примечания</b></font></p>

<p class="label"><font face="Arial">Идентификатор реквизита передается 
с верхнем регистре (<span lang="en-us">UCASE</span>)<span lang="en-us">. <br>
</span>Если поле заполнения реквизита только для<span lang="en-us"> </span>
чтения (задан атрибут <span lang="en-us">R)</span>, то генерации события не 
происходит.</font></p>
</body>
</html>