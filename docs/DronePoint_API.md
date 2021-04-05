## Аппаратный API дронпоинт2

Плата управления аппаратурой **дронпоинт2** построена на микроконтроллере<br>
**stm32F103ZET6**. Обмен данными с верхними программными уровнями осуществляется по
USB, а конкретней через реализацию **Maple Serial(COM порт).** Для приема команд и отсылки
данных по **uart(COM порт)** используется протокол **JSON**.<br>
Имеются следующие группы команд:<br>

1. **Команды перемещения каретки**, навигация по ячейкам.<br>

2. **Команды специальных операций**. Это допустим загрузка или выгрузка контейнера в<br>
    ячейку, установка контейнера в коптер и.т.д.<br>

3. **Команды тестирования** отдельных элементов и сценариев. Можно использовать<br>
    для управления какими-то отдельными исполнительными механизмами. Допустим<br>
    пощелкать соленоидом отсека выдачи, открыть или закрыть замок контейнера на<br>
    коптере, открыть или закрыть замок крышки зарядки, то-есть это те простые<br>
    операции которые входят в состав более сложных команд специальных операций.<br>
    Также сюда входят сценарии тест оси Z, тест оси X, комплексное перемещение по<br>
    различным ячейкам с погрузкой и выгрузкой контейнера и.т.д.<br>

4. **Команды посадочному столу**. Исполнительным механизмом посадочного стола<br>
    является механизм позиционирования. Он выполняет функцию центрирования<br>
    коптера после посадки т.е. выставляет его точно над верхним люком, точное<br>
    положение коптера очень важно для операций установки и снятия контейнера.<br>
    <br>
    <br>


