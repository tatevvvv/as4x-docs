﻿<html>
<head>
<title>Документ\Control</title>
</head>

<body>

<p><font face="Arial"><font size="4"><strong>Свойство Control<br>
<br>
</strong></font><a href="../Asdoc.html">См. также</a>&nbsp; <u>Пример</u>&nbsp;
<a href="../Asdoc.html">Применяется к</a></font></p>

<p class="label"><font face="Arial">Возвращает ссылку на 
осуществляюший ввод элемент управления. Свойство имеет смысл применять при 
визуальных обработках документа, при фоновой обработке загруженного документа 
данное свойство неприменимо.</font></p>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Синтаксис</b></font></p>

<p><font face="Arial"><em>object.</em><strong>Control(</strong><em>RekvName</em><strong>).</strong><em>PropName</em></font></p>

<p><font face="Arial">Синтаксис свойства <strong>Control</strong>
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
    <td width="29%"><font face="Arial"><em>RekvName</em></font></td>
    <td width="71%"><font face="Arial">выражение типа вариант, 
	определяющее идентификатор реквизита документа</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>PropName</em></font></td>
    <td width="71%"><font face="Arial">строковое выражение, 
	определяющее свойство реквизита. В зависимости от <a href="../../types.html">
	внутреннего типа реквизита</a>
    становятся доступными различные наборы свойств.</font></td>
  </tr>
</TBODY>
</table>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial">Ниже приводятся свойства, 
доступные через Control, для различных типов реквизитов документа:</font></p>

<p class="label"><font face="Arial"><a href="../../Types/Folder().html">
Folder()</a>:</font></p>

<table border="1" cellPadding="5" cols="2" frame="below" rules="rows">
  <tr vAlign="top">
    <td class="label" width="29%"><b><font face="Arial">Свойство</font></b></td>
    <td class="label" width="71%"><font face="Arial"><strong>Описание</strong></font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">AsType</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	внутренний тип реквизита. Тип значения свойства - строка.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Button</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	наличие кнопки выбора значения реквизита из списка. Тип значения свойства - 
	логическое выражение.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Caption</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	заголовок вспомогательного списка выбора. Тип значения свойства - строка.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Comment</font></td>
    <td width="71%"><font face="Arial">Возвращает комментарий 
	выбранного элемента папки. Тип значения свойства - строка.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">DlinaKey</font></td>
    <td width="71%"><font face="Arial">Возвращает длину ключа элемента 
	папки. Тип значения свойства - целое число.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Enabled</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	признак доступности реквизита. Тип значения свойства - логическое выражение.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">FolderID</font></td>
    <td width="71%"><font face="Arial">Возвращает идентификатор папки 
	для выбранного элемента папки. Тип значения свойства - строка.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">ISN</font></td>
    <td width="71%"><font face="Arial">Возвращает внутрисистемный ISN 
	выбранного значения элемента папки. Тип значения свойства - длинное целое 
	число.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Key</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	ключевое значение выбранного элемента папки. При установке нового значения, 
	в поле реквизита заменяется ранее выбранное значение. Тип значения свойства 
	- строка.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">ReadOnly</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает режим 
	редактирования реквизита. Тип значения свойства - логическое выражение.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">ShowName</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	признак показа комментария справа от значения выбранного реквизита. Тип 
	значения свойства - логическое выражение.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Validate</font></td>
    <td width="71%"><font face="Arial">Возвращает признак неверного 
	ввода значения в реквизит. Если значение свойства True тогда активным 
	остается данный реквизит, до ввода допустимого значения. А если значением 
	свойства является False, то управление передается следующим реквизитам. Тип 
	значения свойства - логическое выражение.</font></td>
  </tr>
</table>

<p class="label"><font face="Arial"><a href="../../Types/Tree().html">
Tree()</a>,
<a href="../../Types/FULLTREE().html">FullTree()</a>:</font></p>

