

<table class=MsoNormalTable border=1 cellspacing=0 cellpadding=0
 style='margin-left:11.05pt;border-collapse:collapse;border:none;mso-border-alt:
 solid windowtext .5pt;mso-padding-alt:0cm 5.4pt 0cm 5.4pt;mso-border-insideh:
 .5pt solid windowtext;mso-border-insidev:.5pt solid windowtext'>
 <tr style='mso-yfti-irow:0;mso-yfti-firstrow:yes;mso-yfti-lastrow:yes;
  height:682.35pt'>
  <td width=737 valign=top style='width:442.25pt;border:solid windowtext 1.0pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt;height:682.35pt'>
  <h2 align=center style='margin-bottom:6.6pt;text-align:center;background:
  white'><span style='font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:#24292E'>Аппаратный API дронпоинт2<o:p></o:p></span></h2>
  <p style='margin-top:0cm;margin-right:0cm;margin-bottom:6.6pt;margin-left:
  0cm;text-align:justify;background:white;box-sizing: border-box;font-variant-ligatures: normal;
  font-variant-caps: normal;orphans: 2;text-align:start;widows: 2;-webkit-text-stroke-width: 0px;
  text-decoration-thickness: initial;text-decoration-style: initial;text-decoration-color: initial;
  word-spacing:0px'><span style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI";color:#24292E'><span
  style='mso-spacerun:yes'>             </span>Плата управления аппаратурой&nbsp;<strong
  style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>дронпоинт2</span></strong>&nbsp;построена на
  микроконтроллере <strong><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>stm32F103ZET6</span></strong>. <span
  style='mso-spacerun:yes'> </span>Обмен данными с верхними программными
  уровнями осуществляется по USB, а конкретней через реализацию&nbsp;<strong
  style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>Maple Serial(COM порт).</span></strong>&nbsp;Для
  приема команд и отсылки данных по&nbsp;<strong style='box-sizing: border-box'><span
  style='font-family:"Calibri Light","sans-serif";mso-bidi-font-family:"Segoe UI"'>uart(COM
  порт)</span></strong>&nbsp;используется протокол&nbsp;<strong
  style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>JSON</span></strong>.<br style='box-sizing: border-box'>
  Имеются следующие группы команд:<o:p></o:p></span></p>
  <p style='margin-top:6.6pt;margin-right:0cm;margin-bottom:6.6pt;margin-left:
  36.0pt;text-indent:-18.0pt;mso-list:l1 level1 lfo2;tab-stops:list 36.0pt;
  background:white;box-sizing: border-box'><![if !supportLists]><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-fareast-font-family:
  "Calibri Light";mso-bidi-font-family:"Calibri Light";color:#24292E'><span
  style='mso-list:Ignore'>1.<span style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;
  </span></span></span><![endif]><strong style='box-sizing: border-box'><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:#24292E'>Команды перемещения каретки</span></strong><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:#24292E'>, навигация по ячейкам.<o:p></o:p></span></p>
  <p style='margin-top:6.6pt;margin-right:0cm;margin-bottom:6.6pt;margin-left:
  36.0pt;text-align:justify;text-indent:-18.0pt;mso-list:l1 level1 lfo2;
  tab-stops:list 36.0pt;background:white;box-sizing: border-box'><![if !supportLists]><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-fareast-font-family:
  "Calibri Light";mso-bidi-font-family:"Calibri Light";color:#24292E'><span
  style='mso-list:Ignore'>2.<span style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;
  </span></span></span><![endif]><strong style='box-sizing: border-box'><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:#24292E'>Команды специальных операций</span></strong><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:#24292E'>. Это допустим загрузка или выгрузка контейнера в ячейку,
  установка контейнера в коптер и.т.д.<o:p></o:p></span></p>
  <p style='margin-top:6.6pt;margin-right:0cm;margin-bottom:6.6pt;margin-left:
  36.0pt;text-align:justify;text-indent:-18.0pt;mso-list:l1 level1 lfo2;
  tab-stops:list 36.0pt;background:white;box-sizing: border-box'><![if !supportLists]><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-fareast-font-family:
  "Calibri Light";mso-bidi-font-family:"Calibri Light";color:#24292E'><span
  style='mso-list:Ignore'>3.<span style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;
  </span></span></span><![endif]><strong style='box-sizing: border-box'><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:#24292E'>Команды тестирования</span></strong><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:#24292E'>&nbsp;отдельных элементов и сценариев. Можно
  использовать для управления какими-то отдельными исполнительными механизмами.
  Допустим пощелкать соленоидом отсека выдачи, открыть или закрыть замок
  контейнера на коптере, открыть или закрыть замок крышки зарядки, то-есть это
  те простые<br style='box-sizing: border-box'>
  операции которые входят в состав более сложных команд специальных операций. Также
  сюда входят сценарии тест оси Z, тест оси X, комплексное перемещение по различным
  ячейкам с погрузкой и выгрузкой контейнера и.т.д.<o:p></o:p></span></p>
  <p style='margin-top:6.6pt;margin-right:0cm;margin-bottom:6.6pt;margin-left:
  36.0pt;text-align:justify;text-indent:-18.0pt;mso-list:l1 level1 lfo2;
  tab-stops:list 36.0pt;background:white;box-sizing: border-box'><![if !supportLists]><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-fareast-font-family:
  "Calibri Light";mso-bidi-font-family:"Calibri Light";color:#24292E'><span
  style='mso-list:Ignore'>4.<span style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;
  </span></span></span><![endif]><strong style='box-sizing: border-box'><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:#24292E'>Команды посадочному столу</span></strong><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:#24292E'>. Исполнительным механизмом посадочного стола является
  механизм позиционирования. Он выполняет функцию центрирования коптера после
  посадки т.е. выставляет его точно над верхним люком, точное положение коптера
  очень важно для операций установки и снятия контейнера.<br style='mso-special-character:
  line-break;box-sizing: border-box'>
  <![if !supportLineBreakNewLine]><br style='mso-special-character:line-break'>
  <![endif]><o:p></o:p></span></p>
  <p align=center style='margin-top:6.6pt;margin-right:0cm;margin-bottom:6.6pt;
  margin-left:36.0pt;text-align:center;background:white;box-sizing: border-box'><span
  style='font-size:6.5pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:#24292E'><br style='mso-special-character:line-break'>
  <![if !supportLineBreakNewLine]><br style='mso-special-character:line-break'>
  <![endif]></span><span style='font-size:16.0pt;font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI";color:#24292E'><o:p></o:p></span></p>
  <h3 align=center style='margin-top:9.95pt;margin-right:0cm;margin-bottom:
  6.6pt;margin-left:0cm;text-align:center;background:white;box-sizing: border-box;
  font-variant-ligatures: normal;font-variant-caps: normal;orphans: 2;
  text-align:start;widows: 2;-webkit-text-stroke-width: 0px;text-decoration-thickness: initial;
  text-decoration-style: initial;text-decoration-color: initial;word-spacing:
  0px'><span style='font-size:16.0pt;line-height:115%;font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>Команды перемещения каретки<o:p></o:p></span></h3>
  <p style='margin-top:0cm;margin-right:0cm;margin-bottom:6.6pt;margin-left:
  0cm;background:white;box-sizing: border-box;font-variant-ligatures: normal;
  font-variant-caps: normal;orphans: 2;text-align:start;widows: 2;-webkit-text-stroke-width: 0px;
  text-decoration-thickness: initial;text-decoration-style: initial;text-decoration-color: initial;
  word-spacing:0px'><span style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI";color:#24292E'><span
  style='mso-spacerun:yes'>        </span>Команда перемещения каретки может
  иметь следующий вид<br style='box-sizing: border-box'>
  </span><strong style='box-sizing: border-box'><span style='font-size:14.0pt;
  font-family:"Calibri Light","sans-serif";mso-bidi-font-family:"Segoe UI";
  color:red'>{&quot;command&quot;: &quot;goto_cell&quot;, &quot;params&quot;:
  {&quot;x&quot;: 2, &quot;y&quot;: 2, &quot;z&quot;: 1}}</span></strong><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:#24292E'><br style='box-sizing: border-box'>
  Команда&nbsp;</span><strong style='box-sizing: border-box'><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:red'>goto_cell</span></strong><span style='font-size:14.0pt;
  font-family:"Calibri Light","sans-serif";mso-bidi-font-family:"Segoe UI";
  color:#24292E'>&nbsp;имеет следующий набор параметров:<br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'><span style='mso-spacerun:yes'>     </span></span></strong></span><strong><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:red'>Z</span></strong><span style='font-size:14.0pt;
  font-family:"Calibri Light","sans-serif";mso-bidi-font-family:"Segoe UI";
  color:#24292E'>&nbsp;уровень каретки по z от&nbsp;</span><strong
  style='box-sizing: border-box'><span style='font-size:14.0pt;font-family:
  "Calibri Light","sans-serif";mso-bidi-font-family:"Segoe UI";color:red'>0</span></strong><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:#24292E'>&nbsp;до&nbsp;</span><strong style='box-sizing: border-box'><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:red'>8</span></strong><span style='font-size:14.0pt;
  font-family:"Calibri Light","sans-serif";mso-bidi-font-family:"Segoe UI";
  color:#24292E'><br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'><span style='mso-spacerun:yes'>     </span></span></strong></span><strong><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:red'>X</span></strong><span style='font-size:14.0pt;
  font-family:"Calibri Light","sans-serif";mso-bidi-font-family:"Segoe UI";
  color:#24292E'>&nbsp;положение каретки по x от&nbsp;</span><strong
  style='box-sizing: border-box'><span style='font-size:14.0pt;font-family:
  "Calibri Light","sans-serif";mso-bidi-font-family:"Segoe UI";color:red'>0</span></strong><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:#24292E'>&nbsp;до&nbsp;</span><strong style='box-sizing: border-box'><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:red'>4</span></strong><span style='font-size:14.0pt;
  font-family:"Calibri Light","sans-serif";mso-bidi-font-family:"Segoe UI";
  color:#24292E'><br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'><span style='mso-spacerun:yes'>     </span></span></strong></span><strong><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:red'>Y</span></strong><span style='font-size:14.0pt;
  font-family:"Calibri Light","sans-serif";mso-bidi-font-family:"Segoe UI";
  color:#24292E'>&nbsp;положение каретки по y от&nbsp;</span><strong
  style='box-sizing: border-box'><span style='font-size:14.0pt;font-family:
  "Calibri Light","sans-serif";mso-bidi-font-family:"Segoe UI";color:red'>0</span></strong><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:#24292E'>&nbsp;до&nbsp;</span><strong style='box-sizing: border-box'><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:red'>3</span></strong><strong><span style='font-size:14.0pt;
  font-family:"Calibri Light","sans-serif";mso-bidi-font-family:"Segoe UI";
  color:#24292E'><o:p></o:p></span></strong></p>
  <p style='margin-top:0cm;margin-right:0cm;margin-bottom:6.6pt;margin-left:
  0cm;text-align:justify;background:white'><span style='font-size:14.0pt;
  font-family:"Calibri Light","sans-serif";mso-bidi-font-family:"Segoe UI";
  color:#24292E'><br>
  <span style='mso-spacerun:yes'>      </span>Здесь&nbsp;<strong
  style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>Y</span></strong>&nbsp;выполняет следующую
  роль когда&nbsp;<strong style='box-sizing: border-box'><span
  style='font-family:"Calibri Light","sans-serif";mso-bidi-font-family:"Segoe UI"'>1</span></strong>&nbsp;то
  после выхода каретки на заданную ячейку команды погрузки и выгрузки будут
  выполняться с задней ячейкой, когда <strong><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>3</span></strong>&nbsp;то с передней, если&nbsp;<strong
  style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>2</span></strong>&nbsp;это просто
  перемещение.<br style='box-sizing: border-box'>
  Перед у дронпоинта там где отсек выдачи.<o:p></o:p></span></p>
  <p style='margin-top:0cm;margin-right:0cm;margin-bottom:6.6pt;margin-left:
  0cm;background:white'><span style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI";color:#24292E'><br>
  <span style='mso-spacerun:yes'>      </span>Команда перемещения каретки может
  иметь следующий вид<br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'><span style='mso-spacerun:yes'>      
  </span></span></strong></span><strong><span style='font-size:14.0pt;
  font-family:"Calibri Light","sans-serif";mso-bidi-font-family:"Segoe UI";
  color:red'>{&quot;command&quot;: &quot;goto_cell&quot;, &quot;params&quot;:
  {&quot;Xkr&quot;: 1, &quot;y&quot;: 2, &quot;z&quot;: 7}}<o:p></o:p></span></strong></p>
  <p style='margin-top:0cm;margin-right:0cm;margin-bottom:6.6pt;margin-left:
  0cm;text-align:justify;background:white'><span style='font-size:14.0pt;
  font-family:"Calibri Light","sans-serif";mso-bidi-font-family:"Segoe UI";
  color:#24292E'><br>
  <span style='mso-spacerun:yes'>       </span>Когда в команде присутствует
  параметр&nbsp;<strong style='box-sizing: border-box'><span style='font-family:
  "Calibri Light","sans-serif";mso-bidi-font-family:"Segoe UI"'>Xkr</span></strong>&nbsp;это
  воспринимается как<br style='box-sizing: border-box'>
  движение каретки к позиции установки или снятие крышки зарядки.<br
  style='box-sizing: border-box'>
  У&nbsp;<strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>дронпоинт2</span></strong>&nbsp;имеется&nbsp;<strong
  style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>8</span></strong>&nbsp;ячеек для установки
  крышки зарядки, следовательно параметр может принимать от&nbsp;<strong
  style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>0</span></strong>&nbsp;до&nbsp;<strong
  style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>7</span></strong>. Остальные параметры не
  несут смысла. Заставить каретку выйти на позиции операций с крышками зарядки
  можно также используя<span
  style='mso-spacerun:yes'>                           </span><span
  style='mso-spacerun:yes'> </span>такие команды:&nbsp;<strong
  style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;posKR0&quot;} {&quot;command&quot;:&quot;posKR1&quot;}</span></strong><br
  style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;posKR3&quot;}</span></strong>&nbsp;и.т.д.<br
  style='mso-special-character:line-break;box-sizing: border-box'>
  <![if !supportLineBreakNewLine]><br style='mso-special-character:line-break'>
  <![endif]><o:p></o:p></span></p>
  <p style='margin-top:0cm;margin-right:0cm;margin-bottom:6.6pt;margin-left:
  0cm;background:white'><span style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI";color:#24292E'><span
  style='mso-spacerun:yes'>       </span>Также имеются следующие команды
  перемещения<br style='box-sizing: border-box'>
  </span><strong style='box-sizing: border-box'><span style='font-size:14.0pt;
  font-family:"Calibri Light","sans-serif";mso-bidi-font-family:"Segoe UI";
  color:red'>{&quot;command&quot;:&quot;posOV&quot;}</span></strong><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:#24292E'>&nbsp;- позиция отсека выдачи, равносильна команде<br
  style='box-sizing: border-box'>
  {&quot;command&quot;: &quot;goto_cell&quot;, &quot;params&quot;:
  {&quot;x&quot;: 2, &quot;y&quot;: 3, &quot;z&quot;: 1}}<br style='box-sizing: border-box'>
  </span><strong style='box-sizing: border-box'><span style='font-size:14.0pt;
  font-family:"Calibri Light","sans-serif";mso-bidi-font-family:"Segoe UI";
  color:red'>{&quot;command&quot;:&quot;posDN&quot;}</span></strong><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:#24292E'>&nbsp;- позиция операций с дроном(подается перед
  операциями с дроном, вставить или снять контейнер).<br style='box-sizing: border-box'>
  <br style='mso-special-character:line-break;box-sizing: border-box'>
  <![if !supportLineBreakNewLine]><br style='mso-special-character:line-break'>
  <![endif]><o:p></o:p></span></p>
  <h3 align=center style='margin-top:9.95pt;margin-right:0cm;margin-bottom:
  6.6pt;margin-left:0cm;text-align:center;background:white;box-sizing: border-box;
  font-variant-ligatures: normal;font-variant-caps: normal;orphans: 2;
  text-align:start;widows: 2;-webkit-text-stroke-width: 0px;text-decoration-thickness: initial;
  text-decoration-style: initial;text-decoration-color: initial;word-spacing:
  0px'><span style='font-size:16.0pt;line-height:115%;font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI";color:#24292E'>Команды специальных операций.<o:p></o:p></span></h3>
  <p style='margin-top:0cm;margin-right:0cm;margin-bottom:6.6pt;margin-left:
  0cm;background:white;box-sizing: border-box;font-variant-ligatures: normal;
  font-variant-caps: normal;orphans: 2;text-align:start;widows: 2;-webkit-text-stroke-width: 0px;
  text-decoration-thickness: initial;text-decoration-style: initial;text-decoration-color: initial;
  word-spacing:0px'><strong style='box-sizing: border-box'><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:#24292E'>{&quot;command&quot;:&quot;loadingCELL&quot;}</span></strong><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:#24292E'>&nbsp;- загрузка в ячейку переднею или заднею будет
  зависеть<br style='box-sizing: border-box'>
  от того, что было указанно в параметре&nbsp;<strong style='box-sizing: border-box'><span
  style='font-family:"Calibri Light","sans-serif";mso-bidi-font-family:"Segoe UI"'>Y</span></strong>&nbsp;команды&nbsp;<strong
  style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>goto_cell</span></strong>&nbsp;при
  перемещении к этой ячейки. Напомню если&nbsp;<strong style='box-sizing: border-box'><span
  style='font-family:"Calibri Light","sans-serif";mso-bidi-font-family:"Segoe UI"'>&quot;y&quot;:
  3</span></strong>&nbsp;это перед, если&nbsp;<strong style='box-sizing: border-box'><span
  style='font-family:"Calibri Light","sans-serif";mso-bidi-font-family:"Segoe UI"'>&quot;y&quot;:
  1</span></strong>&nbsp;это зад, если&nbsp;<strong style='box-sizing: border-box'><span
  style='font-family:"Calibri Light","sans-serif";mso-bidi-font-family:"Segoe UI"'>&quot;y&quot;:
  2</span></strong>&nbsp;это просто перемещение.<br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;unloadingCELL&quot;}</span></strong>&nbsp;-
  выгрузка из ячейки передней или задней также<br style='box-sizing: border-box'>
  зависит от параметра&nbsp;<strong style='box-sizing: border-box'><span
  style='font-family:"Calibri Light","sans-serif";mso-bidi-font-family:"Segoe UI"'>Y</span></strong>&nbsp;команды&nbsp;<strong
  style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>goto_cell.</span></strong><br
  style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;lock_top_hatch_lock&quot;}</span></strong>&nbsp;-
  установка верхнего люка.<br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;release_top_hatch_lock&quot;}</span></strong>&nbsp;-
  снятие верхнего люка .<br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;charging_cover_removing&quot;}</span></strong>&nbsp;–
  снятие крышки с зарядки.<br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;charging_cover_install&quot;}</span></strong>&nbsp;–
  установка крышки на зарядку.<br style='box-sizing: border-box'>
  Номер крышки задается позицией на которой стоит каретка. То есть перед операциями
  с<br style='box-sizing: border-box'>
  крышками надо выполнить команду перемещения к нужной ячейки крышки. За это
  отвечает параметр&nbsp;<strong style='box-sizing: border-box'><span
  style='font-family:"Calibri Light","sans-serif";mso-bidi-font-family:"Segoe UI"'>Xkr</span></strong>&nbsp;команды&nbsp;<strong
  style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>goto_cell</span></strong>&nbsp;или команды&nbsp;<strong
  style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;posKR0&quot;}
  {&quot;command&quot;:&quot;posKR1&quot;}</span></strong><br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;hatch_delivery_open&quot;}</span></strong>&nbsp;-
  открыть люк отсека выдачи.<br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;hatch_delivery_close&quot;}</span></strong>&nbsp;-
  закрыть люк отсека выдачи.<br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;container_insert&quot;}</span></strong>&nbsp;–
  установка контейнера в коптер.<br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;container_removing&quot;}</span></strong>&nbsp;–
  снятие контейнера с коптера.<br style='box-sizing: border-box'>
  Эти операции выполняются при открытом верхнем люке и нахождении каретки на<br
  style='box-sizing: border-box'>
  определенной позиции. Для&nbsp;<strong style='box-sizing: border-box'><span
  style='font-family:"Calibri Light","sans-serif";mso-bidi-font-family:"Segoe UI"'>дронпоинта2</span></strong>&nbsp;позиция
  операций с коптером следующая<br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;: &quot;goto_cell&quot;,
  &quot;params&quot;: {&quot;x&quot;: 2, &quot;y&quot;: 2, &quot;z&quot;: 5}}</span></strong><br
  style='box-sizing: border-box'>
  Но так как у разных дронпоинтов эта позиция может отличатся есть специальная
  команда<br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;posDN&quot;}</span></strong><br
  style='box-sizing: border-box'>
  <br style='mso-special-character:line-break;box-sizing: border-box'>
  <![if !supportLineBreakNewLine]><br style='mso-special-character:line-break'>
  <![endif]><o:p></o:p></span></p>
  <h3 align=center style='margin-top:9.95pt;margin-right:0cm;margin-bottom:
  6.6pt;margin-left:0cm;text-align:center;background:white;box-sizing: border-box;
  font-variant-ligatures: normal;font-variant-caps: normal;orphans: 2;
  text-align:start;widows: 2;-webkit-text-stroke-width: 0px;text-decoration-thickness: initial;
  text-decoration-style: initial;text-decoration-color: initial;word-spacing:
  0px'><span style='font-size:16.0pt;line-height:115%;font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI";color:#24292E'>Команды тестирования.<o:p></o:p></span></h3>
  <p style='margin-top:0cm;margin-right:0cm;margin-bottom:6.6pt;margin-left:
  0cm;background:white;box-sizing: border-box;font-variant-ligatures: normal;
  font-variant-caps: normal;orphans: 2;text-align:start;widows: 2;-webkit-text-stroke-width: 0px;
  text-decoration-thickness: initial;text-decoration-style: initial;text-decoration-color: initial;
  word-spacing:0px'><strong style='box-sizing: border-box'><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:#24292E'>{&quot;command&quot;:&quot;Ztest&quot;}</span></strong><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:#24292E'>&nbsp;- тест оси Z.<br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;Ytest&quot;}</span></strong>&nbsp;-
  тест оси Y.<br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;Xtest&quot;}</span></strong>&nbsp;-
  тест оси X.<br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;ABlock&quot;}</span></strong>&nbsp;–
  выдвинуть крышки платформы А<br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;BBlock&quot;}</span></strong>&nbsp;–
  выдвинуть крышки платформы B<br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;VLtest&quot;}</span></strong>&nbsp;-
  тест верхнего люка<br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;lockKR2O&quot;}</span></strong>&nbsp;-
  открыть замок крышки KR2<br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;lockKR2C&quot;}</span></strong>&nbsp;-
  закрыть замок крышки KR2<br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;lockKR3O&quot;}</span></strong>&nbsp;-
  открыть замок крышки KR3<br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;lockKR3C&quot;}</span></strong>&nbsp;-
  закрыть замок крышки KR3 и.т.д.<br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;LockConO&quot;}</span></strong>&nbsp;-
  открыть замок контейнера коптера<br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;LockConC&quot;}</span></strong>&nbsp;-
  закрыть замок контейнера коптера<br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;testSol&quot;}</span></strong>&nbsp;-
  тест соленоида отсека выдачи<br style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;tesCont&quot;}</span></strong>&nbsp;-
  тест контейнера коптера устанавливает и снимает 10раз.<br style='box-sizing: border-box'>
  <br style='mso-special-character:line-break;box-sizing: border-box'>
  <![if !supportLineBreakNewLine]><br style='mso-special-character:line-break'>
  <![endif]><o:p></o:p></span></p>
  <h3 align=center style='margin-top:9.95pt;margin-right:0cm;margin-bottom:
  6.6pt;margin-left:0cm;text-align:center;background:white;box-sizing: border-box;
  font-variant-ligatures: normal;font-variant-caps: normal;orphans: 2;
  text-align:start;widows: 2;-webkit-text-stroke-width: 0px;text-decoration-thickness: initial;
  text-decoration-style: initial;text-decoration-color: initial;word-spacing:
  0px'><span style='font-size:16.0pt;line-height:115%;font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI";color:#24292E'>Команды посадочному столу.<o:p></o:p></span></h3>
  <p style='margin-top:0cm;background:white;box-sizing: border-box;font-variant-ligatures: normal;
  font-variant-caps: normal;orphans: 2;text-align:start;widows: 2;-webkit-text-stroke-width: 0px;
  text-decoration-thickness: initial;text-decoration-style: initial;text-decoration-color: initial;
  word-spacing:0px'><strong style='box-sizing: border-box'><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:#24292E'>{&quot;command&quot;:&quot;centr&quot;}</span></strong><span
  style='font-size:14.0pt;font-family:"Calibri Light","sans-serif";mso-bidi-font-family:
  "Segoe UI";color:#24292E'>&nbsp;– сдвигает механизм
  позиционирования(центрирует коптер).<br style='box-sizing: border-box'>
  Команда подается после посадки коптера. Выставляет коптер над верхним люком.<br
  style='box-sizing: border-box'>
  <strong style='box-sizing: border-box'><span style='font-family:"Calibri Light","sans-serif";
  mso-bidi-font-family:"Segoe UI"'>{&quot;command&quot;:&quot;uncentr&quot;}</span></strong>&nbsp;–
  разводит механизм позиционирования. После того как<br style='box-sizing: border-box'>
  контейнер с грузом и крышкой установлен в коптер, и верхний люк закрыт. Далее
  можно<br style='box-sizing: border-box'>
  взлетать.<o:p></o:p></span></p>
  <p class=MsoNormal><o:p>&nbsp;</o:p></p>
  </td>
 </tr>
</table>


