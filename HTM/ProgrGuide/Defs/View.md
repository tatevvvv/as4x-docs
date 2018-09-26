﻿<html>
<head>
<title>View Definition</title>
<style type="text/css">
.style1 {
	border-width: 0;
}
.style2 {
	border: 1px solid #C5C5C5;
}
.style3 {
	font-weight: bold;
	border: 1px solid #C5C5C5;
}
.style4 {
	border: 1px solid #C5C5C5;
}
.style5 {
	font-style: italic;
	border: 1px solid #C5C5C5;
}
    .style6
    {
        font-style: normal;
    }
</style>
</head>

<body>

<p><strong><font size="4" face="Arial">Описание вида просмотра</font></strong></p>

<p class="label"><font face="Arial">Вид просмотра строится на основе <a href="Data.html">источника данных</a>, 
перечислением необходимых колонок и заданием дополнительных условий фильтрации 
строк. Один и тот же источник данных может иметь множество видов просмотра, 
предназначенных для различных пользователей и рабочих мест. Вид просмотра может 
состоять из строк, являющихся <a href="doc.html">документами</a>, или же являться 
бездокументной папкой-отчетом.</font></p>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Синтаксис</b></font></p>

<font face="Arial"><strong>VIEW</strong> {<strong>&nbsp;<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Name</strong> 
= <em>sViewName</em>;<br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Caption</strong> 
= <em>sViewCaption</em>;<br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ECaption</strong> 
= <em>sViewECaption</em>;<br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; DataSource</strong> 
= <em>sViewSource</em>;<br>
<span lang="ru">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span><strong>Group</strong> 
= <em>sGroup</em>;<br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Condition</strong> 
= <em>sCondition</em>;<br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; AllowAddNew</strong> 
= <em>nAllowAddNew</em>;<strong><br />
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; AllowAccess 
= </strong> <em>nAllowAccess</em><strong>;<br />
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; AllowCopy 
= </strong> <em>nAllowCopy</em><strong>;<br />
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; AllowDelete 
= </strong> <em>nAllowDelete</em><strong>;<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; AllowEdit</strong> = <em>
nAllowEdit</em>;<br />
    <em>
    <strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong> </em><strong>
    &nbsp;AllowEditUDR</strong><em>
    = 
nAllowEditUDR; 
    <br />
    <strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong> </em><strong>&nbsp;AllowExport</strong><em>
    = 
nAllowExport;<br />
    <strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span class="style6">&nbsp;AllowHistory</span> </strong> 
    = 
nAllowHistory;<br />
    <strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong> </em><strong>AllowPrintPreview</strong><em> = 
nAllowPrintPreview<strong>;<br />
    &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <span class="style6">&nbsp;AllowSecondEntry</span> 
=
    </strong> 
    nAllowSecondEntry<strong>;</strong></em><br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; AllowView</strong> 
= <em>nAllowView</em>;<br>
    <strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; AllowViewDocChildren </strong> 
<em>= 
nAllowViewDocChildren</em><strong>;<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; AllowViewDocParents
<em>= </em></strong> <em>nAllowViewDocParents;</em><br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; AllowVisa</strong> 
= <em>nAllowVisa</em>;<em><br />
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong> 
    </em>
<strong>&nbsp; ColorColumn</strong><em>
= sColorColName;<br />
    </em><strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; DisableDocFunctions
<em>= </em></strong> <em>nDisableDocFunctions;<br />
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong> 
    </em>
<strong>DocBased</strong><em> 
= nDocBased;<br />
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong>
    </em>
<strong>HelpContext</strong><em>
= nHelpContext;<br />
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong> 
    </em>
<strong>&nbsp;ShowOnBottom</strong><em> 
= nShowOnBottom;<br />
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong> 
    </em>
<strong>SQLSort</strong><em> 
= nSortSource;<br />
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong> 
    </em>
<strong>Version</strong><em> 
= nVersion;<br />
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong>
    </em>
<strong>UnMoveColumnCount</strong><em>
= nUnMoveColCount;</em><strong><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; UpdateStyle</strong> = <em>
nUpdateStyle</em>;<br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; UserDefined </strong> 
<em>= n</em><em>UserDefined;</em><strong><br>
<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</strong> 
<em>&nbsp;</em><a href="../viewcolumn.html"><em>{</em><span lang="ru"><em>Описания колонок 
вида просмотра</em></span>}<em>;</em></a><br>
<strong> 
<em>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;</em></strong><a href="../ViewParam.html"><em>{</em><span lang="ru"><em>Описания 
значений параметров вида просмотра</em></span>}<em>;</em></a><strong><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Doc</strong> { = <em>
sDocName</em>1; .....;&nbsp; = <em>sDocName</em>N; };<br>
<br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
Script</strong> 
{<br>
<strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong>
<font color="#000000"><i><strong>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </strong> 
Subs and Functions</i></font><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;};<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; };<br>
</font>

