Программа распаковки/упаковки, а также редактирования сохранений игры Overlord - Raising Hell.

Проект имеет консольную версию ограниченную в функционале и GUI находяющуся в разработке под win32.

Проверка проводиться под версию игры 0.4. 

Прим. Вероятно будет работать и под более ранние версии, позже по окончанию проект будет тест.

Консольная версия имеет функционал:
- распаковка файлов сохранений игры Overlord - Raising Hell
- упаковка файлов сохранений игры Overlord - Raising Hell

GUI версия на данный момент имеет следующий функционал:
- распаковка файлов сохранений игры Overlord - Raising Hell
- упаковка файлов сохранений игры Overlord - Raising Hell

На стадии реализации:
- точечное редактирование минионов от количества до обмундирования
- изменение количества золота
- добавление игровых элементов (оружие, броня, тотемы на хп, ману и т.д.)
- по окончанию проекта мультиязычность
- возможно будет реализована добавить/убрать ачивку или сменить локацию

Перенос на *unix системы состоится после окончания разработки


Справка по консольной версии:

progname.exe option -i input -o output 

- i name 	: name file input
- o name 	: name file output
- C 			: compressed
- D 			: uncompressed
- f 			: help

Sample: progname.exe -D -i SaveInfo.osi.tzf -o SaveInfo_uncompress.osi.tzf

Sample: progname.exe -C -i SaveInfo_uncompress.osi.tzf -o SaveInfo.osi.tzf


Справка по версии c GUI:

/*в стадии разработки*/

Сборка осуществляется с использованием rules.sh (makefile на прямую не вызывается)

Использование: rules.sh options...

Параметры:

	- g opt			Cборка gui версии (требуются дополнительные ключи)
	- c				Cборка console версии
	- h				Справка