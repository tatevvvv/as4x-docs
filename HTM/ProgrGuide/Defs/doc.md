﻿<html>
<head>
<title>Document Definition</title>
<style type="text/css">
.style1 {
	font-family: Arial;
}
</style>
</head>

<body>

<strong><font size="4" face="Arial">Описание документа<br>
</font></strong><font face="Arial">Основой системы
является документ с набором состояний и
логикой существования. Документ может содержать
реквизиты различных типов. В качестве реквизитов
документа могут выступать <a href="../rekvizit.html">обычные
поля ввода</a>, <a href="../grid.html">реквизиты типа грид-таблиц</a>,
<a href="../image.html">реквизиты-изображения</a>, <a href="../memo.html">реквизиты
типа мемо-полей</a>,<span lang="ru"> <a href="../line.html">реквизиты типа линий</a></span>,<a href="../button.html">
<span lang="ru">реквизиты типа кнопок</span></a>. Реквизиты могут быть
сгруппированы в <a href="../page.html">страничных вкладках</a>. В
скриптовом разделе описания документа могут
находится как <a href="../scriptstproced.html">обработчики
системных событий</a>, так и пользовательские
процедуры и функции.<br>
<span lang="ru">В описании документа могут содержаться <a href="../access.html">дескрипторы доступа</a> и 
<a href="../FolderInfo.html">папок документа</a>.<br>
</span><b><br>
Синтаксис</b></font>

<font face="Arial"><strong><br>
<br>
DOCUMENT</strong> {<strong><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Name </strong>=<em> sDocName</em>;
<strong><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Caption </strong>=<em> sDocCaption</em>;<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ECaption </strong>= <em>sDocECaption</em>;<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; PrintWidth</strong>=<em>nDocPrintWidth</em>;<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; PrintFormated</strong>=<em>nDocPrintFormated</em>;<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; DisableDraft</strong>=<em>nDocDisableDraft</em>;<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <b>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; DisableCopy</b>=<em>nDocDisableCopy;<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<strong>Type</strong> = nPatternSupport;
<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<strong>Attachments</strong>
= nAttachments; <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; HI2Support</strong> 
=
nHI2Support;<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; HISSSupport</strong> 
=
nHISSSupport; <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; MTSupport</strong> 
=
nMTSupport; <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; FASupport</strong> 
=
nFASupport; <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; WordTemplate</strong> = stmplNameWord;<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ExcelTemplate</strong> = stmplNameExcel;<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Version</strong> = nVersion;<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Icon</strong> = sIconName;<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<strong>Accounting</strong> = nAccountingCode;<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<strong>ContrSupport </strong>= bContrSupport;<br>
<strong><span lang="en-us">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span>AccessFolder</strong> = 
sAccessFolder;<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </em>
<strong>STOREINTREE</strong><em> = nStoreInTree<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
<strong>CopyA</strong></em><strong><em>sRepeatable</em></strong><em> = nCopyMode<br />
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
    DISABLEATTACHMENTSIZECHECK</strong> = nDisableAttachsizeCheck</em><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<span lang="en-us"><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><a href="../page.html">{Страничные вкладки<span lang="en-us"> };</span></a><strong><br>
</strong>&nbsp;&nbsp;<span lang="en-us">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span>&nbsp;<span lang="en-us"><a href="../access.html">{Дескрипторы доступа};</a><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;</span><a href="../FolderInfo.html">{</a><span lang="en-us"><a href="../FolderInfo.html">Дескрипторы папки документа};</a></span><br />
    <br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <a href="../FolderInfo.html">{</a><span lang="en-us"><a href="../PrintDataGroup.html">Группы печатной формы документа};</a></span><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong><br>
<span lang="ru">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>
<span lang="en-us">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><strong>Script</strong> {<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<em>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Subs and
Functions</em></font>
<font face="Arial"><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; };<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; };<br>
</font>

<p><font face="Arial">Синтаксис описания документа
состоит из следующих частей:</font></p>

