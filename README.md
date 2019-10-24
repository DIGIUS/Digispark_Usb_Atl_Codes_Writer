<p><span style="font-size:14px"># DigisparkUSBwriter<br />
<strong>Код написан (если можно это назвать кодом) и отлажен за пару вечеров, если хотите его оптимизировать и улучшить то я буду только рад.&nbsp;</strong><br />
Прошивка вводит текст в целевую систему&nbsp;через&nbsp;плату&nbsp;<strong>Digispark</strong>&nbsp;&nbsp;используя Alt Коды (<strong><span style="color:#FF0000">Only Windows</span></strong> (<strong>проверено на <span style="color:#008000">Win 7, WIn 10</span></strong>), <strong><span style="color:#008000">работает без учёта Numlock и вне зависимости от установленного языка</span></strong>)</span><br />
<span style="font-size:16px"><strong>Возможности данной прошивки:</strong></span><br />
&nbsp; &nbsp;<span style="font-size:14px"> Вызов CMD.<br />
&nbsp; &nbsp; Ввод текста на английском, символы доступные для ввода:&nbsp;</span></p>

<ul>
	<li><span style="font-size:14px">&nbsp;abcdefghijklmnopqrstuvwxyz</span></li>
	<li><span style="font-size:14px">ABCDEFGHIJKLMNOPQRSTUVWXYZ</span></li>
	<li><span style="font-size:14px">[]\/^&#39;_(){}`&quot;@?&lt;&gt;=;:.,+-*!</span></li>
	<li><span style="font-size:14px">1234567890</span></li>
	<li><span style="font-size:14px">символ | используеться для эмуляции нажатия enter</span></li>
	<li><span style="font-size:14px">&nbsp;пробел (&quot; &quot;) используеться как побел (логично)</span></li>
</ul>

<p><span style="font-size:16px"><strong>Описание кода:</strong></span><br />
<span style="font-size:14px"><strong>&nbsp;Процедура<u> st(char sm)</u></strong><br />
&nbsp; В качестве переменной <strong><u><span style="color:#FF0000">передаётся только один символ</span></u></strong> типа char,&nbsp;<br />
&nbsp;Пример вызова:&nbsp;&nbsp;<strong>st(&#39;T&#39;);</strong>&nbsp; введёт&nbsp; в систему букву T один раз.</span></p>

<p><br />
<span style="font-size:14px"><strong>&nbsp;Процедура <u>cmd()</u></strong><br />
&nbsp; Открывает коммандную строку по&nbsp; принципу:&nbsp;</span></p>

<ol>
	<li><span style="font-size:14px">&nbsp;Эмулирует нажатие win+r</span></li>
	<li><span style="font-size:14px">Ждёт секунду (1000 милисекунд)</span></li>
	<li><span style="font-size:14px">Вводит cmd и нажимает enter&nbsp;</span></li>
	<li><span style="font-size:14px">Ждёт 3 секунды&nbsp;(3000 милисекунд) и завершает свою работу</span></li>
</ol>

<p><span style="font-size:14px">Тайминг выбран из головы, в зависимости от целевой машины можете их менять.</span></p>

<p>&nbsp;</p>

<p><span style="font-size:14px"><strong>&nbsp; Процедура&nbsp;<u>po()</u></strong></span></p>

<p><span style="font-size:14px">Пассивная процедура, используется в коде для отключения всех ранее нажатых клавиш кроме ALT.</span></p>

<p>&nbsp;</p>

<p><span style="font-size:14px">&nbsp;<u><strong>Процедура&nbsp;nl()</strong></u></span></p>

<p><span style="font-size:14px">Выполняет функционал что и процедура выше.</span></p>

<p>&nbsp;</p>

<p><span style="font-size:14px">&nbsp;<strong>Процедура keyp(byte o, byte t)</strong></span></p>

<p><span style="font-size:14px">Используется для ввода Alt кодов из процедуры <strong>st()</strong>, изначальная история создания данной процедуры заключаеться в сокращении занимаемого места в памяти микроконтроллера.</span></p>

<p>&nbsp;</p>

<p><span style="font-size:16px"><strong>Использование:</strong></span></p>

<p>Для создания на локальном диске текстового документа с текстом Hello User нам понадобиться код конвертор на js:</p>

<pre>
jjjjj</pre>

<p>&nbsp;</p>

<p>&nbsp;</p>

<p>&nbsp;</p>
