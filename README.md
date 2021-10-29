# E-commerce-with-Vue-Django-Python

## E-commerce website build with Vue, Django &amp; Python

### Install dependecies:

-Python
-Django
-Pip
-Virtualenv
-Django-rest-framework
-Django-cors-headers
-Djoser
-Pillow
-Stripe

Create a virtualenv. Then install all the dependecies listed above.
For security add to urls.py ~
"from django.contrib import admin
from django.urls import path, include

urlpatterns = [
path('admin/', admin.site.urls),
path('api/v1/', include('djoser.urls')),
path('api/v1/', include('djoser.urls.authtoken')),
]"

For settings.py add these, or replace ~
"INSTALLED_APPS = [
'django.contrib.admin',
'django.contrib.auth',
'django.contrib.contenttypes',
'django.contrib.sessions',
'django.contrib.messages',
'django.contrib.staticfiles',
'rest_framework',
'rest_framework.authtoken',
'corsheaders',
'djoser',
]

CORS_ALLOWED_ORIGINS = [
"http://localhost:5050",
]

MIDDLEWARE = [
'django.middleware.security.SecurityMiddleware',
'django.contrib.sessions.middleware.SessionMiddleware',
'corsheaders.middleware.CorsMiddleware',
'django.middleware.common.CommonMiddleware',
'django.middleware.csrf.CsrfViewMiddleware',
'django.contrib.auth.middleware.AuthenticationMiddleware',
'django.contrib.messages.middleware.MessageMiddleware',
'django.middleware.clickjacking.XFrameOptionsMiddleware',
]"

Activate the environment using bash for Windows & Linux ~
$ source environment3_9/scripts/activate
Then run migrations ~
$ python manage.py makemigrations
$ python manage.py migrate

Create a superuser ~
$ python manage.py createsuperuser

_VUE SETUP_
npm install -g @vue/cli
vue create ecommerce-project with bellow settings ~
"Vue CLI v4.5.15
? Please pick a preset: Manually select features
? Check the features needed for your project: Choose Vue version, Babel, Router, Vuex, CSS Pre-processors
? Choose a version of Vue.js that you want to start the project with 3.x
? Use history mode for router? (Requires proper server setup for index fallback in production) Yes
? Pick a CSS pre-processor (PostCSS, Autoprefixer and CSS Modules are supported by default): Sass/SCSS (with dart-sass)
? Where do you prefer placing config for Babel, ESLint, etc.? In dedicated config files
? Save this as a preset for future projects? No"

Cd into project and instal some dependencies ~
Axios
Bulma / Alternative-Bootstrap

#_Font Awesome_
"https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta2/css/all.min.css"
