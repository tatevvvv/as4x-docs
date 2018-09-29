<html>
<head>
<title>Документ\RegistrNode</title>
</head>

<body>

<p><strong><font size="4" face="Arial">Метод RegistrNode<br>
<br>
</font></strong><font face="Arial"><a href="../Asdoc.html">См. также</a>&nbsp;
<u>Пример</u>&nbsp; <a href="../Asdoc.html">Применяется к</a></font></p>

<p><font face="Arial">Добавляет группировочный узел в меню 
пользовательских функций. При большом количестве вызываемых функций их удобнее 
сгруппировать в структуру подменю.</font></p>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Синтаксис</b></font></p>

<p><font face="Arial"><em>object</em><strong>.RegistrNode </strong>(<em>NodeId, 
mnCaption, </em>[<em>ParentId</em>]<em>, </em>[<em>ECaption</em>], [AvailableFor])</font></p>

<p><font face="Arial">Синтаксис метода <strong>RegistrNode</strong>
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
    <td width="29%"><font face="Arial"><em>NodeId</em></font></td>
    <td width="71%"><font face="Arial">строковое выражение, 
	определяющее идентификатор узла</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>mnCaption</em></font></td>
    <td width="71%"><font face="Arial">строковое выражение, 
	определяющее заголовок узла</font></td>
  </tr>
</TBODY>
  <tr>
    <td width="29%"><font face="Arial"><em>ParentId</em></font></td>
    <td width="71%"><font face="Arial">необязательное строковое 
	выражение, определяющее ссылку на идентификатор вышестоящего узла в меню 
	контекстных вызовов. Если не задано, то текущая запись меню добавляется на 
	корневом уровне.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>ЕCaption</em></font></td>
    <td width="79%"><font face="Arial">необязательное строковое 
	выражение, определяющее строку добавляемой в контекстное меню записи на 
	иностранном языке. По умолчанию значение равно <em>Caption.</em></font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>AvailableFor</em></font></td>
    <td width="79%"><font face="Arial">необязательное цифровое 
	выражение, определяющее <a href="../../Constants/const_RegistrFunctionAvailability.html">константу видимости</a> группировочного узла.</font></td>
  </tr>
</table>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Примечание</b></font></p>

<p class="label"><font face="Arial">Данный метод должен быть вызван в 
обработчике системного события
<a href="../../ScriptProcs/FunctionsDoc.html">Functions</a>. </font></p>
</body>
</html>