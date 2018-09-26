﻿<html>
<head>
<title>Документ\SetRekvsReadOnly</title>
    <style type="text/css">
        .style1
        {
            height: 29px;
        }
        .style2
        {
            height: 30px;
        }
    </style>
</head>

<body>

<p><strong><font size="4" face="Arial">Свойство SetRekvsReadOnly</font></strong></p>

<p><font face="Arial"><a href="../Asdoc.html">См. также</a>&nbsp; <a href="../../Examples/E_SetRekvsReadOnly.html">Пример</a>&nbsp;&nbsp;<a href="../Asdoc.html">Применяется к</a></font></p>

<p><font face="Arial">Возвращает или устанавливает статус режима 
редактирования набора реквизитов документа.</font></p>

<p class="label"><font face="Arial">Свойство для чтения и записи.</font></p>

<p class="label">&nbsp;</p>

<p class="label"><b><font face="Arial">Синтаксис</font></b></p>

<p><font face="Arial"><em>object.<strong>SetRekvsReadOnly</strong></em>(<em>RekvNames, 
    [bValue], 
    [sDelimeter]</em>)</font></p>

<p><font face="Arial">Синтаксис свойства <strong>SetRekvsReadOnly</strong>
состоит из следующих частей:</font></p>

<table border="1" cellPadding="5" cols="2" frame="below" rules="rows">
<TBODY>
  <tr vAlign="top">
    <td class="label" width="29%"><font face="Arial"><b>Параметр</b></font></td>
    <td class="label" width="71%"><font face="Arial"><strong>Описание</strong></font></td>
  </tr>
  <tr>
    <td width="29%"><em><font face="Arial">object</font></em></td>
    <td width="71%"><font face="Arial">строковое выражение, являющееся 
	ссылкой на экземпляр документа</font></td>
  </tr>
  <tr>
    <td width="29%"><em><font face="Arial">RekvNames</font></em></td>
    <td width="71%"><font face="Arial">строковое выражение, 
	определяющее идентификаторы реквизитов документа, разделенных между собой любым 
        условным символом или пробелом.</font></td>
  </tr>
    <tr>
    <td width="29%" class="style2"><font face="Arial"><em>bValue</em></font></td>
    <td width="71%" class="style2"><font face="Arial">необязательное логическое выражение, определяющее возможность 
        редактирования указанных реквизитов, по умолчанию принимает значение True.</font></td>
    </tr>
  <tr>
    <td width="29%" class="style1"><font face="Arial"><em>sDelimeter</em></font></td>
    <td width="71%" class="style1"><font face="Arial">необязательное строковое выражение, определяющее 
        любой символ или пробел, с помощью которого задаются реквизиты в <em>
        RekvNames.</em></font></td>
  </tr>
</TBODY>
</table>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Установки</b></font></p>

<p><font face="Arial">Установки для <em>bValue</em>
следующие:</font></p>

<table border="1" cellPadding="5" cols="2" frame="below" rules="rows">
<TBODY>
  <tr vAlign="top">
    <td class="label" width="29%"><font face="Arial"><b>Значение</b></font></td>
    <td class="label" width="71%"><font face="Arial"><strong>Описание</strong></font></td>
  </tr>
  <tr vAlign="top">
    <td width="29%"><font face="Arial">True</font></td>
    <td width="71%"><font face="Arial">Редактирование реквизитов 
	допустимо</font></td>
  </tr>
  <tr vAlign="top">
    <td width="29%"><font face="Arial">False</font></td>
    <td width="71%"><font face="Arial">Редактирование реквизитов 
	недопустимо</font></td>
  </tr>
</table>
    <p>
        &nbsp;</p>
    </body>
</html>