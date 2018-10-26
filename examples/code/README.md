# Вставка кода

[Код без подсветки]{https://en.wikibooks.org/wiki/LaTeX/Source_Code_Listings} - пример простейшей вставки кода без всякой подсветки.

Для подсветки кода придется установить `Python3` и `Pygments`, которые необходимы пакету `minted`.

* Устанавливаете Python3 и добавляете его расположение в переменную `PATH` (Панель управления - (ставите мелкие значки) - Учетные записи пользователей - Изменение переменных среды. Работает даже без отсутствия прав администратора).
* Открываете `cmd.exe` и вводите `python --version`.
* Вводите команду `python -m pip install pygments`. Если у вас нет прав администратора, то добавляете в конце ` --user`. 
	* Если вы у вас есть права администратора, то добавляете в `PATH` папку `Scripts` в папке установленного `Python`.
	* Если прав администратора у вас нет, то после установки в консоли выведется адрес, куда было установлено. Его надо скопировать и тоже добавить в переменную `PATH`.

В файле `my_code_insertion.tex` как раз показано использование этого пакета вместе с пакетом `tcolorbox` для красивой рамки вокруг кода.

Использование вставки кода из этого файла: `\mycodeinput{<language>}{<address to file>}{<title of code>}`. Пример: `\mycodeinput{c++}{C:/programs/a.cpp}{a.cpp}`.

[Документация по `minted`.](ftp://ftp.dante.de/tex-archive/macros/latex/contrib/minted/minted.pdf)

[Документация по `tcolorbox`.](https://mirror.hmc.edu/ctan/macros/latex/contrib/tcolorbox/tcolorbox.pdf)

[Стили подсветки кода в `minted`.](https://help.farbox.com/pygments.html) (выбираются опцией `\usemintedstyle{<стиль>}` в преамбуле)