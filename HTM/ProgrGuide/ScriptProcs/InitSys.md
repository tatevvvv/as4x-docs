﻿<html>
<head>
<title>Системное событие InitSys</title>
</head>

<body>

<p><font size="4" face="Arial"><strong>Событие InitSys<br>
<br>
</strong></font><font face="Arial"><a href="../scriptstproced.html">См. 
также</a>&nbsp; <u>Пример</u>&nbsp; <a href="../Defs/Module.html">Применяется к</a></font></p>

<p class="label"><font face="Arial">Происходит при входе в систему, 
после ввода пароля пользователя. Обработчик данного события должен быть описан в 
одном из <a href="../Defs/Module.html">общедоступных модулей</a>, у которых в 
описании Public=1. Причем в системе должна существовать только одна процедура с 
именем InitSys. Она удобна для совершения предварительных любых действий до 
входа в систему.</font></p>

<p class="label"><font face="Arial"><b>Синтаксис</b></font></p>

<p><font face="Arial">Sub <strong>InitSys</strong>()<br>
<em>&nbsp;&nbsp;&nbsp;&nbsp; statements</em><br>
End Sub</font></p>

<p>&nbsp;</p>
</body>
</html>