<p><font face="Arial">СинтаСинтаксис описания вида просмотра состоит из 
следующих частей:</font></p>

<table cellPadding="5" cols="2" frame="below" rules="rows" class="style1">
<TBODY>
  <tr vAlign="top">
    <td>&nbsp;</td>
    <td class="style3" width="29%"><font face="Arial">Параметр</font></td>
    <td class="style2" width="71%"><font face="Arial"><strong>Описание</strong></font></td>
  </tr>
  <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16"></td>
    <td width="29%" class="style2"><em><font face="Arial">sViewName</font></em></td>
    <td width="71%" class="style2"><font face="Arial">строковое выражение, 
	определяющее идентификатор вида просмотра</font></td>
  </tr>
  <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><em><font face="Arial">sViewCaption</font></em></td>
    <td width="71%" class="style2"><font face="Arial">строковое выражение, 
	определяющее наименование вида просмотра</font></td>
  </tr>
  <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><em><font face="Arial">sViewECaption</font></em></td>
    <td width="71%" class="style2"><font face="Arial">строковое выражение, 
	определяющее наименование вида просмотра на иностранном языке</font></td>
  </tr>
  <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><em><font face="Arial">sViewSource</font></em></td>
    <td width="71%" class="style2"><font face="Arial">строковое выражение, 
	определяющее <a href="Data.html">источник данных</a> для данного вида<span lang="ru"> 
	просмотра</span>.</font></td>
  </tr>
  <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2">

<font face="Arial"> <em>sGroup</em></font></td>
    <td width="71%" class="style2"><font face="Arial">строковое выражение, 
	определяющее <span lang="ru">группу</span> данного вида<span lang="ru"> 
	просмотра</span>.</font></td>
  </tr>
  <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><em><font face="Arial">sCondition</font></em></td>
    <td width="71%" class="style2"><font face="Arial">строковое выражение, 
	определяющее условие выборки строк из источника данных. Данный параметр 
	является условием фильтрации над произвольными колонками источника данных.</font></td>
  </tr>
  <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><font face="Arial"> <em>nAllowAddNew</em></font></td>
    <td width="71%" class="style2"><font face="Arial">числовое выражение, принимающее 
	значения 1 или 0, определяющее разрешение на добавление нового документа. Не 
	имеет смысла для бездокументных папок.</font></td>
  </tr>
    <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><em><font face="Arial">nAllowAccess</font></em></td>
    <td width="71%" class="style2"><font face="Arial">числовое выражение, принимающее 
	значения 1 или 0, определяющее разрешение на установку доступов на документы 
	из вида просмотра. Не имеет смысла для бездокументных папок.</font></td>
    </tr>
    <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><em><font face="Arial">nAllowCopy</font></em></td>
    <td width="71%" class="style2"><font face="Arial">числовое выражение, принимающее 
	значения 1 или 0, определяющее разрешение на копирование документа, если 
        соответствующие значения <em>nAllowEdit</em> или <em>nAllowView </em>будут 
        равными 1. По умолчанию принимает значение 1.</font></td>
    </tr>
    <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><em><font face="Arial">nAllowDelete</font></em></td>
    <td width="71%" class="style2"><font face="Arial">числовое выражение, принимающее 
	значения 1 или 0, определяющее разрешение на удаление документа. Не имеет 
	смысла для бездокументных папок.</font></td>
    </tr>
  <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><em><font face="Arial">nAllowEdit</font></em></td>
    <td width="71%" class="style2"><font face="Arial">числовое выражение, принимающее 
	значения 1 или 0, <br>
    определяющее разрешение на корректировку документа. Не имеет смысла для 
	бездокументных папок.</font></td>
  </tr>
    <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2">

