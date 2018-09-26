﻿<html>
<head>
<title>Системное событие опис. диалога _Validate</title>
</head>

<body>

<p><font face="Arial"><font size="4"><strong>Событие _Validate<br>
<br>
</strong></font><a href="../scriptstproced.html">См. также</a>&nbsp; <a
href="../Examples/E_Dialog_Validate.html">Пример</a>&nbsp; <a
href="../Defs/Dialog.html">Применяется к</a></font></p>

<p class="label"><font face="Arial">Генерируется cистемой для проверки 
значений элементов управления диалога. Данное событие генерируется и для диалога 
и для элементов управления, имеющихся в <a
href="../Defs/Dialog.html">диалоге</a>.</font></p>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Синтаксис</b></font></p>

<p><font face="Arial">Sub <em>ContrName</em><strong>_Validate()<br>
</strong><em>&nbsp;&nbsp;&nbsp; statements</em><br>
End Sub</font></p>

<p><font face="Arial"><br>
Синтаксис события <strong>_Validate</strong> состоит из следующих частей:</font></p>

<table border="1" cellPadding="5" cols="2" frame="below" rules="rows">
<TBODY>
  <tr vAlign="top">
    <td class="label" width="29%"><font face="Arial"><b>Параметр</b></font></td>
    <td class="label" width="71%"><font face="Arial"><strong>Описание</strong></font></td>
  </tr>
  <tr>
    <td width="29%"><em><font face="Arial">ContrName</font></em></td>
    <td width="71%"><font face="Arial">строковое выражение, являющееся 
	либо идентификатором элемента управления либо ключевым словом <strong>Dialog</strong>. 
	В первом случае событие выполняется для проверки значений элемента 
	управления с указанным именем. Во втором случае, событие выполняется после 
	нажатия кнопки OK, для глобальной проверки введенных значений элементов 
	управления диалога, перед их сохранением.&nbsp;&nbsp;</font></td>
  </tr>
</table>
</body>
</html>