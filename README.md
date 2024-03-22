# Chatbot Deployment with Flask and JavaScript



This gives 2 deployment options:
- Deploy within Flask app with jinja2 template
- Serve only the Flask prediction API. The used html and javascript files can be included in any Frontend application (with only a slight modification) and can run completely separate from the Flask App then.

## project description: 

A Flask-based Python web app offers diverse healthcare services: chatbot, doctor appointments, exercise guides,Yoga/Meditation tips, and diet plans. Prioritizes user-friendly interface and holistic well-being.
It includes features such as a chatbot for interactive communication, appointment booking with specialized doctors and exercise guides, Yoga and Meditation tips, and a diet plan.
The application offers a user-friendly interface and a range of features to cater to different aspects of health & well-being.



## Initial Setup for chat bot:
This repo currently contains the starter files.

Clone repo and create a virtual environment
```
$ git clone https://github.com/python-engineer/chatbot-deployment.git
$ cd chatbot-deployment
$ python3 -m venv venv
$ . venv/bin/activate
```
Install dependencies
```
$ (venv) pip install Flask torch torchvision nltk
```
Install nltk package
```
$ (venv) python
>>> import nltk
>>> nltk.download('punkt')
```
Modify `intents.json` with different intents and responses for your Chatbot

Run
```
$ (venv) python train.py
```
This will dump data.pth file. And then run
the following command to test it in the console.
```
$ (venv) python chat.py
```

