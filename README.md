# Django-Chat-Application
Video Tutorial for this project
https://youtu.be/SQ4A7Q6_md8


Getting the files
Download zip file
or
git clone command (need git to be installed) and remove git folder afterwards

git clone https://github.com/andyjud/django-starter.git . && rm -rf .git




Setup
- Create Virtual Environment
# Mac
python3 -m venv venv
source venv/bin/activate
# Windows
python3 -m venv venv
.\venv\Scripts\activate.bat

- Install dependencies
pip install --upgrade pip
pip install -r requirements.txt

- Migrate to database
python manage.py migrate
python manage.py createsuperuser

- Run application
python manage.py runserver

- Generate Secret Key ( ! Important for deployment ! )
python manage.py shell
from django.core.management.utils import get_random_secret_key
print(get_random_secret_key())
exit()
