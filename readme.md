# SysOpenMath
SysOpenMath (Система открытой математики, СОМ) - программный продукт, предназначенный для создания и настройки свободной среды обработки математических данных

Проект состоит из трех файлов:
* installer.sh - скрипт для установки Julia
* package_installer.jl - скрипт для установки пакетов
* JuliaRussianGuide.pdf - русскоязычная справка
## Возможности
* установка и обновление Julia
* установка среды разработки
* установка и обновление пакетов из выбранных наборов
* создание своих наборов пакетов

### скрипт installer.sh
Скрипт обладает следующими  ключами
* `--l` - выводит список доступных версий для установки
* `--ver` - выбор версии языка Julia
* `--lts` - выбор текущей lts версии языка
* `-h или --help` - вывод справки по скрипту

### скрипт package_installer.sh
устанавливает пакеты из выбранных наборов

Для создания своих наборов необходимо отредактировать скрипт

Для этого необходимо открыть скрипт в любом удобном текстовом редакторе, найти глобальную переменную `DEFAULT_PACKAGES` и вписать в словарь новый элемент вида `'название_набора' => массив пакетов`
Пакеты могут быть найдены на [juliahub](https://juliahub.com/ui/Home)



## Как пользоваться
Чтобы воспользоваться программным продуктом необходимо

скачать файлы installer.sh и package_installer.jl

выдать права на исполнение для файла installer.sh используя команду `chmod u+x installer.sh`

запустить installer.sh командой `./installer.sh`

следовать инструкции.