<table border="1" cellPadding="5" cols="2" frame="below" rules="rows">
  <tr vAlign="top">
    <td class="label" width="29%"><font face="Arial"><b>Свойство</b></font></td>
    <td class="label" width="71%"><font face="Arial"><strong>Описание</strong></font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">AsType</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	внутренний тип реквизита. Тип значения свойства - строка.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Button</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	наличие кнопки выбора значения реквизита из списка. Тип значения свойства - 
	логическое выражение.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Code</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает ключ 
	элемента в дереве. При установке нового значения, в поле реквизита 
	заменяется ранее выбранное значение. Тип значения свойства - логическое 
	выражение.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Comment</font></td>
    <td width="71%"><font face="Arial">Возвращает комментарий 
	выбранного элемента дерева. Тип значения свойства - строка.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Enabled</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	признак доступности реквизита. Тип значения свойства - логическое выражение.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">ISN</font></td>
    <td width="71%"><font face="Arial">Возвращает внутрисистемный ISN 
	выбранного значения элемента папки. Тип значения свойства - длинное целое 
	число.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Path</font></td>
    <td width="71%"><font face="Arial">Возвращает путь элемента в 
	дереве, начиная с корня дерева. Тип значения свойства - строка.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">ReadOnly</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает режим 
	редактирования&nbsp; реквизита. Тип значения свойства - логическое выражение.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">ShowName</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	признак показа комментария справа от значения выбранного реквизита. Тип 
	значения свойства - логическое выражение.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">TreeID</font></td>
    <td width="71%"><font face="Arial">Возвращает идентификатор дерева 
	для выбранного элемента дерева. Тип значения свойства - строка.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Validate</font></td>
    <td width="71%"><font face="Arial">Возвращает признак неверного 
	ввода значения в реквизит. Если значение свойства True тогда активным 
	остается данный реквизит, до ввода допустимого значения. А если значением 
	свойства является False, то управление передается следующим реквизитам. Тип 
	значения свойства - логическое выражение.</font></td>
  </tr>
</table>

<p><font face="Arial"><a href="../../Types/Amacc.html">AmAcc()</a>:</font></p>

<table border="1" cellPadding="5" cols="2" frame="below" rules="rows">
  <tr vAlign="top">
    <td class="label" width="29%"><font face="Arial"><b>Свойство</b></font></td>
    <td class="label" width="71%"><font face="Arial"><strong>Описание</strong></font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Acc</font></td>
    <td width="71%"><font face="Arial">Возвращает код внутреннего 
	счета для значения реквизита. Тип значения свойства - строка.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">AccName</font></td>
    <td width="71%"><font face="Arial">Возвращает наименование счета 
	для значения реквизита. Тип значения свойства - строка.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">AsType</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	внутренний тип реквизита. Тип значения свойства - строка.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Bank</font></td>
    <td width="71%"><font face="Arial">Возвращает код банка для 
	значения реквизита. Тип значения свойства - строка.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">BankName</font></td>
    <td width="71%"><font face="Arial">Возвращает наименование банка 
	для значения реквизита. Тип значения свойства - строка.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Button</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	признак видимости кнопок выбора. Тип значения свойства - логическое 
	выражение.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Enabled</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	признак доступности реквизита. Тип значения свойства - логическое выражение.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">FullAcc</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	значение всего структурного лицевого счета реквизита. Тип значения свойства 
	- строка.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">ReadOnly</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает режим 
	редактирования&nbsp; реквизита. Тип значения свойства - логическое выражение.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Validate</font></td>
    <td width="71%"><font face="Arial">Возвращает признак неверного 
	ввода значения в реквизит. Если значение свойства True тогда активным 
	остается данный реквизит, до ввода допустимого значения. А если значением 
	свойства является False, то управление передается следующим реквизитам. Тип 
	значения свойства - логическое выражение.</font></td>
  </tr>
</table>

<p><font face="Arial"><a href="../../Types/NumPair().html">NumPair()</a>:</font></p>

