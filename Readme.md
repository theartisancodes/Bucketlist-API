# Bucketlist API

## Description
#### This is an API for an online bucket list.


# Requirements
```
Python 3.6
postgresql9.6
postman
```

# Installation

### 1)Clone the repo from GitHub:

```
git clone https://github.com/nzaujk/Bucketlist-API.git

```


### 2) cd to the root of the api
```
cd cp2
```

### 3) Create a virtual environment and install the necessary packages with:
```
$ pip install -r requirements.txt
```

# Launching the program
##### Create a database name
```
$ python manage.py createdb [dbname]
```
#### Enter the DATABASE URI at the config.py file
```
MY_DATABASE_URI = "postgresql://localhost/bucketlist_db"
```
####  Make migrations

```
$ python manage.py db init
$ python manage.py db migrate
$ python manage.py db upgrade
```
#### Runserver and add the endpoints to postman
```
$ python manage.py runserver
```
### Endpoints
```http://address/api/v1/auth/login```
```http://address/api/v1/auth/register```
```http://address/api/v1/bucketlists```
```http://address/api/v1/bucketlists/<int: bucketlist_id>```
```http://address/api/v1/bucketlists/<int: bucketlist_id>/items```
```http://address/api/v1/bucketlists/<int: bucketlist_id>/items/<int: item_id>```

# Running the tests

```
 $ nosetests
```