<table class=MsoNormalTable border=0 cellspacing=0 cellpadding=0
 style='margin-left:12.2pt;border-collapse:collapse;mso-padding-alt:0cm 5.4pt 0cm 5.4pt'>
 <tr style='mso-yfti-irow:0;mso-yfti-firstrow:yes;mso-yfti-lastrow:yes;
  height:290.1pt'>
  <td width=568 valign=top style='width:340.5pt;padding:0cm 5.4pt 0cm 5.4pt;
  height:290.1pt'>
  <p class=MsoNormal style='mso-margin-top-alt:auto;mso-margin-bottom-alt:auto;
  text-align:justify;line-height:normal;background:white'><span
  style='font-size:9.5pt;mso-fareast-font-family:"Times New Roman";mso-bidi-font-family:
  "Times New Roman";mso-fareast-language:RU'><span
  style='mso-spacerun:yes'>        </span></span><span style='font-size:9.5pt;
  font-family:"Helvetica","sans-serif";mso-fareast-font-family:"Times New Roman";
  mso-bidi-font-family:"Times New Roman";mso-fareast-language:RU'>Плата
  управления аппаратурой&nbsp;</span><span style='font-size:9.5pt;mso-fareast-font-family:
  "Times New Roman";mso-bidi-font-family:"Times New Roman";mso-fareast-language:
  RU'> </span><b><span style='font-size:9.5pt;mso-bidi-font-size:11.0pt;
  font-family:"Helvetica","sans-serif";mso-fareast-font-family:"Times New Roman";
  mso-bidi-font-family:"Times New Roman";mso-fareast-language:RU'>дронпоинт2</span></b><span
  style='font-size:9.5pt;font-family:"Helvetica","sans-serif";mso-fareast-font-family:
  "Times New Roman";mso-bidi-font-family:"Times New Roman";mso-fareast-language:
  RU'>&nbsp;</span><span style='font-size:9.5pt;mso-fareast-font-family:"Times New Roman";
  mso-bidi-font-family:"Times New Roman";mso-fareast-language:RU'> </span><span
  style='font-size:9.5pt;font-family:"Helvetica","sans-serif";mso-fareast-font-family:
  "Times New Roman";mso-bidi-font-family:"Times New Roman";mso-fareast-language:
  RU'>построена на микроконтроллере</span><span style='font-size:9.5pt;
  mso-fareast-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
  mso-fareast-language:RU'> </span><b><span style='font-size:9.5pt;mso-bidi-font-size:
  11.0pt;font-family:"Helvetica","sans-serif";mso-fareast-font-family:"Times New Roman";
  mso-bidi-font-family:"Times New Roman";mso-fareast-language:RU'>stm32F103ZET6</span></b><span
  style='font-size:9.5pt;font-family:"Helvetica","sans-serif";mso-fareast-font-family:
  "Times New Roman";mso-bidi-font-family:"Times New Roman";mso-fareast-language:
  RU'>. Обмен данными с верхними программными </span><span style='font-size:
  9.5pt;mso-fareast-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
  mso-fareast-language:RU'><span style='mso-spacerun:yes'>  </span></span><span
  style='font-size:9.5pt;font-family:"Helvetica","sans-serif";mso-fareast-font-family:
  "Times New Roman";mso-bidi-font-family:"Times New Roman";mso-fareast-language:
  RU'>уровнями осуществ</span><span style='font-size:9.5pt;mso-fareast-font-family:
  "Times New Roman";mso-bidi-font-family:"Times New Roman";mso-fareast-language:
  RU'> <span style='mso-spacerun:yes'>  </span></span><span style='font-size:
  9.5pt;font-family:"Helvetica","sans-serif";mso-fareast-font-family:"Times New Roman";
  mso-bidi-font-family:"Times New Roman";mso-fareast-language:RU'>ляется по
  USB, а конкретней </span><span style='font-size:9.5pt;mso-fareast-font-family:
  "Times New Roman";mso-bidi-font-family:"Times New Roman";mso-fareast-language:
  RU'><span style='mso-spacerun:yes'>    </span></span><span style='font-size:
  9.5pt;font-family:"Helvetica","sans-serif";mso-fareast-font-family:"Times New Roman";
  mso-bidi-font-family:"Times New Roman";mso-fareast-language:RU'>через
  реализацию&nbsp;</span><span style='font-size:9.5pt;mso-fareast-font-family:
  "Times New Roman";mso-bidi-font-family:"Times New Roman";mso-fareast-language:
  RU'><span style='mso-spacerun:yes'>  </span></span><b><span style='font-size:
  9.5pt;mso-bidi-font-size:11.0pt;font-family:"Helvetica","sans-serif";
  mso-fareast-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
  mso-fareast-language:RU'>Maple Serial(COM порт).</span></b><span
  style='font-size:9.5pt;font-family:"Helvetica","sans-serif";mso-fareast-font-family:
  "Times New Roman";mso-bidi-font-family:"Times New Roman";mso-fareast-language:
  RU'>&nbsp;Для приема команд </span><span style='font-size:9.5pt;mso-fareast-font-family:
  "Times New Roman";mso-bidi-font-family:"Times New Roman";mso-fareast-language:
  RU'><span style='mso-spacerun:yes'>               </span></span><span
  style='font-size:9.5pt;font-family:"Helvetica","sans-serif";mso-fareast-font-family:
  "Times New Roman";mso-bidi-font-family:"Times New Roman";mso-fareast-language:
  RU'>и </span><span style='font-size:9.5pt;mso-fareast-font-family:"Times New Roman";
  mso-bidi-font-family:"Times New Roman";mso-fareast-language:RU'><span
  style='mso-spacerun:yes'> </span></span><span style='font-size:9.5pt;
  font-family:"Helvetica","sans-serif";mso-fareast-font-family:"Times New Roman";
  mso-bidi-font-family:"Times New Roman";mso-fareast-language:RU'>отсылки
  данных</span><span style='font-size:9.5pt;mso-fareast-font-family:"Times New Roman";
  mso-bidi-font-family:"Times New Roman";mso-fareast-language:RU'> </span><span
  style='font-size:9.5pt;font-family:"Helvetica","sans-serif";mso-fareast-font-family:
  "Times New Roman";mso-bidi-font-family:"Times New Roman";mso-fareast-language:
  RU'>по&nbsp;</span><b><span style='font-size:9.5pt;mso-bidi-font-size:11.0pt;
  font-family:"Helvetica","sans-serif";mso-fareast-font-family:"Times New Roman";
  mso-bidi-font-family:"Times New Roman";mso-fareast-language:RU'>uart(COMпорт)</span></b><span
  style='font-size:9.5pt;font-family:"Helvetica","sans-serif";mso-fareast-font-family:
  "Times New Roman";mso-bidi-font-family:"Times New Roman";mso-fareast-language:
  RU'>&nbsp;используется</span><span style='font-size:9.5pt;mso-fareast-font-family:
  "Times New Roman";mso-bidi-font-family:"Times New Roman";mso-fareast-language:
  RU'> </span><span style='font-size:9.5pt;font-family:"Helvetica","sans-serif";
  mso-fareast-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
  mso-fareast-language:RU'>протокол&nbsp;</span><b><span style='font-size:9.5pt;
  mso-bidi-font-size:11.0pt;font-family:"Helvetica","sans-serif";mso-fareast-font-family:
  "Times New Roman";mso-bidi-font-family:"Times New Roman";mso-fareast-language:
  RU'>JSON</span></b><span style='font-size:9.5pt;font-family:"Helvetica","sans-serif";
  mso-fareast-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
  mso-fareast-language:RU'>.<br>
  </span><span style='font-size:9.5pt;mso-fareast-font-family:"Times New Roman";
  mso-bidi-font-family:"Times New Roman";mso-fareast-language:RU'><span
  style='mso-spacerun:yes'>      </span><span style='mso-spacerun:yes'> </span></span><span
  style='font-size:9.5pt;font-family:"Helvetica","sans-serif";mso-fareast-font-family:
  "Times New Roman";mso-bidi-font-family:"Times New Roman";mso-fareast-language:
  RU'>Имеются следующие группы команд:</span><span style='font-size:9.5pt;
  mso-fareast-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
  mso-fareast-language:RU'><o:p></o:p></span></p>
  <p class=MsoNormal style='margin-top:6.0pt;margin-right:0cm;margin-bottom:
  6.0pt;margin-left:22.5pt;text-indent:-18.0pt;line-height:normal;mso-list:
  l0 level1 lfo1;tab-stops:list 36.0pt;background:white'><![if !supportLists]><span
  style='font-size:9.5pt;font-family:"Helvetica","sans-serif";mso-fareast-font-family:
  Helvetica;mso-bidi-font-family:Helvetica;mso-fareast-language:RU'><span
  style='mso-list:Ignore'>1.<span style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  </span></span></span><![endif]><b><span style='font-size:9.5pt;mso-bidi-font-size:
  11.0pt;font-family:"Helvetica","sans-serif";mso-fareast-font-family:"Times New Roman";
  mso-bidi-font-family:"Times New Roman";mso-fareast-language:RU'>Команды
  перемещения каретки</span></b><span style='font-size:9.5pt;font-family:"Helvetica","sans-serif";
  mso-fareast-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
  mso-fareast-language:RU'>, навигация по ячейкам.<o:p></o:p></span></p>
  <p class=MsoNormal style='margin-top:6.0pt;margin-right:0cm;margin-bottom:
  6.0pt;margin-left:22.5pt;text-align:justify;text-indent:-18.0pt;line-height:
  normal;mso-list:l0 level1 lfo1;tab-stops:list 36.0pt;background:white'><![if !supportLists]><span
  style='font-size:9.5pt;font-family:"Helvetica","sans-serif";mso-fareast-font-family:
  Helvetica;mso-bidi-font-family:Helvetica;mso-fareast-language:RU'><span
  style='mso-list:Ignore'>2.<span style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  </span></span></span><![endif]><b><span style='font-size:9.5pt;mso-bidi-font-size:
  11.0pt;font-family:"Helvetica","sans-serif";mso-fareast-font-family:"Times New Roman";
  mso-bidi-font-family:"Times New Roman";mso-fareast-language:RU'>Команды
  специальных операций</span></b><span style='font-size:9.5pt;font-family:"Helvetica","sans-serif";
  mso-fareast-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
  mso-fareast-language:RU'>. Это допустим загрузка или выгрузка контейнера вячейку,
  установка контейнера в коптер и.т.д.<o:p></o:p></span></p>
  <p class=MsoNormal style='margin-top:6.0pt;margin-right:0cm;margin-bottom:
  6.0pt;margin-left:22.5pt;text-align:justify;text-indent:-18.0pt;line-height:
  normal;mso-list:l0 level1 lfo1;tab-stops:list 36.0pt;background:white'><![if !supportLists]><span
  style='font-size:9.5pt;font-family:"Helvetica","sans-serif";mso-fareast-font-family:
  Helvetica;mso-bidi-font-family:Helvetica;mso-fareast-language:RU'><span
  style='mso-list:Ignore'>3.<span style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  </span></span></span><![endif]><b><span style='font-size:9.5pt;mso-bidi-font-size:
  11.0pt;font-family:"Helvetica","sans-serif";mso-fareast-font-family:"Times New Roman";
  mso-bidi-font-family:"Times New Roman";mso-fareast-language:RU'>Команды
  тестирования</span></b><span style='font-size:9.5pt;font-family:"Helvetica","sans-serif";
  mso-fareast-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
  mso-fareast-language:RU'>&nbsp;отдельных элементов и сценариев. Можно
  использовать</span><span style='font-size:9.5pt;mso-fareast-font-family:"Times New Roman";
  mso-bidi-font-family:"Times New Roman";mso-fareast-language:RU'><span
  style='mso-spacerun:yes'>  </span></span><span style='font-size:9.5pt;
  font-family:"Helvetica","sans-serif";mso-fareast-font-family:"Times New Roman";
  mso-bidi-font-family:"Times New Roman";mso-fareast-language:RU'>для
  управления какими-то отдельными</span><span style='font-size:9.5pt;
  mso-fareast-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
  mso-fareast-language:RU'> </span><span style='font-size:9.5pt;font-family:
  "Helvetica","sans-serif";mso-fareast-font-family:"Times New Roman";
  mso-bidi-font-family:"Times New Roman";mso-fareast-language:RU'>исполнительными
  механизмами. Допустим</span><span style='font-size:9.5pt;mso-fareast-font-family:
  "Times New Roman";mso-bidi-font-family:"Times New Roman";mso-fareast-language:
  RU'> </span><span style='font-size:9.5pt;font-family:"Helvetica","sans-serif";
  mso-fareast-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
  mso-fareast-language:RU'>пощелкать соленоидом отсека выдачи, открыть или
  закрыть замок контейнера на</span><span style='font-size:9.5pt;mso-fareast-font-family:
  "Times New Roman";mso-bidi-font-family:"Times New Roman";mso-fareast-language:
  RU'> </span><span style='font-size:9.5pt;font-family:"Helvetica","sans-serif";
  mso-fareast-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
  mso-fareast-language:RU'>коптере, открыть или закрыть замок крышки зарядки,
  то-есть это те простые<br>
  операции которые входят в состав более сложных команд специальных операций.</span><span
  style='font-size:9.5pt;mso-fareast-font-family:"Times New Roman";mso-bidi-font-family:
  "Times New Roman";mso-fareast-language:RU'><span style='mso-spacerun:yes'> 
  </span></span><span style='font-size:9.5pt;font-family:"Helvetica","sans-serif";
  mso-fareast-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
  mso-fareast-language:RU'>Также сюда входят сценарии тест оси Z, тест оси X,
  комплексное перемещение по</span><span style='font-size:9.5pt;mso-fareast-font-family:
  "Times New Roman";mso-bidi-font-family:"Times New Roman";mso-fareast-language:
  RU'><span style='mso-spacerun:yes'>  </span></span><span style='font-size:
  9.5pt;font-family:"Helvetica","sans-serif";mso-fareast-font-family:"Times New Roman";
  mso-bidi-font-family:"Times New Roman";mso-fareast-language:RU'>различным
  ячейкам с погрузкой и выгрузкой контейнера и.т.д.<o:p></o:p></span></p>
  <p class=MsoNormal style='margin-top:6.0pt;margin-right:0cm;margin-bottom:
  6.0pt;margin-left:22.5pt;text-align:justify;text-indent:-18.0pt;line-height:
  normal;mso-list:l0 level1 lfo1;tab-stops:list 36.0pt;background:white'><![if !supportLists]><span
  style='font-size:9.5pt;font-family:"Helvetica","sans-serif";mso-fareast-font-family:
  Helvetica;mso-bidi-font-family:Helvetica;mso-fareast-language:RU'><span
  style='mso-list:Ignore'>4.<span style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  </span></span></span><![endif]><b><span style='font-size:9.5pt;mso-bidi-font-size:
  11.0pt;font-family:"Helvetica","sans-serif";mso-fareast-font-family:"Times New Roman";
  mso-bidi-font-family:"Times New Roman";mso-fareast-language:RU'>Команды
  посадочному столу</span></b><span style='font-size:9.5pt;font-family:"Helvetica","sans-serif";
  mso-fareast-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
  mso-fareast-language:RU'>. Исполнительным механизмом посадочного стола</span><span
  style='font-size:9.5pt;mso-fareast-font-family:"Times New Roman";mso-bidi-font-family:
  "Times New Roman";mso-fareast-language:RU'><span style='mso-spacerun:yes'> 
  </span></span><span style='font-size:9.5pt;font-family:"Helvetica","sans-serif";
  mso-fareast-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
  mso-fareast-language:RU'>является механизм позиционирования. Он выполняет
  функцию центрирования</span><span style='font-size:9.5pt;mso-fareast-font-family:
  "Times New Roman";mso-bidi-font-family:"Times New Roman";mso-fareast-language:
  RU'><span style='mso-spacerun:yes'>  </span></span><span style='font-size:
  9.5pt;font-family:"Helvetica","sans-serif";mso-fareast-font-family:"Times New Roman";
  mso-bidi-font-family:"Times New Roman";mso-fareast-language:RU'>коптера после
  посадки т.е. выставляет его точно над верхним люком, точное</span><span
  style='font-size:9.5pt;mso-fareast-font-family:"Times New Roman";mso-bidi-font-family:
  "Times New Roman";mso-fareast-language:RU'><span style='mso-spacerun:yes'> 
  </span></span><span style='font-size:9.5pt;font-family:"Helvetica","sans-serif";
  mso-fareast-font-family:"Times New Roman";mso-bidi-font-family:"Times New Roman";
  mso-fareast-language:RU'>положение коптера очень важно для операций установки
  и снятия контейнера.<o:p></o:p></span></p>
  <p class=MsoNormal><o:p>&nbsp;</o:p></p>
  </td>
 </tr>
