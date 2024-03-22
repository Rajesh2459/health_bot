# Chatbot Deployment with Flask and JavaScript



This gives 2 deployment options:
- Deploy within Flask app with jinja2 template
- Serve only the Flask prediction API. The used html and javascript files can be included in any Frontend application (with only a slight modification) and can run completely separate from the Flask App then.

## project description: 

A Flask-based Python web app offers diverse healthcare services: chatbot, doctor appointments, exercise guides,Yoga/Meditation tips, and diet plans. Prioritizes user-friendly interface and holistic well-being.
It includes features such as a chatbot for interactive communication, appointment booking with specialized doctors and exercise guides, Yoga and Meditation tips, and a diet plan.
The application offers a user-friendly interface and a range of features to cater to different aspects of health & well-being.

## Services Provided :

1. User Authentication:
   
- Implement user signup, login, and logout functionalities.
     
- Store user information in a database (e.g., SQLite).
    
2. Chatbot with NLP:
   
- Integrate a natural language processing (NLP) engine to understand user queries.
-Create intents for health-related questions, symptoms, medication information, and general health advice.
    
3.Health Information:

- Based on the user's query, fetch relevant health information from reliable sources or a predefined database.
-	Provide accurate and concise responses to user queries.
  
4.Appointment Booking:
 	
-	 Allow users to schedule appointments with doctors of specific specializations.
- 	Store appointment details in the database (date, time, doctor, user, etc.).
  
5.User Interface:
  - design a user-friendly interface for interacting with the chatbot.
 -Implement a responsive design for both desktop and mobile.

6.Backend Processing:

- Implement backend logic to handle user queries, process appointments, and interact with the database.



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

## Screenshots 
1.Login Page: 

![Screenshot (114)](https://github.com/Rajesh2459/health_bot/assets/131291830/aacd7e0a-1c6d-4428-b714-fafdc720816f)

2.Signup Page:

![Screenshot (115)](https://github.com/Rajesh2459/health_bot/assets/131291830/49a4cf2e-4dfa-4900-ab9d-b938aba4e8cd)

3.Dashboard page:

![Screenshot (116)](https://github.com/Rajesh2459/health_bot/assets/131291830/509686b1-836c-400a-9f65-fb59d40ace3f)
![Screenshot (117)](https://github.com/Rajesh2459/health_bot/assets/131291830/1052b0fb-73d9-4423-b1e8-1e74393c6bba)
![Screenshot (118)](https://github.com/Rajesh2459/health_bot/assets/131291830/1edd2576-d1c8-460e-86c2-43240dfd2b78)



4.challenges Page:

![Screenshot (121)](https://github.com/Rajesh2459/health_bot/assets/131291830/b38f3389-15d5-4a79-9f9d-e2b6ff78bd04)

5.Review Page:

![Screenshot (122)](https://github.com/Rajesh2459/health_bot/assets/131291830/93bf6ec4-d4ef-45b5-8299-476197387f9d)

6.appointment booking:

![Screenshot (119)](https://github.com/Rajesh2459/health_bot/assets/131291830/f67b6b3e-cfcc-414e-9a04-c2bb110df3ae)
![Screenshot (120)](https://github.com/Rajesh2459/health_bot/assets/131291830/08ad2899-9f0d-4018-8b38-d9fcd252c8ae)
