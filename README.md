# Disaster-Response-Pipelines

There is a huge opportunity of Machine Learning use cases to improve quick response in disaster recovery.In this project, I develop a machine learning pipeline to analyze real disaster data from Figure Eight with objective that these message categories will be viewed and sent to an appropriate disaster relief agency. 

# Installation
No extra libraries needs to be installed as all the libraries used here comes up wwith the Anaconda distribution with Python3.6.

Project Motivation
Incident managment has huge oppertunity around ML use case as these get generated from huge event log data. Here I thought to analyze Incident event data to see what hidden patterns will help us to come up with impactful ML use case.

File Descriptions
Below are the details of files:-

This project requires file:

  app

    # template # sub folder for html files
    master.html # main page of web app
    go.html # classification result page of web app
    
    run.py # Flask file that runs app
  models
  
     train_classifier.py
     classifier.pkl # will be saved model once you run the script
     
  data

    disaster_categories.csv # data to process
    disaster_messages.csv # data to process
    process_data.py
    DisasterResponse.db # database to save clean data to
    

# How To Interact With Your Project

1. Run the following commands in the project's root directory to set up your database and model.

    - To run ETL pipeline that cleans data and stores in database
        `python data/process_data.py data/disaster_messages.csv data/disaster_categories.csv data/DisasterResponse.db`
    - To run ML pipeline that trains classifier and saves
        `python models/train_classifier.py data/DisasterResponse.db models/classifier.pkl`

2. Run the following command in the app's directory to run your web app.
    `python run.py`

3. Go to http://0.0.0.0:3001/

# Licensing, Authors, Acknowledgements, Authors, Acknowledgements
Data is provided by Figure Eight.