</table>




  
### Команды перемещения каретки

  Команда перемещения каретки может иметь следующий вид<br>
  **{"command": "goto_cell", "params": {"x": 2, "y": 2, "z": 1}}**<br>
  Команда **goto_cell** имеет следующий набор параметров:<br>
**Z** уровень каретки по z от **0** до **8**<br>
**X** положение каретки по x от **0** до **4**<br>
**Y** положение каретки по y от **0** до **3**<br>
  Здесь **Y** выполняет следующую роль когда **1** то после<br>
  выхода каретки на заданную ячейку команды погрузки<br>
  и выгрузки будут выполняться с задней ячейкой, когда<br>
  **3** то с передней, если **2** это просто перемещение.<br>
  Перед у дронпоинта там где отсек выдачи.<br>
  Команда перемещения каретки может иметь следующий вид<br>
  **{"command": "goto_cell", "params": {"Xkr": 1, "y": 2, "z": 7}}**<br>
  Когда в команде присутствует параметр **Xkr** это воспринимается как<br>
  движение каретки к позиции установки или снятие крышки зарядки.<br>
  У **дронпоинт2** имеется **8** ячеек для установки крышки зарядки, следовательно<br>
  параметр может принимать от **0** до **7**. Остальные параметры не несут смысла.<br>
  Заставить каретку выйти на позиции операций с крышками зарядки можно<br>
  также используя такие команды: **{"command":"posKR0"} {"command":"posKR1"}**<br>
  **{"command":"posKR3"}**   и.т.д.<br>
  Также имеются следующие команды перемещения<br>
  **{"command":"posOV"}** - позиция отсека выдачи, равносильна команде<br>
  {"command": "goto_cell", "params": {"x": 2, "y": 3, "z": 1}}<br>
  **{"command":"posDN"}** - позиция операций с дроном(подается перед операциями<br>
  с дроном, вставить или снять контейнер).<br>
  <br>
  <br>
 
