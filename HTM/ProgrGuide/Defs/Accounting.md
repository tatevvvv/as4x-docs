﻿<html>
<head>
<title>Accounting Definition</title>
</head>

<body>

<p><font size="4" face="Arial"><strong>Описание учета</strong></font></p>

<p><font face="Arial">Если для данного вида деятельности по какому-то 
объекту ведется учет, то его нужно описать в системе, указав на всевозможные 
операции, отслеживание остатков, ведение валюты и т.д. Учет тесно связан с 
регистрацией проводок в таблице <a href="../Database/Hi.html">HI</a>
и объектом <a href="../Functions/Asfact.html">типа проводка</a>. Перед 
регистрацией проводок в учете, может появиться единое окно предварительного 
показа проводок и остатков. </font></p>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Синтаксис</b></font></p>

<p><font color="#000000" face="Arial"><strong>Accounting</strong> {<strong>Name</strong>
= <em>sAccName</em>; <br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Caption</strong> = <em>sAccCaption</em>;<br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;MainFolder</strong> = <em>sMainFolder</em>;<br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;AccFolder</strong> = <em>sAccFolder</em>;<br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Currency</strong> = <em>nCurrencyPresent</em>;<br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Remainder</strong> = <em>nRemainderPresent</em>;<br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Limit</strong> = <em>nLimitCheck</em>;<br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;RoundSumma</strong> = <em>nRoundSumma</em>;<br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;RoundCurSumma</strong> = <em>nRoundCurSumma</em>;<br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;LinkedAccounting</strong> = <em>sLinkedAccounting</em>;<br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Description</strong> = <em>sUchetDescription</em>;<br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;FactHeader</strong> = <em>sFactHeader</em>;<br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;RemHeader</strong> = <em>sRemHeader</em>;<br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Version</strong> = <em>nVersion</em>;<br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Operation</strong> {<strong>Name</strong>
= <em>sNameOperation</em>1;<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<strong>Caption</strong>
= <em>sCaptionOperation</em>1; };<br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;. . . . .</strong><br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Operation</strong> {<strong>Name</strong>
= <em>sNameOperation</em>N;<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<strong>Caption</strong>
= <em>sCaptionOperation</em>N; };<br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Script</strong> {<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<i>Subs and Functions</i><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;};<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;};<br>
</font></p>

<p><font face="Arial">Синтаксис описания учета состоит из следующих 
частей:</font></p>

