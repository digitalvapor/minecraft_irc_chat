Демон на python/twisted (ну не совсем демон, немонизации тут нет).
Запускает (перезапускает) minecraft сервер и копирует лог сервера на канал в irc сеть
и обратно.

Юзабельно.
Чтобы запустить подредактируйте файлы (настройки в main.py и имя канала в bot.py и irc.py).
Удобно запускается через nohup.

TODO:
Исправить качество кода.
Классы реализовать через синглтоны и вычистить все ссылки друг на друга.
После очищения покурить мануалы и грамотно реализовать работу с факторями.

Авторизацию irc юзера.
Выполнение команд из irc (особенно нужен бан и редактор вайтлиста).
Динамические запросы со стороны irc (кто играет на сервере, например).

Написать нормальный демонизатор.
Нормально класть логи.

Ну и для фана можно web-server туда всунуть :) логи чата + отдача статики от рендера карты

#######

На все было потрачено около часа, так что все ужасно. Надеюсь, найду время и сделать по уму хехе :)

#Changes or notes-to-self
* irc hardcoded `#kingdomplantar`
* assumes freenode `chat.freenode.net` and port `6666`
* assumes minecraft server file is named `minecraft_server.jar`
* if dont want to mess with eula.txt etc, run this in the same folder as `minecraft_server.jar`
  * i'm currently just doing `nohup python minecraft_irc_bot/main.py` from my `minecraft` folder
* todo: have bot speak as well in irc
