# Команды git pull и git fetch
Загрузить содержимое из удаленного репозитория можно с помощью двух команд: ***git pull*** и ***git fetch***.
## git fetch
Команда __git fetch__ загружает коммиты, файлы и ссылки из удаленного репозитория в ваш локальный репозиторий.
## git pull
Команда __git pull__ используется для извлечения и загрузки содержимого 
из удаленного репозитория и немедленного обновления локального репозитория этим содержимым.

Команда __git pull__ на самом деле представляет собой комбинацию двух других команд: __git fetch__ и __git merge__.
Сначала команда __git pull__ запускает команду __git fetch__ для загрузки содержимого из указанного удаленного репозитория.
Затем выполняется команда __git merge__, объединяющая ссылки и указатели удаленного содержимого в новый локальный коммит слияния.

## Отличие команд
Команду __git fetch__ можно считать _«безопасным»_ вариантом, а __git pull__ — _«небезопасным»_. Команда __git fetch__ загружает удаленное содержимое,
но не изменяет состояние локального репозитория, в то время как __git pull__ загружает удаленное содержимое и сразу пытается изменить 
состояние локального репозитория, чтобы оно соответствовало этому содержимому.
Это может привести к возникновению непредумышленного конфликта в локальном репозитории.