### Команды специальных операций.

  **{"command":"loadingCELL"}** - загрузка в ячейку переднею или заднею будет зависеть<br>
  от того, что было указанно в параметре **Y** команды **goto_cell** при перемещении к этой ячейки.
  Напомню если **"y": 3** это перед, если **"y": 1** это зад, если **"y": 2** это просто перемещение.<br>
  **{"command":"unloadingCELL"}** - выгрузка из ячейки передней или задней также<br>
  зависит от параметра **Y** команды **goto_cell.**<br>
  **{"command":"lock_top_hatch_lock"}** - установка верхнего люка.<br>
  **{"command":"release_top_hatch_lock"}** - снятие верхнего люка .<br>
  **{"command":"charging_cover_removing"}** – снятие крышки с зарядки.<br>
  **{"command":"charging_cover_install"}** – установка крышки на зарядку.<br>
  Номер крышки задается позицией на которой стоит каретка. То есть перед операциями с<br>
  крышками надо выполнить команду перемещения к нужной ячейки крышки. За это отвечает
  параметр **Xkr** команды **goto_cell** или команды **{"command":"posKR0"} {"command":"posKR1"}**<br>
  **{"command":"hatch_delivery_open"}** - открыть люк отсека выдачи.<br>
  **{"command":"hatch_delivery_close"}** - закрыть люк отсека выдачи.<br>
  **{"command":"container_insert"}** – установка контейнера в коптер.<br>
  **{"command":"container_removing"}** – снятие контейнера с коптера.<br>
  Эти операции выполняются при открытом верхнем люке и нахождении каретки на<br>
  определенной позиции. Для **дронпоинта2** позиция операций с коптером следующая <br>
  **{"command": "goto_cell", "params": {"x": 2, "y": 2, "z": 5}}**<br>
  Но так как у разных дронпоинтов эта позиция может отличатся есть специальная команда<br>
  **{"command":"posDN"}**<br>
  <br>
  <br>
  
