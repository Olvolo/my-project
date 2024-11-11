# my-project

# Инициализация нового Git-репозитория
git init

# Создание .gitignore и добавление в него правил игнорирования
echo "*.sass" >> .gitignore
echo "bin/" >> .gitignore
echo "admin/" >> .gitignore
echo "config/" >> .gitignore

# Добавление всех файлов в локальное хранилище (индексация)
git add .

# Коммит всех текущих файлов в основную ветку
git commit -m "Initial commit with .gitignore"

# Создание новой ветки и переход в неё
git branch new-branch
git checkout new-branch

# Создание папки blog и файлов index.js, index.html
mkdir blog
touch blog/index.js blog/index.html

# Добавление папки blog в коммит и его создание
git add blog/
git commit -m "Add blog folder with index.js and index.html"

# Возвращение в основную ветку (main)
git checkout main

# Подключение к удаленному репозиторию (замените <URL-репозитория> на адрес вашего удаленного репозитория)
git remote add origin <URL-репозитория>

# Отправка основной ветки на удаленный репозиторий
git push -u origin main
