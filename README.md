# E-commerce website build with Vue, Django &amp; Python

#### Install dependecies:

-Python <br />
-Django <br />
-Pip <br />
-Virtualenv <br />
-Django-rest-framework <br />
-Django-cors-headers <br />
-Djoser <br />
-Pillow <br />
-Stripe <br />

###Create a virtualenv. <br />
Then install all the dependecies listed above. <br />
For security add to urls.py ~ <br />

\*"from django.contrib import admin
from django.urls import path, include

urlpatterns = [
path('admin/', admin.site.urls),
path('api/v1/', include('djoser.urls')),
path('api/v1/', include('djoser.urls.authtoken')),
]"\*

For settings.py add these, or replace ~ <br />

\*"INSTALLED_APPS = [
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
]"\*

Activate the environment using bash for Windows & Linux ~ <br />
_$ source environment3_9/scripts/activate
Then run migrations ~
$ python manage.py makemigrations
$ python manage.py migrate_

Create a superuser ~
_$ python manage.py createsuperuser_

### _VUE SETUP_

npm install -g @vue/cli
vue create ecommerce-project with bellow settings ~ <br />
_"Vue CLI v4.5.15
? Please pick a preset: Manually select features
? Check the features needed for your project: Choose Vue version, Babel, Router, Vuex, CSS Pre-processors
? Choose a version of Vue.js that you want to start the project with 3.x
? Use history mode for router? (Requires proper server setup for index fallback in production) Yes
? Pick a CSS pre-processor (PostCSS, Autoprefixer and CSS Modules are supported by default): Sass/SCSS (with dart-sass)
? Where do you prefer placing config for Babel, ESLint, etc.? In dedicated config files
? Save this as a preset for future projects? No"_

Cd into project and instal some dependencies ~
_Axios
Bulma / Alternative-Bootstrap_

### _Font Awesome_

_"https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta2/css/all.min.css"_
