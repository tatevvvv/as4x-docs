<html>
<head>
<title>Документ\ControlValue</title>
</head>

<body>

<p><font face="Arial"><font size="4"><strong>Свойство ControlValue<br>
<br>
</strong></font><a href="../Asdoc.html">См. также</a>&nbsp; <u>Пример</u>&nbsp;
<a href="../Asdoc.html">Применяется к</a></font></p>

<p class="label">У<font face="Arial">станавливает значение для элемента 
    управления, осуществляющий ввод. Другими словами задает значение свойству <a href="Control.html">
	Control</a>. <strong>ControlValue</strong>&nbsp; предназначено для параметра 
    <strong><em>OldValue</em></strong> события <a href="../../ScriptProcs/Valid.html">Valid</a>. При отсутствии 
    данного свойства, после обработки события 
    <a href="../../ScriptProcs/ClickDropDown.html">ClickDropDown</a> значение <strong>
    <em>OldValue</em></strong> портится, и при изменении значения 
    реквизита старое значение не сохраняется.

</font></p>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Синтаксис</b></font></p>

<p><font face="Arial"><em>object.</em><strong>ControlValue(</strong><em>RekvName</em><strong>) = </strong><em>vValue</em></font></p>

<p><font face="Arial">Синтаксис свойства <strong>ControlValue</strong>
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
	ссылкой на экземпляр документа</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>RekvName</em></font></td>
    <td width="71%"><font face="Arial">строковое выражение, 
	определяющее идентификатор реквизита документа</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>vValue</em></font></td>
    <td width="71%"><font face="Arial">выражение типа вариант, 
	определяющее значение элемента управления</font></td>
  </tr>
</TBODY>
</table>

<p class="label">&nbsp;</p>

</body>
</html>