Deploying Flask Application on Ubuntu (Apache+WSGI)
        Required Packages:
              sudo apt-get install python3 python3-pip python3-venv
              sudo apt-get install apache2 libapache2-mod-wsgi-py3
        Set up your Flask application:
              mkdir home/user/api/pflask
              cd  home/user/api/pflask
              python3 -m venv venv (Avoid for Stable diffusion)
              source venv/bin/activate (Avoid for Stable diffusion)
              pip install flask
        Create app.py python file
              from flask import Flask
              app = Flask(__name__)
              @app.route('/')
              def hello():
                  return 'Hello, World!'
              export FLASK_APP=app.py 
              flask run

