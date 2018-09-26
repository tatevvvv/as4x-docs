﻿<html>
<head>
<title>Константы типов выполнения SQL-запроса</title>
</head>

<body>

<p><font face="Arial"><big>Константы типов выполнения SQL-запроса</big></font></p>

<p><font face="Arial">Т.к. эти константы объявлены в системном ядре, 
то нет необходимости в их дополнительном объявлении. Их можно использовать везде 
в скриптах, взамен их значений.</font></p>

<table border="1">
  <tr>
    <td width="20%"><font size="3" face="Arial"><b>Константа</b></font></td>
    <td width="20%"><font size="3" face="Arial"><b>Значение</b></font></td>
    <td width="60%"><font size="3" face="Arial"><b>Описание</b></font></td>
  </tr>
  <tr>
    <td width="20%"><strong><font face="Arial">ASAsyncEnable</font></strong></td>
    <td width="20%" align="center"><font face="Arial"><strong>32</strong></font></td>
    <td width="60%"><font face="Arial">выполняет запрос асинхронным 
	образом.</font></td>
  </tr>
  <tr>
    <td width="20%"><strong><font face="Arial">ASExecDirect</font></strong></td>
    <td width="20%" align="center"><font face="Arial"><strong>64</strong></font></td>
    <td width="60%"><font face="Arial">по умолчанию. Использует 
	функцию ODBC <b>SQLExecDirect</b> для выполнения запроса.</font></td>
  </tr>
</table>

<blockquote>
</blockquote>

<p><font face="Arial"><br>
Эти константы могут быть также использованы в качестве параметров функции <a
href="../Functions/Functions/ExecuteQuery.html">ExecuteQuery</a>, для определения 
типа выполнения SQL-запроса.</font></p>
</body>
</html>