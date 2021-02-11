# Web App with Flask Server serving React Front-End #

## Set Up ##

Disclaimer: I haven't experimented with how much of this is actually necessary, but these are all the steps that I took before I set this up.

```
python3 -m venv venv
source venv/bin/activate
```

Then once you are in the virtual environment (you should see venv prepending all your commands in terminal), enter the following commands:

```
pip install flask python-dotenv
pip install -U flask-cors
```

Then, create your .env file:

```
touch .env
```

Open the .env file with your favorite editor and add the following configurations:

```
FLASK_APP=app.py
FLASK_ENV=development
```

## Execution ##

In order to run the web server, you will need two open terminals, one to run the react app and one to run the flask server. The React app is the main app that you interact with as a user, and it makes calls to the Flask server in the backend using the useEffect hook. 

From the root directory, enter the following command:

```flask run```

From react-flask-app, enter the following command:

```npm start```