### Команды тестирования.

  **{"command":"Ztest"}** - тест оси Z.<br>
  **{"command":"Ytest"}** - тест оси Y.<br>
  **{"command":"Xtest"}** - тест оси X.<br>
  **{"command":"ABlock"}** – выдвинуть крышки платформы А<br>
  **{"command":"BBlock"}** – выдвинуть крышки платформы B<br>
  **{"command":"VLtest"}** - тест верхнего люка<br>
  **{"command":"lockKR2O"}** - открыть замок крышки KR2<br>
  **{"command":"lockKR2C"}** - закрыть замок крышки KR2<br>
  **{"command":"lockKR3O"}** - открыть замок крышки KR3<br>
  **{"command":"lockKR3C"}** - закрыть замок крышки KR3 и.т.д.<br>
  **{"command":"LockConO"}** - открыть замок контейнера коптера<br>
  **{"command":"LockConC"}** - закрыть замок контейнера коптера<br>
  **{"command":"testSol"}** - тест соленоида отсека выдачи<br>
  **{"command":"tesCont"}** - тест контейнера коптера устанавливает и снимает 10раз.<br>
<br>
<br>

### Команды посадочному столу.

  **{"command":"centr"}** – сдвигает механизм позиционирования(центрирует коптер).<br>
  Команда подается после посадки коптера. Выставляет коптер над верхним люком.<br>
  **{"command":"uncentr"}** – разводит механизм позиционирования. После того как<br>
  контейнер с грузом и крышкой установлен в коптер, и верхний люк закрыт. Далее можно<br>
  взлетать.
