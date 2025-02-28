Task Force Arma 3 radio
=======================

Arma 3 Team Speak Radio Plugin
_v0.8.1.5 от 17.11.2013_

###Установка

* Скачайте [архив с рацией 0.8.1](https://github.com/michail-nikolaev/task-force-arma-3-radio/raw/master/releases/0.8.1.zip) и распакуйте его.
* Cкопируйте содержимое папки `TeamSpeak 3 Client` в корневую папку TeamSpeak.
* Скопируйте содержимое папки `Arma 3` в папку с игрой `...\SteamApps\common\Arma 3`.

> TF Radio использует последнюю версию СBA (Community Base Addons). Поэтому, если этот мод у вас уже установлен, Windows предложит заменить папку.


###Настройка

* Убедитесь, что в TeamSpeak клавиша `Caps Lock` не используется для разговора.
* Также в ARMA 3 отключите разговор по внутренней связи (VON) по нажатию `Caps Lock` (чтобы не двоиться).
* Откройте список плагинов в Team Speak `Settings > Plugins`.
  1. Включите `Task Force Arma 3 Radio`.
  2. Отключите `ACRE` и `radio ts ARMA3.ru version`, если они есть, чтобы избежать конфликтов.
  3. На всякий случай внизу слева можно нажать кнопку Reload All для перезагрузки всех плагинов.
* Убедитесь, что громкость оповещений в Team Speak не отключена: `Options > Payback > Sound Pack Volume` установите в положительное значение.
* Запустите игру с аддонами `@CBA_A3` и `@task_force_radio` (Community Base Addons: A3 Beta и Task Force Arrowhead Radio). Это можно сделать, прописав в ярлыке игры имена модов после EXE файла `…\arma3.exe -mod=@CBA_A3;@task_force_radio`, но рекомендуется включить необходимые моды в настройках игры (Настройки - Дополнения, Settings -> Expansions).
* Зайдите в тот же канал, где находятся другие игроки, играющие с данной рацией, либо вас перебросит в канал `TaskForceRadio` в случае его наличия при старте миссии.

> Если ник в профиле игры и TeamSpeak совпадает - плагин изменит ваш ник в TS в процессе игры.

> Не рекомендуется использовать плагин при одновременном подключении к нескольким серверам в TeamSpeak

> Рекомендуется отключить встроенные звуки оповещений TeamSpeak: `Options > Notifications > Sound Pack: "Sounds Deactivated"`. Для применения этой опции необходимо перезапустить TeamSpeak.


###Использование

| Клавиши | Действие |
| --- | --- |
| Кнопка разговора в TeamSpeak | Прямая речь. |
| `Caps Lock` | Разговор по рации. |
| `CTRL`&nbsp;+&nbsp;`Caps Lock` | Разговор по рации дальней связи. |
| `CTRL`&nbsp;+&nbsp;`P` | Открыть интерфейс личной рации (рация должна быть в слоте инвентаря). В том случае, если у вас имеются несколько раций - вы сможете выбрать требуемую. Также есть возможность установить рацию как активную (ту, которая будет использоваться для передачи).
| `NUM[1-8]` | Быстрое переключение каналов коротковолновой рации. | 
| `ALT`&nbsp;+&nbsp;`P` | Открыть интерфейс рации дальней связи (рация дальней связи должна быть надета на спину, либо вы должны быть в технике за водителя, стрелка, командира или помощника пилота). Если доступно несколько раций - вам будет предложено выбрать. Также одну из них можно установить как активную. |
| `CTRL`&nbsp;+&nbsp;`NUM[1-9]` | Быстрое переключение каналов рации дальней связи. |
| `CTRL`&nbsp;+&nbsp;`TAB` | Изменить громкость прямой речи. Можно говорить шепотом (Whispering), нормально (Normal) и кричать (Yelling). Не влияет на громкость сигнала в радио передаче. |
| `SHIFT`&nbsp;+&nbsp;`P` | Открыть интерфейс переговорного устройства для дайверов (на вас должен быть надет ребризер).| 
| `ALT`&nbsp;+&nbsp;`Caps Lock` | Разговор по переговорному устройству для дайверов. |
| `ESC` | Выход из интерфейса рации. |

> Вы можете переназначить клавиши управления в файле настроек, лежащем в папке с игрой `...\Arma 3\userconfig\task_force_radio\radio_keys.hpp`. Файл редактируется обычным блокнотом.

###Информация

#####Рации

| Рация | Сторона | Диапазон/Дальность | Управление |
| --- | --- | --- | --- | 
| Рация [AN/PRC-152](http://ru.wikipedia.org/wiki/AN/PRC-152) (личная) | <font color="blue">BLUEFOR<font> | 30-512Mhz / 3 км | Для того чтобы ввести частоту, нажмите `CLR`, введите значение и нажмите `ENT`. Также вы можете переключать активный канал рации, нажимая на кнопки со стрелками (всего 8 каналов). Возможно изменение громкости приема кнопками `PRE+` и `PRE-`.| 
| Рация [RT-1523G (ASIP)](http://en.wikipedia.org/wiki/SINCGARS#Models) (дальняя связь) | <font color="blue">BLUEFOR<font> | 30-87Mhz / 20 км | Для того чтобы ввести частоту нажмите `MENU CLR`, введите значение и нажмите `FREQ`. Также вы можете переключать активный канал, нажимая цифровые кнопки на рации (всего 9 каналов). Возможно изменение громкости приема кнопками `TIME` и `BATT CALL`. |
| Рация [AN/PRC148-JEM](https://www.thalescomminc.com/ground/anprc148-jem.asp) (личная) | <font color="green">INDEPENDENT</font> | 30-512Mhz / 3 км | Для того чтобы ввести частоту, нажмите `ESC`, введите значение и нажмите `ENT`. Также вы можете переключать активный канал рации, нажимая на кнопки со стрелками (всего 8 каналов). Возможно изменение громкости приема кнопками `MOD` и `GR`. | 
| Рация [AN/PRC-155](http://www.gdc4s.com/anprc-155-2-channel-manpack.html) (дальняя связь)| <font color="green">INDEPENDENT</font>  | 30-87Mhz / 20 км | Для того чтобы ввести частоту нажмите `ESC`, введите значение и нажмите `MENU`. Также вы можете переключать активный канал, нажимая на стрелки (вверх в вниз). Возможно изменение громкости приема кнопкой с изображением динамика. | 
| Рация [FADAK](http://www.iran.ru/news/politics/87228/Iran_prodemonstriroval_tri_novyh_obrazca_voennogo_naznacheniya) (личная) |  <font color="red">OPFOR</font> | 30-512Mhz / 3 км | Для того чтобы ввести частоту, нажмите `CLR`, введите значение и нажмите `ENT`. Также вы можете переключать активный канал рации, нажимая `SET` и `PWR` (всего 8 каналов). Возможно изменение громкости приема кнопками `DATA` и `SEND`. | 
| Рация [MR3000](http://www.railce.com/cw/casc/rohde/m3tr.htm) (дальняя связь) | <font color="red">OPFOR</font> | 30-87Mhz / 20 км | Для того чтобы ввести частоту нажмите `CLR ESC`, введите значение и нажмите `ENT`. Также вы можете переключать активный канал, нажимая цифровые кнопки на рации, либо горизонтальными кнопками-стрелками (всего 9 каналов). Возможно изменение громкости приема вертикальными кнопками-стрелками. | 
| Переговорное устройство дайверов | Все | 32-41kHz / 70-300 м. (в зависимости от уровня волн) | Для того чтобы ввести частоту, нажмите `MODE`, введите значение и нажмите `ADV`. Возможно изменение громкости приема кнопкой с правой стороны устройства. | 


> Личная и дальняя рации одной фракции поддерживают единый протокол, поэтому могут связываться друг с другом. В случае если передача осуществляется с личной -  звук будет высокочастотным. В случае передачи с дальней - низкочастотным. 

#####Выдача раций
* По умолчанию рация дальней связи выдается лидерам отрядов. Если у игрока надет рюкзак - он его автоматически положит на землю.

* Рация ближней связи выдается игрокам, у которых есть `ItemRadio` в инвентаре. Выдача рации может потребовать нескольких секунд ожидания (следите за сообщениями в центре экрана).

#####Техника
* Рация дальней доступна в технике водителю, командиру, стрелку и помощнику пилота. Не вся техника имеет встроенные рации.

* У каждого слота техники своя рация, которая должна быть настроена отдельно. Если вы планируете пересаживаться с места на места в технике - предварительно настройте рацию на всех слотах (например на слоте водителя и на слоте стрелка).

* Техника делиться  на открытую и закрытую (изолированную). Если вы находитесь в изолированной технике, то не будете слышать голоса снаружи (и наоборот). Однако если вы выгляните из техники, то будете слышать как голоса внутри, так и снаружи.

#####Радиоперехват

* Рации можно поднимать у убитых игроков, передавать их друг другу. При этом они сохраняют все настройки (каналы, частоты, громкость). 

> Рекомендуется поднимать рации открывая инвентарь на том месте, где она лежит (чтобы она не пропала из-за ошибок игры). 

* Настройки рации в технике также сохраняются.
* По умолчанию рации каждой фракции используют свои коды шифрования, поэтому вы не будете слышать вражеские переговоровы, даже введя используемую врагами частоту. Чтобы прослушивать (и говорить в эфир) противника - необходимо каким-либо образом захватить вражескую радиостанцию.

> Для того, чтобы прослушивать рацию дальней связи (рюкзак) противника рекомендуется находиться в своей технике. В таком случае вы сможете слушать эфир противника использую рюкзак, и передавать союзникам использую рацию в технике, как активную.

#####Водолазы
* Вы не можете говорить голосом находясь под водой (даже в водолазном костюме). Однако на близком расстоянии ваш собеседник сможет расслышать что-либо очень невнятное (исключение - если вы под водой в изолированной технике).
* Находясь под водой, вы невнятно и слабо слышите голоса на суше.
* Для связи между дайверами используйте Переговорное устройство.
* Вы не можете пользоваться радио связью под водой (ни говорить, ни слышать). Если нужно что-то передать на сушу - всплывайте. Исключение - субмарина на перископной глубине (в ней водолазам можно использовать рацию дальней связи).

#####Режимы работы плагина
Плагин поддерживает два режима работы — **серьезный** и **упрощенный**. 

* **Упрощенный** — используется по умолчанию. Он предназначен главным образом для кооперативных игр. Его особенностью является то, что игроки с плагином и в игре слышат мертвых, не играющих, играющих на другом сервере и играющих без плагина игроков минуя рацию (просто как через TeamSpeak). Это делает менее удобным игры против людей, но позволяет вашему другу без проблем узнать, где вы играете, какая у вас частота и т.д. Разумется, те кто играет на одном сервере со включенными аддонами и плагинами будут слышать друг друга по "законам" рации с учетом расстояния и частот.

* **Серьезный** — предназначен для проведения игр, где игроки играют против других игроков. Для его активации в TeamSpeak необходимо создать канал с названием `TaskForceRadio` и паролем `123`. Игроки должны включить плагин рации, зайти на сервер и, разойдясь по каналам сторон, брифинговать. При старте миссии через несколько секунд игроки будут переброшены в канал `TaskForceRadio`. В данном случае игроки будут слышать только живых игроков со включенным плагином играющих на этом же сервере. Мертвые игроки, в свою очередь, могут общаться друг с другом. Если мертвый игрок респавниться - он снова будет слышать только живых. После того, как игра заканчивается, игроки перебрасываются в канал, в котором они брифинговали до игры.

#####Решение проблем
* `Pipe error 230` - вы скорее всего вы забыли включить плагин в TeamSpeak.
* Плагин в TS показываться красным и не загружается - скорее всего вам нужно обновить TeamSpeak.
* Если что-то поломалось - попробуйте перезапустить плагин.
* Не работают действия на `Caps Lock` - возможно из-за геймерской клавиатуры, где код `Caps Lock` отличается. Попробуйте изменить используемые клавиши (путем редактирования `userconfig`).
* Если из-за ошибки или еще чего-то вы перестали слышать других игроков даже вне игры, откройте `Setup 3D Sound` в TeamSpeak и кликните `Center All`.
* Для устранения возможных ошибок с плагином разработчикам может потребоваться лог TeamSpeak, чтобы его скопировать выберите `Tools` -> `Client Log`, поставьте все галочки сверху и, выделив весь текст на `CTRL + A` Скопируйте его в буфер обмена
* Если TeamSpeak (тьфу-тьфу-тьфу) упал при использовании плагина - он показывает окошко с описанием того, где можно найти дамп (путь к файлу). Буду очень благодарен за этот файлик. 

#####Картоделам
* Классы рации дальней связи: `tf_rt1523g`,`tf_mr3000`,`tf_anprc155`. Добавить ее игроку в строке инициализации в редакторе можно примерно следующим образом: `this addBackpack "tf_rt1523g";`
* Чтобы отключать автоматическую выдачу раций дальней связи игрокам добавьте в `init.sqf` следующую строку: `tf_no_auto_long_range_radio = true`
* Для того, чтобы изменить коды шифрования, используемые фракциями (для того, чтобы позволить нескольким фракциям переговариваться) добавьте в `init.sqf` примерно следующий код:
`tf_west_radio_code = "_bluefor";
tf_east_radio_code = "_opfor"; tf_guer_radio_code = "_independent"; `. Для того, чтобы две фракции могли связываться по радио у них должен быть идентичный код шифрования (вам потребуется поменять значения).

#####Администраторам TeamSpeak серверов
На всякий случай уменьшите уровень защиты от флуда: `Правый клик по серверу > Edit Virtual Server > More > Anti Flood` поставьте значения 30, 300, 3000 (сверху вниз).


#####Разработчикам
Если данная разработка будет как-либо популярна, то хотелось бы избежать кучи несовместимых форков. По этой причине в случае желания внесения изменений связывайтесь со мной - велика вероятность, что ваши разработки будут вмержены в главную ветку. Ждем ваших Pull Requests :)

#####Спасибки
* Отряду [Task Force Arrowhead](http://forum.task-force.ru/) за тестирование, поддержку, терпение и всяческую помощь.
* [MTF](http://forum.task-force.ru/index.php?action=profile;u=7) ([varzin](https://github.com/varzin)) за помощь с графикой и документацией.
* [Hardckor ](http://forum.task-force.ru/index.php?action=profile;u=14) за помощь с графикой.
* [Блендеру](http://arma3.ru/forums/index.php/user/41-blender/) за шрифт.
* [vinniefalco](https://github.com/vinniefalco) за [DSP фильтры](https://github.com/vinniefalco/DSPFilters).
* [WOG](http://wogames.info/) и лично [TRUE](http://wogames.info/profile/TRUE/) за помощь в тестировании.
* [Music DSP Collection](https://github.com/music-dsp-collection) за компрессор.
* [Avi](http://arma3.ru/forums/index.php/user/715-avi/) за кодревью.
* [andrey-zakharov](https://github.com/andrey-zakharov) ([Vaulter](http://arma3.ru/forums/index.php/user/1328-vaulter/)) за помощь в разработке.
* Дине за перевод.
* Извините, если кого-то случайно забыл.
