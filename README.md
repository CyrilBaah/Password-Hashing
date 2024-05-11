# Password-Hashing
This is a Flask application demonstrating authentication features with password hashing.

## Technology Stack
- [Python](https://www.python.org/ "python")
- [SqlAchemy](https://docs.sqlalchemy.org/en/20/ "SqlAchemy")
- [Flask](https://flask.palletsprojects.com/en/3.0.x/ "Flask")

## How to set up locally
1. Clone the project.
```sh
 git clone https://github.com/CyrilBaah/Password-Hashing.git
```
```sh
 cd Password-Hashing
```
2. Create a virtualenv
```sh
 virtualenv env
 source env/bin/activate
```
3. Install the packages
```sh
 pip install -r requirements.txt
```
4. Start the Server
```sh
 python3 app.py 
```

## How to interact with the application API
Registration
```sh
curl -X POST http://127.0.0.1:5000/register -H "Content-Type: application/json" -d '{"username": "john_doe", "password": "password123"}'
```

Login
```sh
curl -X POST http://127.0.0.1:5000/login -H "Content-Type: application/json" -d '{"username": "john_doe", "password": "password123"}'
```