<table border="1" cellPadding="5" cols="2" frame="below" rules="rows">
  <tr vAlign="top">
    <td class="label" width="29%"><font face="Arial"><b>Свойство</b></font></td>
    <td class="label" width="71%"><font face="Arial"><strong>Описание</strong></font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">AsType</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	внутренний тип реквизита. Тип значения свойства - строка.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Comment</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	комментарий для набранного курса. Комментарий располагается справа от 
	значений курса. Максимальная длина 10 символов. Тип значения свойства - 
	строка.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Enabled</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	признак доступности реквизита. Тип значения свойства - логическое выражение.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">LabelCaption</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	разделитель между ценой и количеством валюты. Максимальная длина разделителя 
	не ограничена. Тип значения свойства - строка.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Number1</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	значение первого числа. Тип значения свойства - Currency.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Number2</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	значение второго числа. Тип значения свойства - Currency.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">ReadOnly</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает режим 
	редактирования&nbsp; реквизита. Тип значения свойства - логическое выражение.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Validate</font></td>
    <td width="71%"><font face="Arial">Возвращает признак неверного 
	ввода значения в реквизит. Если значение свойства True тогда активным 
	остается данный реквизит, до ввода допустимого значения. А если значением 
	свойства является False, то управление передается следующим реквизитам. Тип 
	значения свойства - логическое выражение.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Value</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	значение реквизита типа курс, в виде структурной строки вида:&nbsp; &quot;цена / 
	количество&quot;. Тип значения свойства - строка.</font></td>
  </tr>
  <tr>
    <td width="29%"><a name="ZeroNumber1"><font face="Arial">
	ZeroNumber1</font></a></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	возможность ввода нулевого значения в первое число. Тип значения свойства - 
	логическое выражение.</font></td>
  </tr>
  <tr>
    <td width="29%"><a name="ZeroNumber2"><font face="Arial">
	ZeroNumber2</font></a></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	возможность ввода нулевого значения во второе число. Тип значения свойства - 
	логическое выражение.</font></td>
  </tr>
</table>

<p><font face="Arial">Image</font></p>

<table border="1" cellPadding="5" cols="2" frame="below" rules="rows">
  <tr vAlign="top">
    <td class="label" width="29%"><font face="Arial"><b>Свойство</b></font></td>
    <td class="label" width="71%"><font face="Arial"><strong>Описание</strong></font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Enabled</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	признак доступности реквизита. Тип значения свойства - логическое выражение.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Picture</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	значение реквизита в виде байтового массива. Тип значения свойства - 
	Variant.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">ReadOnly</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает режим 
	редактирования&nbsp; реквизита. Тип значения свойства - логическое выражение.</font></td>
  </tr>
</table>

<p><font face="Arial"><a href="../../Types/Ch().html">CH()</a>:</font></p>

<table border="1" cellPadding="5" cols="2" frame="below" rules="rows">
  <tr vAlign="top">
    <td class="label" width="29%"><font face="Arial"><b>Свойство</b></font></td>
    <td class="label" width="71%"><font face="Arial"><strong>Описание</strong></font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">AsType</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	внутренний тип реквизита. Тип значения свойства - строка.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Code</font></td>
    <td width="71%"><font face="Arial">Возвращает ключевой код для 
	выбранного элемента из дерева комментариев. Тип значения свойства - строка.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Comment</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	комментарий для выбранного элемента из дерева комментариев. Тип значения 
	свойства - строка.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">DlinaKey</font></td>
    <td width="71%"><font face="Arial">Возвращает длину ключа элемента 
	дерева комментариев. Тип значения свойства - целое число.</font></td>
  </tr>
    <tr>
    <td width="29%"><font face="Arial">Enabled</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	признак доступности реквизита. Тип значения свойства - логическое выражение.</font></td>
    </tr>
  <tr>
    <td width="29%"><font face="Arial">Label<br />
        </font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает 
	    пометку для выбранного элемента из дерева комментариев. Тип значения свойства - 
        строка.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">ReadOnly</font></td>
    <td width="71%"><font face="Arial">Возвращает/устанавливает режим 
	редактирования&nbsp; реквизита. Тип значения свойства - логическое выражение.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">TreeID</font></td>
    <td width="71%"><font face="Arial">Возвращает идентификатор дерева 
	для выбранного элемента. Тип значения свойства - строка.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial">Validate</font></td>
    <td width="71%"><font face="Arial">Возвращает признак неверного 
	ввода значения в реквизит. Если значение свойства True тогда активным 
	остается данный реквизит, до ввода допустимого значения. А если значением 
	свойства является False, то управление передается следующим реквизитам. Тип 
	значения свойства - логическое выражение.</font></td>
  </tr>
</table>
</body>
</html>