<table border="1" cellPadding="5" cols="2" frame="below" rules="rows">
<TBODY>
  <tr vAlign="top">
    <td class="label" style="height: 31px; width: 4%;">&nbsp;</td>
    <td class="label" width="29%" style="height: 31px"><font face="Arial"><b>Параметр</b></font></td>
    <td class="label" width="71%" style="height: 31px"><font face="Arial"><strong>
	Описание</strong></font></td>
  </tr>
  <tr>
    <td style="width: 4%">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16"></td>
    <td width="29%"><em><font face="Arial">sDocName</font></em></td>
    <td width="71%"><font face="Arial">строковое выражение, определяющее 
	идентификатор документа</font></td>
  </tr>
  <tr>
    <td style="width: 4%">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16"></td>
    <td width="29%"><em><font face="Arial">sDocCaption</font></em></td>
    <td width="71%"><font face="Arial">строковое выражение, определяющее 
	заголовок документа</font></td>
  </tr>
  <tr>
    <td style="width: 4%">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16"></td>
    <td width="29%"><em><font face="Arial">sDocECaption</font></em></td>
    <td width="71%"><font face="Arial">строковое выражение, определяющее 
	заголовок документа на иностранном языке</font></td>
  </tr>
  <tr>
    <td style="width: 4%">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16"></td>
    <td width="29%"><font face="Arial"><em>nDocPrintWidth</em></font></td>
    <td width="71%"><font face="Arial">числовое выражение, определяющее ширину 
	печатной формы документа в символах.</font></td>
  </tr>
  <tr>
    <td style="width: 4%">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16"></td>
    <td width="29%"><font face="Arial"><em>nDocPrintFormated</em></font></td>
    <td width="71%"><font face="Arial">числовое выражение, принимающее значения 
	1 или 0, определяющее признак форматирования текста в печатной форме(<a href="../Functions/AsRepViewer/UseFormatting.html">см. 
	также</a>).</font></td>
  </tr>
  <tr>
    <td style="width: 4%">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16"></td>
    <td width="29%"><font face="Arial"><em>nDocDisableDraft</em></font></td>
    <td width="71%"><font face="Arial">числовое выражение, принимающее значения 
	1 или 0, определяющее признак создания документа без возможности создания 
	черновика. </font></td>
  </tr>
  <tr>
    <td style="width: 4%; height: 16px">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" style="height: 16px"><font face="Arial"><em>nDocDisableCopy</em></font></td>
    <td width="71%" style="height: 16px"><font face="Arial">числовое выражение, принимающее значения 
	1 или 0. При значении 1 отключается возможность создания копии для 
	документов данного типа. Значение по умолчанию 0.</font></td>
  </tr>
  <tr>
    <td style="width: 4%">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16"></td>
    <td width="29%"><em><font face="Arial">nPatternSupport</font></em></td>
    <td width="71%"><font face="Arial">численное выражение, принимающее значения 
	1 или 0, определяющее признак поддержки шаблонов проводок. Шаблоны типовых 
	операций возможно описывать только над документами, для которых данное 
	значение установлено 1.</font></td>
  </tr>
  <tr>
    <td style="width: 4%">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16"></td>
    <td width="29%"><font face="Arial"><em>nAttachments</em></font></td>
    <td width="71%"><font face="Arial">численное выражение, принимающее значения 
	1 или 0, определяющее признак прикрепления <a href="../Functions/AsAttachment.html">
	файлового дополнения</a> к документу.</font></td>
  </tr>
  <tr>
    <td style="width: 4%">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16"></td>
    <td width="29%"><em><font face="Arial">nHI2Support</font></em></td>
    <td width="71%"><font face="Arial">численное выражение, принимающее значения 
	1 или 0, определяющее признак отслеживания изменений в таблице HI2 при 
	работе с данным документом. Это относится к удалению документа и проводок с 
	очисткой их следов из HI2, а также проверке лимитов при сохранении проводок.</font></td>
  </tr>
  <tr>
    <td style="width: 4%">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16" longdesc="../../../IMAGES/pubfield.gif"></td>
    <td width="29%"><em><font face="Arial">nHISSSupport</font></em></td>
    <td width="71%"><font face="Arial">численное выражение, принимающее значения 
	1 или 0, определяющее признак отслеживания изменений в специальных таблицах 
	срочных договоров при работе с данным документом.</font></td>
  </tr>
  <tr>
    <td style="width: 4%">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16"></td>
    <td width="29%"><em><font face="Arial">nMTSupport</font></em></td>
    <td width="71%"><font face="Arial">численное выражение, принимающее значения 
	1 или 0, определяющее признак отслеживания изменений в специальных таблицах 
	материальных ценностей при работе с данным документом.</font></td>
  </tr>
  <tr>
    <td style="width: 4%">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16"></td>
    <td width="29%"><em><font face="Arial">nFASupport</font></em></td>
    <td width="71%"><font face="Arial">численное выражение, принимающее значения 
	1 или 0, определяющее признак отслеживания изменений в специальных таблицах 
	основных средств при работе с данным документом.</font></td>
  </tr>
  <tr>
    <td style="width: 4%">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16"></td>
    <td width="29%"><em><font face="Arial">stmplNameWord</font></em></td>
    <td width="71%"><font face="Arial">строковое выражение, определяющее имя 
	файла шаблона печатного вида документа в формате Word-а. Длина имени 
	шаблонного файла не должна превышать 20 символов. <br>В связи с вводом 
	механизма настриваемого пользователями шаблонов печати этот механизм <strong>
	явлется устаревшим, </strong>настоятельно рекомендуется не использовать его.</font></td>
  </tr>
