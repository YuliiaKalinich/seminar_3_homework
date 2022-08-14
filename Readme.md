# Инструкция по работе с GIT

## Что такое *Git*?

*Git* - одна из реализаций распределенных систем контроля версий, позволяющаяорганизовать версионность, как локально , так и на удаленном сервере. Самая популярная платформа, реализующая *Git*, - [GitHub](http://github.com)

## Подготовка репозитория
Для создания в папке репозитория необходимо открыть эту папку в терминале и написать команду "git init", после чего в этой папке создастся скрытая папка *.git * , и таким образом папка станет репозиторием


  ## Создание "сохранений"
Для создания сохранений сначала вносим текстовые изменения. Затем сохраняем их через команду файл-сохранить или нажатием команды клавиш "CTRL+S". Затем в открытом терминале в папке-репозитория вводим команду *"git add <название нашего файла>"*. 


## Журнал изменений
Для просмотра истории изменений используется команда *git log*. Для этого в терминале с папкой-репозиторием необходимо написать комманду *git log* , и вы увидите список всех коммитов в этой ветке с описанием: имени, электронной почтысообщением к комиту и номер коммита.

## Добавление файла к коммиту
Для того, чтобы добавить файл к "сохранению" , необходимо использовать комманду *git add* . В терминале с открытой папкой-репозиторием необходимо написать *git add <название файла>* , и этот файл добавится к "сохранению" 

### Просмотр состояния репозитория
Для просмотра состояния репозитория используется команда *git status*. В терминале с открытой папкой-репозиторием необходимо написать команду *git status*.  В результате можно увидеть следующие выводы: 
1. On branch *** nothing to comit- это означает нет активных изменений
2. Untracked file- это означает, что имеются файлы не отслеживаемые системой контроля версий и тд...
### создание фиксации
Для создания фиксации используется команда *git commit* . Для этого в терминале с папкой-репозиторием необходимо написать команду *git commit-m <сообщение коммиту>*. Сообщение к коммиту писать **обязательно**.
## Создание "коммитов"
 Для этого нужно сохранить изменнения командой файл - сохранить или "CTRL+S". Далее в терминале в открытой папке-репозитории используем комманду *git add <имя файла>* и уже после сохранения и добавления сохранения, мы создаем коммит с сообщением к коммиту командой "*git commit -m <текст>*"

## Журнал изменнений

Журнал изменений - это файл, который содержит общий, хронологически упорядоченнный список изменений, внесенных в проект. он часто организован по версии с указанием даты, после чего следует список добавленных, переработанных и удаленных функций.
 В общем смысле, существует два способа делать записи в журнал изменений.
 * обычный способ: создайте текстовый файл и начните перечислять все внесенные вами изменения с указанием определенной даты.
 * выбор разработчика: автоматическое создание списка изменений из ваших сообщений к коммитам. 
 
## Перемещение между коммитами

Для перемещения между коммитами используется комманда *git checkout* . Для этого в терминале с папкой-репозиторием необходимо написать *git checkout <номер коммита>*. Номер коммита берется из журнала изменений ветки. 
## Ветки в GIT
Это простой перемещаемый указатель на один из коммитов. 
### Перемещение по веткам
Для начала нужно проверить где вы находитесь командой *"git branch"* - вводим команду в открытом терминале папки-репозиторий.
Далее нам предоставляется список всех существующих веток в этой папке, текущая папка будет помечена "*", основная папка называется "master". Если кроме master больше нет веток, то создаем при помощи комманды *"git branch <имяВетки>"*. Для перехода между ветками используем комманду *"git checkout <имяВетки>"*. Чтобы проверить свое место нахождения снова набираем комманду *" git branch"* . Чтобы удалить ненужную ветку- используем комманду *"git branch -d <имяВетки>"*
## Слияние веток и решение конфликтов
Для слияния двух веток переходим в основную ветку к которой будем добавлять изменения. И используем комманду "git merge <name>". В процессе слияния могут произойти конфликты, программа может предложить варианты решения этих конфликтов, а также их можно решить в ручную. После внесения изменений нужно сохранить файл и создать коммит с сообщением.

## Удаление веток
Чтобы удалить ветку используем комманду "git branch -d <name>" . Вводим комманду в терминале открытой папки-репозитория.

