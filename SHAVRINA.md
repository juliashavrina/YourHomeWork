# Инструкция по работе с git
**Базовые команды с первого семинара.**

* git init - команда, инициализирущая репозиторий
* git status - команда, показывает состояния файлов в репозитории
* git add - команда, добавляет изменения в файл для их последующего отслеживания
* git commit - команда, фиксирует изменения , внесенные в файл командой git add
* git log - команда, выводящая журнал всех commit
* git checkout - команда, позволяяет передвигаться по всем изменениям файла 
* git checkout  master- команда, позволяет перейти к актуальному состоянию файла
* git diff - команда вычисляет разницу между файлами

**Базовые команда со второго семинара.**

* git branch branch_name - команда создает новую ветку с именем branch_name;
* git branch - команда показывает все ветки файла;
* git branch check out branch_name - команда для перехода на ветку с именем branch_name;
* git branch _d branch_name - команда для удаления ветки с именем branch_name;
* git merge branch_name - команда для слияние ветки с именем branch_name с основной веткой.
* git log --graph - команда, выводящая журнал всех коммитов всех веток.

*Пошаговая инструкция по слиянию веток.*

1. Перейти на основную ветку с помощью команды git checkout.
2. Для слияния ветки с именем branch_name с основной веткой ввести команду git merge branch_name.
3. При возникновении конфликта*, разрешить его и закомиттеть результат.

**Возникновение конфликта и способы их разрешения:*
1. Auto - merging - конфликта нет, происходит автоматическое слияние и автоматически создается commit/
2. Fast-forward - конфликта нет , когда текущей ветка не имеет дополнительных коммитов по сравнению с веткой, которую мы хотим слить, commit тоже создается автоматически.
3. Конфликт есть и git предлагает выбрать варианты разрешения конфликта:
* accept current change - принять изменения текущей ветки;
* accept incoming change - принять изменения, ветки которую мы хотим слить;
* accept both changes - принять изменения обеих веток.
После выбора варианта разрешения конфликта, нужно создать commit.

**Базовые команды с третьего семинара.**
* git clone *ссылка на удаленнный репозиторий* - команда копирует в локальную папку на своем компьютере, удаленный репозиторий;
* cd - команда, для смены текущего каталога;
* git remote add origin *ссылка на удаленный репозиторий* - команда создает удаленный репозиторий, адрес его указан в ссылке;
* git push -u origin main - команда направляет локальный репозиторий  на удаленный в интернете;
* git push - команда вносит изменения из локального репозитория в удаленный;
* git pull- команда сливает изменения из удаленного репозитория в локальной и автоматически делает merge 

**Как скопировать удаленный репозиторий в локальную папку.**

1. Авторизация на GitHub.

2. На своем компьютере создаем новую папку.

3. На GitHub нажимаем кнопку Code, появившуюся в окне ссылку копируем.

4. Открываем терминал , набираем команду git clone и вставляем ссылку.

**Как скопировать локальный репозиторий в удаленный.**

1. Создать новый репозиторий на компьютере.

2. Создать новый репозиторий на GitHub, нажав кнопку New.

3. Дать репозиторию имя.

4. Чтобы прикрепить, уже существующий репозиторий  к удаленному нажать команду git remote add origin ссылка на удаленный репозиторий.
5. Направить локальный репозиторий в удаленный репозиторий -  git push -u origin main.

**Участие в проекте другого человека.**

1. Находим интересующий нас проект и его репозиторий.

2. Делаем копию ссылки на репозиторий проекта в свой аккаунт на GitHub, с помощью команды Fork.

3. И далее идем по схеме с командой clone.