# Django [Volt Dashboard](https://appseed.us/generator/volt-dashboard/)

Open-source **Django Dashboard** generated by `AppSeed` on top of a modern design. **[Volt Dashboard](https://appseed.us/generator/volt-dashboard/)** is a free and open source `Bootstrap 5` Admin Dashboard featuring over 100 components, 11 example pages and 3 plugins with Vanilla JS. There are more than 100 free Bootstrap 5 components included some of them being buttons, alerts, modals, datepickers and so on.

- 👉 [Volt Dashboard Django](https://appseed.us/product/volt-dashboard/django/) - Product page
- 👉 [Complete documentation](https://docs.appseed.us/products/django-dashboards/volt) - `Learn how to use and update the product`
- ✅ [PRO Version Available](#pro-version) - `enhanced UI` and more `features` 
  
<br />

> Built with [Volt Dashboard Generator](https://appseed.us/generator/volt-dashboard/)

- Timestamp: `2022-06-23 20:04`
- Build ID: `c17f2093-7ee8-4540-a3f4-4f0da961f1e6`
- **Free [Support](https://appseed.us/support/)** (registered users) via `Email` and `Discord`

<br />

> Features

- `Up-to-date dependencies`
- Database: `mysql`
- UI-Ready app, Django Native ORM
- `Session-Based authentication`, Forms validation

<br />

![Volt Dashboard - Full-Stack Starter generated by AppSeed.](https://user-images.githubusercontent.com/51070104/168843604-b026fd94-5969-4be7-81ac-5887cf0958e5.png)

<br />




## ✨ Set up the MySql Database

**Note:** Make sure your Mysql server is properly installed and accessible. 

> **Step 1** - Create the MySql Database to be used by the app

- `Create a new MySql` database
- `Create a new user` and assign full privilegies (read/write)

<br />

> **Step 2** - Edit the `.env` to match your MySql DB credentials. Make sure `DB_ENGINE` is set to `mysql`.

- `DB_ENGINE`  : `mysql` 
- `DB_NAME`    : default value = `appseed_db`
- `DB_HOST`    : default value = `localhost`
- `DB_PORT`    : default value = `3306`
- `DB_USERNAME`: default value = `appseed_db_usr`
- `DB_PASS`    : default value = `pass`

<br />

Here is a sample:  

```txt
# .env sample

DB_ENGINE=mysql             # Database Driver
DB_NAME=appseed_db          # Database Name
DB_USERNAME=appseed_db_usr  # Database User
DB_PASS=STRONG_PASS_HERE    # Password 
DB_HOST=localhost           # Database HOST, default is localhost 
DB_PORT=3306                # MySql port, default = 3306 
```

<br />


## ✨ How to use it

> Download the code 

```bash
$ # Get the code
$ git clone https://github.com/appseed-projects/c17f2093-7ee8-4540-a3f4-4f0da961f1e6.git
$ cd c17f2093-7ee8-4540-a3f4-4f0da961f1e6
```

<br />

### 👉 Set Up for `Unix`, `MacOS` 

> Install modules via `VENV`  

```bash
$ virtualenv env
$ source env/bin/activate
$ pip3 install -r requirements.txt
```

<br />

> Set Up Database

```bash
$ python manage.py makemigrations
$ python manage.py migrate
```

<br />

> Start the app

```bash
$ python manage.py runserver
```

At this point, the app runs at `http://127.0.0.1:8000/`. 

<br />

### 👉 Set Up for `Windows` 

> Install modules via `VENV` (windows) 

```
$ virtualenv env
$ .\env\Scripts\activate
$ pip3 install -r requirements.txt
```

<br />

> Set Up Database

```bash
$ python manage.py makemigrations
$ python manage.py migrate
```

<br />

> Start the app

```bash
$ python manage.py runserver
```

At this point, the app runs at `http://127.0.0.1:8000/`. 

<br />

### 👉 Create Users

By default, the app redirects guest users to authenticate. In order to access the private pages, follow this set up: 

- Start the app via `flask run`
- Access the `registration` page and create a new user:
  - `http://127.0.0.1:8000/register/`
- Access the `sign in` page and authenticate
  - `http://127.0.0.1:8000/login/`

<br />

## ✨ Code-base structure

The project is coded using a simple and intuitive structure presented below:

```bash
< PROJECT ROOT >
   |
   |-- core/                               # Implements app configuration
   |    |-- settings.py                    # Defines Global Settings
   |    |-- wsgi.py                        # Start the app in production
   |    |-- urls.py                        # Define URLs served by all apps/nodes
   |
   |-- apps/
   |    |
   |    |-- home/                          # A simple app that serve HTML files
   |    |    |-- views.py                  # Serve HTML pages for authenticated users
   |    |    |-- urls.py                   # Define some super simple routes  
   |    |
   |    |-- authentication/                # Handles auth routes (login and register)
   |    |    |-- urls.py                   # Define authentication routes  
   |    |    |-- views.py                  # Handles login and registration  
   |    |    |-- forms.py                  # Define auth forms (login and register) 
   |    |
   |    |-- static/
   |    |    |-- <css, JS, images>         # CSS files, Javascripts files
   |    |
   |    |-- templates/                     # Templates used to render pages
   |         |-- includes/                 # HTML chunks and components
   |         |    |-- navigation.html      # Top menu component
   |         |    |-- sidebar.html         # Sidebar component
   |         |    |-- footer.html          # App Footer
   |         |    |-- scripts.html         # Scripts common to all pages
   |         |
   |         |-- layouts/                   # Master pages
   |         |    |-- base-fullscreen.html  # Used by Authentication pages
   |         |    |-- base.html             # Used by common pages
   |         |
   |         |-- accounts/                  # Authentication pages
   |         |    |-- login.html            # Login page
   |         |    |-- register.html         # Register page
   |         |
   |         |-- home/                      # UI Kit Pages
   |              |-- index.html            # Index page
   |              |-- 404-page.html         # 404 page
   |              |-- *.html                # All other pages
   |
   |-- requirements.txt                     # Development modules - SQLite storage
   |
   |-- .env                                 # Inject Configuration via Environment
   |-- manage.py                            # Start the app - Django default start script
   |
   |-- ************************************************************************
```

<br />



## PRO Version

> For more components, pages and priority on support, feel free to take a look at this amazing starter:

Volt Pro is a premium Bootstrap 5 Admin Dashboard featuring over 800 components, 20 example pages and 10 fully customized plugin written in Vanilla Javascript. 

- 👉 [Django Volt PRO](https://appseed.us/product/volt-dashboard-pro/django/) - product page
  - ✅ `Enhanced UI` - more pages and components
  - ✅ `Priority` on support

<br >

![Volt Dashboard PRO - Starter generated by AppSeed.](https://user-images.githubusercontent.com/51070104/172672843-8c40a801-3438-4e9c-86db-38a34191fbdf.png)

<br />

---
Django [Volt Dashboard](https://appseed.us/generator/volt-dashboard/) - Open-source starter generated by **[AppSeed Generator](https://appseed.us/generator/)**.
