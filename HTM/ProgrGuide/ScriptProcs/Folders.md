﻿<html>
<head>
<title>Системное событие Folders</title>
</head>

<body>

<p><strong><font size="4" face="Arial">Событие Folders<br>
<br>
</font></strong><font face="Arial"><a href="../scriptstproced.html">См. 
также</a>&nbsp; <a href="../Examples/E_Folders.html">Пример</a>&nbsp; <a
href="../Defs/doc.html">Применяется к</a></font></p>

<p class="label"><font face="Arial">Генерируется системой для 
размещения документа в папках и деревьях. Происходит также при использовании 
методов&nbsp;&nbsp; <a
href="../Functions/ASDOC/Store.html">Store</a> или <a
href="../Functions/ASDOC/CheckAndStore.html">CheckAndStore</a>. Оно выполняется в 
режиме включенной транзакции. При сохранении документа в папке&nbsp; черновых 
документов, данное событие не срабатывает. <br>
Последовательность генерации системных событий для документа приведена здесь <a href="Events_Sequence.html"><img
src="../../../IMAGES/More.gif" width="12" height="12" alt="More.gif (304 bytes)"
border="0"></a>.</font></p>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Синтаксис</b></font></p>

<p><font face="Arial">Sub <strong>Folders</strong>()<br>
<em>&nbsp;&nbsp;&nbsp;statements</em><br>
End Sub</font></p>

<p class="label">&nbsp;</p>

<p class="label"><font face="Arial"><b>Примечание</b></font></p>

<p class="label"><font face="Arial">В обработчике события <strong>
Folders
</strong>вызываются методы <a href="../Functions/ASDOC/StoreInFolder.html">
StoreInFolder</a>
и <a href="../Functions/ASDOC/StoreInTree.html">StoreInTree</a>.</font></p>
</body>
</html>