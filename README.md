# Instructions for installationa and activation of conda environment and flask


Create a requirements.text and Paste the following segments in it:

+ aniso8601==9.0.1
+ click==8.0.4
+ colorama==0.4.4
+ Flask==2.0.3
+ Flask-Cors==3.0.10
+ Flask-RESTful==0.3.9
+ itsdangerous==2.1.0
+ Jinja2==3.0.3
+ MarkupSafe==2.1.0
+ numpy==1.22.2
+ pandas==1.4.1
+ python-dateutil==2.8.2
+ pytz==2021.3
+ scipy==1.8.0
+ six==1.16.0
+ Werkzeug==2.0.3
+ azure-keyvault-secrets==4.3.0
+ azure-storage-blob==12.10.0
+ azure-identity==1.8.0
+ pyodbc==4.0.32

Save and close.

Then Enter the following commands :

+ conda create --name dni_env --file requirements.txt

If installation fails for some packages in this statement then try commenting them out.

+ pip install waitress - if needed

The above two statments have to be executed only during first installation.

The below statements have to executed after every restart

+ conda activate dni_env

+ waitress-serve --p 8000 backend.wsgi:app

Attach DataService.js inside the service folder in front end file.Then perform necessary changes in code to import and execute DataService.

Then execute frontend using npm run start.



