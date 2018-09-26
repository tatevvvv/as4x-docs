﻿<html>
<head>
<title>Системное событие PostMessage</title>
</head>

<body>

<p><strong><font size="4" face="Arial">Событие PostMessage<br>
<br>
</font></strong><font face="Arial"><a href="../scriptstproced.html">См. 
также</a>&nbsp; <u>Пример</u>&nbsp; <a href="../Defs/doc.html">Применяется к</a></font></p>

<p class="label"><font face="Arial">Генерируется в теле 
документа-получателя при получении сообщения <a
href="../Functions/ASDOC/SendMessage.html">SendMessage</a> от 
документа-инициатора. </font></p>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Синтаксис</b></font></p>

<p><font face="Arial">Sub <strong>PostMessage</strong> (<em>tmpDoc, 
sMessage, </em>[<i>xCheckLevel</i>])<br>
<em>&nbsp;&nbsp;&nbsp;statements</em><br>
End Sub</font></p>

<p><font face="Arial">Синтаксис события <strong>PostMessage</strong>
состоит из следующих частей:</font></p>

<table border="1" cellPadding="5" cols="2" frame="below" rules="rows">
<TBODY>
  <tr vAlign="top">
    <td class="label" width="29%"><font face="Arial"><b>Параметр</b></font></td>
    <td class="label" width="71%"><font face="Arial"><strong>Описание</strong></font></td>
  </tr>
  <tr>
    <td width="29%"><em><font face="Arial">tmpDoc</font></em></td>
    <td width="71%"><font face="Arial">переменная, ссылающаяся на 
	документ-источник сообщения. </font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>sMessage</em></font></td>
    <td width="71%"><font face="Arial">строковое выражение, 
	определяющее текст полученного сообщения</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><i>xCheckLevel</i></font></td>
    <td width="71%"><font face="Arial">ссылочная переменная, 
	возвращающая необходимый уровень проверки документа перед сохранением(см.
	<a href="../Functions/ASDOC/CheckAndStore.html">CheckAndStore</a>).</font></td>
  </tr>
</table>

<p class="label">&nbsp;</p>
</body>
</html>