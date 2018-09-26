﻿<html>

<head><META HTTP-EQUIV="Content-Type" CONTENT="text/html; charset=utf-8">
<meta name="GENERATOR" content="Microsoft FrontPage 12.0">
<title>File</title>
</head>

<body>

<p><font size="4" face="Arial"><strong>Тип данных File</strong></font></p>

<p class="label"><font face="Arial">Файловый тип данных определяющий путь к файлу в 
    файловой системе. Он также дает возможность указать типы файлов, разделяющихся 
    друг от друга точка запятыми(;), например <strong>File</strong>(*.txt;*.xls) или <strong>File</strong>(*.doc), 
    но не обеспечивает проверку типов, если вручную будет введено путь к файлу с 
    типом, не совпадающим с указанными типами.</font></p>
    <p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Синтаксис</b></font></p>

<p><font size="4" face="Arial"><strong>File</strong></font></p>

<p class="label"><font face="Arial"><a href="../types.html">См. также</a></font></p>
    <p class="label">&nbsp;</p>

<p><strong><font size="3" face="Arial">Пример использования </font><font
face="Arial">типа <font size="4" face="Arial">File</font></font></strong></p>

<p><font face="Arial">dlg.AddControl("ImpFile", #ImpFile, "<strong>File</strong>(*.txt;*.xls)", "R", , #e_ImpFile).</font></p>

<p class="label">&nbsp;</p>
</body>
</html>