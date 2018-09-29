<html>
<head>
<title>RunEx</title>
    <style type="text/css">
        .style1 {
            font-family: Arial;
        }
    </style>
</head>

<body>

<p><strong><font size="4" face="Arial">Метод RunEx</font></strong></p>

<p class="label"><font face="Arial">Вызывает процедуру из указанного 
модуля, проверяя существование процедуры. В случае отсутствия вызываемой 
процедуры в указанном модуле, сгенерируется ошибка. Среди возвращаемых значений 
    данного метода могут быть и ссылки на экземпляр объекта</font></p>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Синтаксис</b></font></p>

<p><font face="Arial"><strong>RunEx</strong>(<em>ModName, SubName, 
ParArray()</em>)</font></p>

<p><font face="Arial">Синтаксис метода <strong>RunEx</strong>
состоит из следующих частей:</font></p>

<table border="1" cellPadding="5" cols="2" frame="below" rules="rows">
<TBODY>
  <tr vAlign="top">
    <td class="label" width="29%"><font face="Arial"><b>Параметр</b></font></td>
    <td class="label" width="71%"><font face="Arial"><strong>Описание</strong></font></td>
  </tr>
  <tr>
    <td width="29%"><em><font face="Arial">ModName</font></em></td>
    <td width="71%"><font face="Arial">строковое выражение, 
	определяющее <a href="../../../Defs/Module.html">идентификатор модуля</a></font></td>
  </tr>
</TBODY>
  <tr>
    <td width="29%"><em><font face="Arial">SubName</font></em></td>
    <td width="71%"><font face="Arial">имя процедуры из указанного 
	модуля </font></td>
  </tr>
  <tr>
    <td width="29%"><em><font face="Arial">ParArray()</font></em></td>
    <td width="71%"><font face="Arial">массив параметров для 
	подстановки в процедуру. </font></td>
  </tr>
</table>

<p class="label">&nbsp;</p>

<p class="label"><b><font face="Arial">Примечание</font></b></p>

<p class="label"><font face="Arial">При использовании данного метода 
накладываются следующие ограничения:</font> 

<ul>
    <li>
        <p class="label">
            <font face="Arial">разрешается передача 
	ссылочных переменных (<strong>ByRef</strong>), с учетом возвращения их значений, если 
            типы этих переменных совпадают с типами процедуры или же имеют тип <strong>
            Variant</strong>.<br />
            <br />
            Например:<br />
            <br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1) </font><span class="style1">
            Dim param01 As <strong>Long</strong></span><br class="style1" />
            <span class="style1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;RunEx(&quot;modname&quot;,&quot;methodname1&quot;, param01) </span>
            <br class="style1" />
            <br class="style1" />
            <span class="style1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Sub methodname1(ByRef param01 As <strong>Integer</strong>)</span><br 
                class="style1" />
            <span class="style1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
            ...</span><br class="style1" />
            <span class="style1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;End Sub</span><br class="style1" />
            <br class="style1" />
            <span class="style1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2) Dim 
            param01 As <strong>Long</strong></span><br class="style1" />
            <span class="style1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
            RunEx(&quot;modname&quot;,&quot;methodname2&quot;, param01) </span>
            <br class="style1" />
&nbsp;<br class="style1" />
            <span class="style1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
            Sub methodname2(ByRef param01 As <strong>Long</strong>)</span><br 
                class="style1" />
            <span class="style1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
            ...</span><br class="style1" />
            <span class="style1">&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
            End Sub</span><br class="style1" />
            <br class="style1" />
            <span class="style1">В первом примере 
            значение параметра <strong>param01</strong>
            не будет возвращено, поскольку тип <strong>param01-&gt;Long</strong>, а тип
            соответствующего параметра процедуры <strong>Integer</strong>. Во-втором 
            примере значение возвратится, т.к. типы у обоих парамeтров совпадают и равны
            <strong>Long</strong></span></p>
    </li>
  <li><p class="label"><font face="Arial">при задании необязательных параметров 
      предыдущие необязательные параметры должны быть заполнены.
      <br />
      <br />
      Например:<span class="style1"><br />
      <br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 1) 
      RunEx(&quot;modname&quot;,&quot;methodname&quot;, param1, , Param3)
      <br />
      <br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sub methodname(ByVal param1 As 
      Long<strong>,&nbsp;Optional</strong> ByVal param2 As Long, <strong>Optional</strong> 
      ByVal param3 As Long)<br class="style1" />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
      ...<br class="style1" />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; End Sub<br />
      <br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2) RunEx(&quot;modname&quot;,&quot;methodname&quot;, param1)
      <br />
      <br />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Sub methodname(ByVal param1 As 
      Long,&nbsp;<strong>Optional</strong> ByVal param2 As Long, <strong>Optional</strong> 
      ByVal param3 As Long)<br class="style1" />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
      ...<br class="style1" />
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; End Sub<br />
      </span>
      <br>В первом примере задание параметра <span class="style1">param2 обязательно, поскольку после него 
      задается&nbsp;еще параметр 
      Param3, а во-втором примере - необязательно.</span></font></p>
  </li>
</ul>

<p class="label"><a href="../../../functions.html"><font face="Arial">
См. также</font></a></p>
</body>
</html>