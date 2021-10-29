# E-commerce website build with Vue, Django &amp; Python

### Install dependecies:

-Python <br />
-Django <br />
-Pip <br />
-Virtualenv <br />
-Django-rest-framework <br />
-Django-cors-headers <br />
-Djoser <br />
-Pillow <br />
-Stripe <br />

### Create a virtualenv. <br />

Then install all the dependecies listed above. <br />
For security add to urls.py ~ <br />

\_"from django.contrib import admin
from django.urls import path, include

urlpatterns = [
path('admin/', admin.site.urls),
path('api/v1/', include('djoser.urls')),
path('api/v1/', include('djoser.urls.authtoken')),
]"\_

For settings.py add these, or replace ~ <br />

\*"INSTALLED_APPS = [<br />
'django.contrib.admin',<br />
'django.contrib.auth',<br />
'django.contrib.contenttypes',<br />
'django.contrib.sessions',<br />
'django.contrib.messages',<br />
'django.contrib.staticfiles',<br />
'rest_framework',<br />
'rest_framework.authtoken',<br />
'corsheaders',<br />
'djoser',<br />
]

CORS_ALLOWED_ORIGINS = [<br />
"http://localhost:5050",<br />
]

MIDDLEWARE = [<br />
'django.middleware.security.SecurityMiddleware',<br />
'django.contrib.sessions.middleware.SessionMiddleware',<br />
'corsheaders.middleware.CorsMiddleware',<br />
'django.middleware.common.CommonMiddleware',<br />
'django.middleware.csrf.CsrfViewMiddleware',<br />
'django.contrib.auth.middleware.AuthenticationMiddleware',<br />
'django.contrib.messages.middleware.MessageMiddleware',<br />
'django.middleware.clickjacking.XFrameOptionsMiddleware',<br />
]"\*

Activate the environment using bash for Windows & Linux ~ <br />
_$ source environment3_9/scripts/activate<br />
Then run migrations ~<br />
$ python manage.py makemigrations<br />
$ python manage.py migrate_<br />

Create a superuser ~ <br />
_$ python manage.py createsuperuser_<br />

### _VUE SETUP_

npm install -g @vue/cli <br />
vue create ecommerce-project with bellow settings ~ <br />
_"Vue CLI v4.5.15<br />
? Please pick a preset: Manually select features<br />
? Check the features needed for your project: Choose Vue version, Babel, Router, Vuex, CSS Pre-processors<br />
? Choose a version of Vue.js that you want to start the project with 3.x<br />
? Use history mode for router? (Requires proper server setup for index fallback in production) Yes<br />
? Pick a CSS pre-processor (PostCSS, Autoprefixer and CSS Modules are supported by default): Sass/SCSS (with dart-sass)<br />
? Where do you prefer placing config for Babel, ESLint, etc.? In dedicated config files<br />
? Save this as a preset for future projects? No"_<br />

Cd into project and instal some dependencies ~ <br />
_Axios<br />
Bulma / Alternative-Bootstrap_<br />

### _Font Awesome_

_"https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta2/css/all.min.css"_
