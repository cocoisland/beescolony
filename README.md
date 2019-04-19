# beescolony
Beescolony app.py is created using Dash plotly.
1. To turn on production, 
   Change app.run_server(debug=True) to app.run_server()
   Add app = dash.Dash(__name__, external_stylesheets=external_stylesheets)
   server = app.server
2. Create virtual env, python -m venv new_env
3. Install dash and gunicorn library
   pip install dash==0.39.0  # The core dash backend
   pip install dash-daq==0.1.0  # DAQ components (newly open-sourced!)
   pip install gunicorn
4. Create Procfile with 'web: gunicorn app:server'
   Testing : gunicorn app:server, to make sure everything run properly.
5. pip freeze > requirements.txt, to create requirement environment for Heroku to setup.

This beescolony repo is created to be deployed to Heroku.
On Heroku
1. Create an app
2. Deploy with GitHub

If successfully deployed, application.herokuapps.com will be given.