<font face="Arial"> <em>
nAllowEditUDR</em></font></td>
    <td width="71%" class="style2"><font face="Arial">числовое выражение, принимающее 
        значения 1 или 0, определяющее разрешение на корректировку документа. </font></td>
    </tr>
    <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><em><font face="Arial">nAllowExpro<span lang="ru">r</span>t</font></em></td>
    <td width="71%" class="style2"><font face="Arial">числовое выражение, принимающее 
	значения 1 или 0, определяющее разрешение на экспортирование документов 
	из вида просмотра. 
        </font></td>
    </tr>
    <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><em><font face="Arial">nAllow</font></em><font face="Arial"><em>History</em></font></td>
    <td width="71%" class="style2"><font face="Arial">числовое выражение, принимающее 
	значения 1 или 0, определяющее разрешение на <span lang="ru">просмотр лога 
	документа</span>. </font></td>
    </tr>
    <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><em><font face="Arial">nAllow</font></em><font face="Arial"><em>PrintPreview</em></font></td>
    <td width="71%" class="style2"><font face="Arial">числовое выражение, принимающее 
	значения 1 или 0, определяющее разрешение на <span lang="ru">просмотр 
	внутренней печатной формы документа</span>. </font></td>
    </tr>
    <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><em><font face="Arial">nAllowSecondEntry</font></em></td>
    <td width="71%" class="style2"><font face="Arial">числовое выражение, принимающее 
	значения 1 или 0, определяющее разрешение на вторичный ввод документа через 
	правую клавишу мыши. Не имеет смысла для бездокументных папок.</font></td>
    </tr>
  <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><em><font face="Arial">nAllowView</font></em></td>
    <td width="71%" class="style2"><font face="Arial">числовое выражение, принимающее 
	значения 1 или 0, <br>
    определяющее разрешение на просмотр документа. Не имеет смысла для 
	бездокументных папок.</font></td>
  </tr>
    <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><em><font face="Arial">nAllow</font></em><font face="Arial"><em>ViewDocChildren</em></font></td>
    <td width="71%" class="style2"><font face="Arial">числовое выражение, принимающее 
	значения 1 или 0, определяющее разрешение на<span lang="ru"> просмотр списка 
	дочерних документов</span>. </font></td>
    </tr>
    <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><em><font face="Arial">nAllow</font></em><font face="Arial"><em>ViewDocParents</em></font></td>
    <td width="71%" class="style2"><font face="Arial">числовое выражение, принимающее 
	значения 1 или 0, определяющее разрешение на<span lang="ru"> просмотр списка 
	    родительских документов</span>. </font></td>
    </tr>
  <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><em><font face="Arial">nAllowVisa</font></em></td>
    <td width="71%" class="style2"><font face="Arial">числовое выражение, принимающее 
	значения 1 или 0, определяющее разрешение на визирование документа через 
	правую клавишу мыши. Не имеет смысла для бездокументных папок.<span lang="ru">Кроме 
	того, чтобы визировать документ, нужно присутствие колонок</span> с 
	идентификатором<span lang="ru"> fISN </span>и 
	fFOLDERID <span lang="ru">среди <a href="../column.html">колонок источника данных</a>, указанного в <em>sViewSource</em>
	    .</span></font></td>
  </tr>
    <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><em><font face="Arial">sColorColName</font></em></td>
    <td width="71%" class="style2"><font face="Arial">строковое выражение 
	определяющее идентификатор цветоопределяющей колонки, содержащей 3-х 
	символьную комбинацию значений для определения&nbsp; жирности, курсива, кода 
	цвета строчки вида просмотра. 1-й символ значения определяет жирность (<strong>Bold</strong>) 
	фонта значений в текущей строчке. 2-й символ определяет курсив (<em>Italic</em>). 
	3-й символ определяет код цвета и принимает значения от 1 до 5. Например, 
	если для текущей строчки вида просмотра цветоопределяющая колонка содержит 
	значение &quot;001&quot;, это значит нету жирности и курсива, и выбран цвет под 
	номером 1 из настройки палитры системы (Ctrl+O). В источнике данных вида 
	просмотра цветоопределяющая колонка должна быть объявлена перманентной, 
	иметь тип C(3) и быть расчетной. Данное значение также влияет на цвет 
	колонки в <a href="../Functions/AsModalBrowser.html">произвольном 
	вспомогательном списке</a>.</font></td>
    </tr>
	<tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><font face="Arial"><em>nDisableDocFunctions<br />
        </em></font></td>
    <td width="71%" class="style2"><font face="Arial">числовое выражение, принимающее 
	значения 1 или 0, определяющее разрешение на использование функций документа из вида 
        просмотра.</font></td>
  </tr>
    <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><em><font face="Arial">nDocBased</font></em></td>
    <td width="71%" class="style2"><font face="Arial">числовое выражение, принимающее 
	значения 1 или 0, определяющее oснованность папки на документах. Применяется 
	когда в источнике данных существует колонка fISN (по которой надо 
	организовать обн<span lang="ru">о</span>вление), но она не соответствует некоторому документу в 
	хранилище.</font></td>
    </tr>
  <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><em><font face="Arial">nHelpContext</font></em></td>
    <td width="71%" class="style2"><font face="Arial">числовое выражение, 
	определяющее идентификатор контекстной помощи.&nbsp;</font></td>
  </tr>
    <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><em><font face="Arial">nShowOnBottom</font></em></td>
    <td width="71%" class="style2"><font face="Arial">числовое выражение, принимающее 
	значения 1 или 0, <br>
    определяющее признак установки маркера на последней строчке вида просмотра 
	при ее активации.</font></td>
    </tr>
  <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><em><font face="Arial">nSortSource</font></em></td>
    <td width="71%" class="style2"><font face="Arial">числовое выражение, принимающее 
	значения 1 или 0, устанавливающее источник сортировки колонок. Если 
	установлено значение 1, тогда строчки в виде просмотра будут расположены в 
	порядке полученном из источника данных и установки <strong>ORDER </strong>
	для колонки будут игнорированы. Если установлено значение 0, тогда колонки в 
	виде просмотра будут отсортированы исходя из описания колонок вида 
	просмотра. <a
    href="../Functions/ASVIEW/SQLSort.html">См.также</a></font></td>
  </tr>
  <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><em><font face="Arial">nVersion</font></em></td>
    <td width="71%" class="style2"><font face="Arial">численное выражение целого 
	типа, определяющее номер версии описания вида просмотра.</font></td>
  </tr>
  <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><em><font face="Arial">nUnMoveColCount</font></em></td>
    <td width="71%" class="style2"><font face="Arial">числовое выражение, 
	определяющее количество неподвижных колонок в виде просмотра. Отсчет 
	неподвижных колонок производится в соответствии с порядком описания колонок 
	в виде просмотра.</font></td>
  </tr>
    <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><em><font face="Arial">nUpdateStyle</font></em></td>
    <td width="71%" class="style2"><font face="Arial">численное выражение, 
	принимающее значения 1 или 0,<br>
    определяющее стиль обновления при редактировании документа из вида 
	просмотра(по ISN-у документа или общее обновление вида просмотра).</font></td>
    </tr>
    <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><em>

