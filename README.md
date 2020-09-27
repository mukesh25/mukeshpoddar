# mukeshpoddar
Deploy Django App to Heroku
Usage
If you don't have git installed
make a copy of your project or seprate git branch
Add your dependencies to requirements.txt by typing in the terminal

pip freeze > requirements.txt
pip install gunicorn whitenoise
(gunicorn is used by heroku to run server)

MIDDLEWARE=[
'whitenoise.middleware.WhiteNoiseMiddleware'
]
Add this in settings.py

STATIC_ROOT = os.path.join(BASE_DIR, 'static/')

Make a Heroku account
Download Heroku CLI
Configure Django Heroku


In your terminal type it

git init
git add .
git commit -m "first commit"
git push heroku master

---------------------------------------
heroku create app_name
heroku destroy app_name