</TBODY>
  <tr>
    <td style="width: 4%">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16"></td>
    <td width="29%"><em><font face="Arial">stmplNameExcel</font></em></td>
    <td width="71%"><font face="Arial">строковое выражение, определяющее имя 
	файла шаблона печатного вида документа в формате Excel-а. Длина имени 
	шаблонного файла не должна превышать 20 символов. Если имя файла равно
	<strong>SYSTEMPLATE</strong>, то работает системная процедура выгрузки в&nbsp;&nbsp; 
	в формате Excel-а.<br>В связи с вводом механизма настриваемого 
	пользователями шаблонов печати этот механизм <strong>явлется устаревшим,
	</strong>настоятельно рекомендуется не использовать его кроме случая <strong>
	SYSTEMPLATE</strong>.</font></td>
  </tr>
  <tr>
    <td style="width: 4%">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16"></td>
    <td width="29%"><em><font face="Arial">nVersion</font></em></td>
    <td width="71%"><font face="Arial">численное выражение целого типа, 
	определяющее номер версии описания документа.<span lang="ru"> 
	Зарезервировано для дальнейшего использования.</span></font></td>
  </tr>
  <tr>
    <td style="width: 4%">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16"></td>
    <td width="29%"><em><font face="Arial">sIconName</font></em></td>
    <td width="71%"><font face="Arial">строковое выражение, определяющее 
	идентификатор иконки одного из изображений, поддерживаемых системой.</font></td>
  </tr>
  <tr>
    <td style="width: 4%">

<img src="../../../IMAGES/pubfield.gif" width="16" height="16"></td>
    <td width="29%">

<font face="Arial"><em>nAccountingCode</em></font></td>
    <td width="71%" class="style1"><font face="Arial">строковое выражение,<span lang="ru"> 
	определяющее идентификатор учета, </span>которому<br>
	принадлежит данный документ.</font></td>
  </tr>
  <tr>
    <td style="width: 4%">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16"></td>
    <td width="29%"><em><font face="Arial">sAccessFolder</font></em></td>
    <td width="71%"><font face="Arial">строковое выражение, определяющее 
	идентификатор папки, содержащее заголовки доступов данного документа. При 
	отсутствии данного параметра повторное подтверждение для документа 
	невозможно.</font></td>
  </tr>
  <tr>
    <td style="width: 4%">

<img src="../../../IMAGES/pubfield.gif" width="16" height="16"></td>
    <td width="29%">

<font face="Arial"><em>nContrSupport</em></font></td>
    <td width="71%"><font face="Arial">численное выражение, принимающее значения 
	1 или 0 <span lang="en-us">и</span> определяющее&nbsp; 
	признак регистрации фактов в таблице ContractHI</font></td>
  </tr>
    <tr>
    <td style="width: 4%">

<img src="../../../IMAGES/pubfield.gif" width="16" height="16"></td>
    <td width="29%">

<font face="Arial"><em>nStoreInTree</em></font></td>
    <td width="71%"><font face="Arial">численное выражение, принимающее значения 
	1 или 0 <span lang="en-us">и</span> определяющее&nbsp;признак возможности записи 
	в дереве</font></td>
    </tr>
  <tr>
    <td style="width: 4%">

<img src="../../../IMAGES/pubfield.gif" width="16" height="16"></td>
    <td width="29%">

<font face="Arial"><em> nCopyMode</em></font></td>
    <td width="71%"><font face="Arial">численное выражение, принимающее значения 
	1 или 0 <span lang="en-us">и</span> определяющее&nbsp;режим визуального 
	копирования документа. При значении 0 все реквизиты документа копируются. 
	При значении 1 копируются только значения реквизитов котрые содержат атрибут 
	N. Значение по умолчанию 0.</font></td>
  </tr>
    <tr>
    <td style="width: 4%">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16"></td>
    <td width="29%"><font face="Arial"><em>nDisableAttachsizeCheck</em></font></td>
    <td width="71%"><font face="Arial">численное выражение, принимающее значения 1 или 
        0. При значении 1 отключается проверка максимального размера как отдельного&nbsp; <a href="../Functions/AsAttachment.html">
	файлового дополнения</a> к документу(<strong><em>MAXSIZE</em></strong>), так и&nbsp; 
        всех&nbsp; <a href="../Functions/AsAttachment.html">
	файловых дополнений</a> вместе взятых(<strong><em>MAXTOTALSIZE</em></strong>). По умолчанию 
        принимает значение 0.</font></td>
    </tr>
  <tr>
    <td style="width: 4%">
	<img src="../../../IMAGES/pubmethod.gif" width="16" height="11">&nbsp;</td>
    <td width="29%"><font color="#000000" face="Arial"><i>Subs and Functions</i></font></td>
    <td width="71%"><font face="Arial">скриптовый раздел описания, который может 
	содержать как&nbsp; <a
    href="../scriptstproced.html">обработчики системных событий</a>, так и 
	пользовательские процедуры и функции.</font></td>
  </tr>
</table>


<font face="Arial"><b><br>
Примечание</b></font>

<font face="Arial"><br>
<br>
В системе на описание
документа наложено ограничение на размер файла
описания в 80 kb.<br>
<br>
</font><a href="../Defs.html"><font face="Arial">См. также</font></a>
</body>
</html>