<font face="Arial">nUserDefined</font></em></td>
    <td width="71%" class="style2"><font face="Arial">числовое выражение, принимающее 
	значения 1 или 0, определяющее <span lang="ru">является ли вид просмора 
	пользовательским</span>. <span lang="ru">Пользовательские виды просмотра 
	разрешается редактировать</span>.</font></td>
    </tr>
  <tr>
    <td class="style2">
	<img src="../../../IMAGES/pubfield.gif" width="16" height="16">&nbsp;</td>
    <td width="29%" class="style2"><em><font face="Arial">sDocName</font></em></td>
    <td width="71%" class="style2"><font face="Arial">строковое выражение, в котором 
	перечислены&nbsp; идентификаторы тех <a
    href="doc.html">документов</a>, которые можно добавлять из данного вида 
	просмотра. Следует помнить, что необходимым условием для возможности 
	создания документа из вида просмотра является наличие в АРМ-е вида просмотра 
	описанной ветви для создания данного документа.</font></td>
  </tr>
	<tr>
    <td class="style4">
	<img src="../../../IMAGES/pubmethod.gif" width="16" height="11"></td>
    <td width="29%" class="style5"><font color="#000000" face="Arial">Subs and 
	Functions</font></td>
    <td width="71%" class="style4"><font face="Arial">скриптовый раздел описания, 
	который <span lang="ru">содержит </span>пользовательские процедуры и функции<span lang="ru">.</span></font></td>
  </tr>
</TBODY>
</table>

<p class="label">&nbsp;</p>

<p class="label"><b><font face="Arial">Примечаниеt></b></p>

<p class="label"><font face="Arial">Функция создания копии документа 
не срабатывает для тех типов документов, которые не перечислены в данном виде 
просмотра.</font></p>

<p class="label"><a href="../Defs.html"><font face="Arial">См. также</font></a></p>
</body>
</html>