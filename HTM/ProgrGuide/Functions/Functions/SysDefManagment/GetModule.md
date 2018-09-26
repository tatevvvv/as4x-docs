﻿<html>
<head>
<title>GetModule</title>
</head>

<body>

<p><font size="4" face="Arial"><strong>Функция GetModule</strong></font></p>

<p class="label"><font face="Arial">Возвращает ссылку на модуль, 
параллельно проверяя существование указанной процедуры в модуле.</font></p>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Синтаксис</b></font></p>

<p><font face="Arial"><strong>GetModule</strong>(<em>sModName, 
sSubName</em>)</font></p>

<p><font face="Arial">Синтаксис функции <strong>GetModule</strong>
состоит из следующих частей:</font></p>

<table border="1" cellPadding="5" cols="2" frame="below" rules="rows">
<TBODY>
  <tr vAlign="top">
    <td class="label" width="29%"><font face="Arial"><b>Параметр</b></font></td>
    <td class="label" width="71%"><font face="Arial"><strong>Описание</strong></font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>sModName</em></font></td>
    <td width="71%"><font face="Arial">строковое выражение, 
	определяющее <a href="../../../Defs/Module.html">идентификатор модуля</a>.</font></td>
  </tr>
</TBODY>
  <tr>
    <td width="29%"><font face="Arial"><em>sSubName</em></font></td>
    <td width="71%"><font face="Arial">строковое выражение, 
	определяющее имя искомой процедуры в указанном модуле.</font></td>
  </tr>
</table>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Примечание<br>
<br>
</b>Данная функция полезна в случаях частых вызовов одной и той же процедуры из 
модуля. Для этого с помощью функции <strong>GetModule</strong> один раз 
загружается модуль, с проверкой существования в ней процедуры. В дальнейшем 
командой Run&nbsp; SaxBasic-а многократно запускается процедура, без проверки на 
существование в модуле.<br>
<b><br>
</b><a href="RunSub.html">См. также</a></font></p>

<p>&nbsp;</p>

<p><strong><font face="Arial" size="3">Пример функции </font><font
face="Arial">GetModule</font></strong></p>

<p><font face="Arial">В примере вызывается функция <strong>GetModule</strong>, 
через переменную xMod возвращается ссылка на модуль CRMDGEN. Дальше командой Run 
SaxBasic-а вызывается процедура AgrTypes с передачей параметров.</font></p>

<p><font face="Arial">set xMod = <strong>GetModule(</strong>&quot;CRMDGEN&quot;, 
&quot;AgrTypes&quot;<strong>)</strong><br>
...<br>
call xMod.Run(&quot;AgrTypes&quot;, &quot;Cr1AS21&quot;, TypeAgr, TypeCode)<br>
</font></p>
</body>
</html>