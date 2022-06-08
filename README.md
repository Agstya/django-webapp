mkdir django-webapp
cd ./django-webapp
code .
// Ctrl + `

git init
git status
git checkout -b main
git status

touch README.md
git status

touch .gitignore

echo "venv/" >> .gitignore
python -m venv venv
.\venv\Scripts\activate


python -m install Django
django-admin startproject globamantics
cd globalmantics
django-admin startapp store
ls
cd store
ls
cd ..
python manage.py runserver 
python manage.py migrate
python manage.py runserver 8080
pip install django-livesync