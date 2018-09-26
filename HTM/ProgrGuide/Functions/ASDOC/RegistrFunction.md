﻿<html>
<head>
<title>Документ\RegistrFunction</title>
    <style type="text/css">
        .style1 {
            font-family: Arial;
        }
    </style>
</head>

<body>

<p><strong><font size="4" face="Arial">Метод RegistrFunction<br>
</font></strong><font face="Arial"><br>
<a href="../Asdoc.html">См. также</a>&nbsp; <u>Пример</u>&nbsp; <a
href="../Asdoc.html">Применяется к</a></font></p>

<p><font face="Arial">Добавляет в контекстное меню вызов 
пользовательской функции. Данный метод обеспечивает выполнение пользовательской 
функции из любого вида просмотра, где находится документ.</font></p>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Синтаксис</b></font></p>

<p><font face="Arial"><em>object</em><strong>.RegistrFunction</strong>(<em>Caption,
</em>[<em>RunSub</em>]<em>, </em>[<em>AccessCode</em>]<em>, </em>[<em>ParentId</em>]<em>, </em>
[<em>ECaption</em>], [AvailableFor], [FuncParam])</font></p>

<p><font face="Arial">Синтаксис метода <strong>RegistrFunction</strong>
состоит из следующих частей:</font></p>

<table border="1" cellPadding="5" cols="2" frame="below" rules="rows">
<TBODY>
  <tr vAlign="top">
    <td class="label" width="29%"><font face="Arial"><b>Параметр</b></font></td>
    <td class="label" width="79%"><font face="Arial"><strong>Описание</strong></font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>object</em></font></td>
    <td width="79%"><font face="Arial">строковое выражение, являющееся 
	ссылкой на экземпляр документа</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>Caption</em></font></td>
    <td width="79%"><font face="Arial">строковое выражение, определяющее заголовок 
        функции добавляемой в контекстное меню. Значение &quot;-&quot; 
	данного выражения означает добавление в меню, разделительной линии. </font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>RunSub</em></font></td>
    <td width="79%"><font face="Arial">необязательное строковое выражение, определяющее 
        либо &quot;имя функции&quot;, либо &quot;имя модуля.имя функции&quot;, вызываемое при выборе данной строчки 
	в контекстном меню. Если данный параметр не задан, то в контекстное меню 
	добавляется разделитель.</font></td>
  </tr>
</TBODY>
  <tr>
    <td width="29%"><font face="Arial"><em>AccessCode</em></font></td>
    <td width="79%"><font face="Arial">необязательное строковое 
	выражение, определяющее идентификаторы рабочих мест на которых срабатывает 
	данный вызов. При перечислении нескольких идентификаторов АРМ-ов они 
	отделяются друг от друга символами &quot;;&quot;. Для пользователя, имеющего доступ 
	хотя бы к одному из перечисленных АРМ-ов, данная функция будет доступна из 
	всех АРМ-ов (даже не перечисленных!), где данный документ фигурирует.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>ParentId</em></font></td>
    <td width="79%"><font face="Arial">необязательное строковое 
	выражение, определяющее ссылку <a
    href="RegistrNode.html">на идентификатор узла</a> дерева контекстных вызовов.</font></td>
  </tr>
  <tr>
    <td width="29%"><font face="Arial"><em>ЕCaption</em></font></td>
    <td width="79%"><font face="Arial">необязательное строковое выражение, определяющее 
        запись добавляемой в контекстное меню функции на 
	иностранном языке. По умолчанию значение равно <em>Caption.</em></font></td>
  </tr>
    <tr>
    <td width="29%"><font face="Arial"><em>AvailableFor</em></font></td>
    <td width="79%"><font face="Arial">необязательное цифровое 
	выражение, определяющее 
	<a href="../../Constants/const_RegistrFunctionAvailability.html">константу 
	видимости и иконку</a> контекстного меню.</font></td>
    </tr>
<tr>
    <td width="29%"><font face="Arial"><em>FuncParam</em></font></td>
    <td width="79%"><font face="Arial">необязательное выражение типа 
        Variant, определяющее параметр для функции заданной параметром <em>RunSub.</em></font></td>
  </tr>
</table>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Примечание</b></font></p>

<p class="label"><font face="Arial">Данный метод должен быть вызван в 
обработчике системного события
<a href="../../ScriptProcs/FunctionsDoc.html">Functions</a>. Функция, срабатывающая 
    при вызове, может быть описана либо в скриптовой части
    <a href="../../Defs/doc.html">
    документа</a>,&nbsp;либо в скриптовой части <a href="../../Defs/Module.html"> модуля</a>. 
    Если описание функции находится в скриптовой части документа, то после его 
    вызова срабатывает метод <a href="../FrmPttel/Update.html"> Update</a>&nbsp;по ISN-у 
    документа, для которого она вызывается, в противном случае метод
    <a href="../FrmPttel/Update.html"> Update</a> не сработает.</font></p>
    <p class="style1">Рассмотрим следующие два примера:</p>
    <p class="style1">&nbsp;1.
        <span class="style1">
        <br />
        &#39; Скриптовая часть<em> Doc-а</em></span><br />
&nbsp; Sub Functions<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Doc.RegistrFunction &quot;Operation&quot;, 
        &quot;<strong>OperFunc</strong>&quot;<br />
&nbsp;&nbsp; End Sub<br />
&nbsp;&nbsp; Sub <strong>OperFunc</strong>()<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Doc(&quot;Rekv&quot;) = &quot;AAA&quot;<br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Doc.Storе<br />
&nbsp;&nbsp; End Sub<br />
        <br />
        2.
        <br />
        <span class="style1">&#39; &nbsp;Скриптовая часть<em> Doc-а</em></span><br class="style1" />
        <span class="style1">&nbsp; Sub Functions </span>
        <br class="style1" />
        <span class="style1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Doc.RegistrFunction &quot;Operation&quot;, 
        &quot;<strong>Module.OperFunc</strong>&quot;</span><br class="style1" />
        <span class="style1">&nbsp; End Subոո</span><br class="style1" />
&nbsp;<br class="style1" />
        <span class="style1">&#39; Скриптовая часть <em>Modulе-я</em></span><br class="style1" />
        <span class="style1">&nbsp; Sub           <strong>OperFunc</strong>()</span><br class="style1" />
        <span class="style1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Doc(&quot;Rekv&quot;) = &quot;AAA&quot;</span><br 
            class="style1" />
        <span class="style1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Doc.Store</span><br class="style1" />
        <span class="style1">&nbsp; End Subb<br />
        <br Здесь, после вызова <font face="Arial">В первом примере описание функции 
        находится в скриптовой части дукумента, во втором примере находится в скриптовой части 
        модуля. При первом примере после <font face="Arial">
        вызова функции сработает метод <a href="../FrmPttel/Update.html"> Update</a>, при 
        втором примере не сработает</font>.</span></p>
    <p class="style1">&nbsp;</p>
    <p class="label">&nbsp;</p>
    <p class="label">&nbsp;</p>

<p class="label">&nbsp;</p>
</body>
</html>