<table border="1" cellPadding="5" cols="2" frame="below" rules="rows">
<TBODY>
  <tr vAlign="top">
    <td class="label" width="29%"><font face="Arial"><b>Параметр</b></font></td>
    <td class="label" width="71%"><font face="Arial"><strong>Описание</strong></font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>sAccName</em></font></td>
    <td width="71%"><font face="Arial">строковое выражение, длины 2<span lang="en-us">,</span> задающее 
	идентификатор учета.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>sAccCaption</em></font></td>
    <td width="71%"><font face="Arial">строковое выражение, 
	определяющее наименование учета.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>sMainFolder</em></font></td>
    <td width="71%"><font face="Arial">строковое выражение, определяет 
	объектную папку. Объектная папка - это папка, содержащая объекты над 
	которыми ведутся проводки и хранятся остатки.&nbsp;&nbsp; </font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>sAccFolder</em></font></td>
    <td width="71%"><font face="Arial">строковое выражение, задающее 
	папку счетов, участвующих в<br>
    корреспонденции по дебету или кредиту.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>nCurrencyPresent</em></font></td>
    <td width="71%"><font face="Arial">численное выражение, 
	принимающее значения 1 или 0, разрешающее ведение валютного учета.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>nRemainderPresent</em></font></td>
    <td width="71%"><font face="Arial">численное выражение, 
	принимающее значения 1 или 0, разрешающее отслеживание остатков в учете.</font></td>
  </tr>
  <tr>
    <td width="29%"><font color="#000000" face="Arial"><em>nLimitCheck</em></font></td>
    <td width="71%"><font face="Arial">численное выражение, 
	принимающее значения 1 или 0, определяющее проверку сумм лимита в учете. 
	Перед проведением проводок, сумма проводки предварительно проверяется на 
	нарушение установленных пределов с учетом текущего остатка объекта.</font></td>
  </tr>
  <tr>
    <td width="29%"><em><font color="#000000" face="Arial">nRoundSumma</font></em></td>
    <td width="71%"><font face="Arial">численное выражение, 
	определяющее степень округления суммы в НДЕ после десятичной запятой.</font></td>
  </tr>
  <tr>
    <td width="29%"><em><font color="#000000" face="Arial">
	nRoundCurSumma</font></em></td>
    <td width="71%"><font face="Arial">численное выражение, 
	определяющее степень округления суммы в валюте после десятичной запятой.</font></td>
  </tr>
  <tr>
    <td width="29%"><em><font color="#000000" face="Arial">
	sLinkedAccounting</font></em></td>
    <td width="71%"><font face="Arial">строковое выражение, 
	определяющее код связанного учета. Если данный параметр присутствует, то 
	проверка суммы лимита для объекта в основном учете проводится с учетом 
	текущего остатка объекта в связанном учете. Это удобно для учета отложенных 
	транзакций. Т.о. текущий остаток объекта в связанном учете суммируется с 
	текущим остатком того же объекта в основном учете и потом только <a href="../Functions/Functions/AccManagement/CheckLimit.html">
	проверяются лимиты</a>.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>sUchetDescription</em></font></td>
    <td width="71%"><font face="Arial">строковое выражение, задающее 
	краткое разъяснение назначения учета.</font></td>
  </tr>
  <tr>
    <td width="29%"><font color="#000000" face="Arial"><em>sFactHeader</em></font></td>
    <td width="71%"><font face="Arial">строковое выражение, 
	определяющее трафарет для проводок в окне предварительного показа до их 
	сохранения. Окно предварительного показа проводок и остатков может и <a href="../Functions/Functions/AccManagement/ShowTrans.html">
	не появляться</a>. Содержимое окна заполняется в обработчике системного 
	события <a href="../ScriptProcs/DisplayFact.html">DisplayFact</a>
    и <a href="../ScriptProcs/DisplayRem.html">DispayRem</a>.</font></td>
  </tr>
  <tr>
    <td width="29%"><font color="#000000" face="Arial"><em>sRemHeader</em></font></td>
    <td width="71%"><font face="Arial">строковое выражение, 
	определяющее трафарет остатков в окне предварительного показа до сохранения 
	проводок. Окно предварительного показа проводок и остатков может и <a href="../Functions/Functions/AccManagement/ShowTrans.html">
	не появляться</a>. Содержимое окна заполняется в обработчике системного 
	события <a
    href="../ScriptProcs/DisplayFact.html">DisplayFact</a> и <a
    href="../ScriptProcs/DisplayRem.html">DispayRem</a>.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>nVersion</em></font></td>
    <td width="71%"><font face="Arial">численное выражение целого 
	типа, определяющее номер версии описания учета.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>sNameOperation</em></font></td>
    <td width="71%"><font face="Arial">строковое выражение,<span lang="en-us">
	</span><span lang="ru">длины 3</span><span lang="en-us">,</span> задающее 
	идентификатор (код) допустимой в учете операции.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>sCaptionOperation</em></font></td>
    <td width="71%"><font face="Arial">строковое выражение, задающее 
	наименование операции.</font></td>
  </tr>
</TBODY>
  <tr>
    <td width="29%"><font color="#000000" face="Arial"><i>Subs and 
	Functions</i></font></td>
    <td width="71%"><font face="Arial">скриптовый раздел описания, 
	который может содержать <a
    href="../scriptstproced.html">обработчики системных событий</a>
    и пользовательские процедуры и функции.</font></td>
  </tr>
</table>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Примечание</b></font></p>

<p class="label"><font face="Arial">Если в описании учета не описаны 
операции, тогда в учете допускаются любые операции.</font></p>

<p class="label"><a href="../Defs.html"><font face="Arial">См. также</font></a></p>
</body>
</html>