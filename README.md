# soren-0930

## Project Description

This python repository is intended to showcase and test NER with a Fast API service and h2o_wave UI, both of which are executed with a single Docker Compose. In future iterations of this project, I aim to better use the displaCy visualization and allow for more training of the spaCy program to make it both more accurate and more efficient.

---

## Table of Contents

- [Named Entity Recognition](#named-entity-recognition)
    - [What Is NER?](#what-is-ner)
    - [Why Use NER?](#why-use-ner)
    - [How To Use This Project](#how-to-use-this-project)
- [Test Run](#test-run)
    - [NER Initial Screen](#ner-initial-screen)
    - [NER Raw Output](#ner-raw-output)
    - [NER Visualizer](#ner-visualizer)
- [Technologies](#technologies)
    - [python3](#python3)
    - [Spacy v3](#spacy-v3)
    - [Fast API](#fast-api)
    - [h2o_wave](#h2o_wave)
    - [Docker Engine](#docker-engine)
    - [Docker Compose](#docker-compose)
- [Conclusion](#conclusion)
    - [Credits](#credits)
    - [Thanks](#thanks)
    
## Named Entity Recognition
### What is NER?
Named-Entity Recognition or NER is known by a few names: Entity Identification, Entity Chunking, and Entity Extraction. It is defined as "a subtask of information extraction that seeks to locate and classify named entities mentioned in unstructured text. 
=> Entities refer to specifics such as names, places, dates, phone #'s, etc.
=> Unstructured texts refer to written work such as books, chapters, articles, journals, etc.
=> NER Platforms most commonly used are GATE, OpenNLP, and SpaCy(which is the one we will be using)

### Why Use NER?
With big tech companies as well as big news corporation amassing PETABYTES of data per day, there is a need for fast and more efficient ways of sorting and analyzing data. The fastest way to do it is through a machine learning algorithm like NER. Having NER quickly identify specifics in a text gives any user the opportunity to sort through immense amounts of unfiltered data.

### How To Use This Project
If you are new to NER's, please read through this README document as it highlights all of the technologies used. As of how to run the code, perform the following 2 commands in your main directory in order to activate:

```sh
  docker-compose build
  docker-compose up
```

To deactivate, all you have to do is the opposite of the latter statement or ctrl+c in your terminal:

```sh
  docker-compose down
```

## Test Run
The last thing I want to do before getting into what tools I used is both showcase the capability of the NER and show you what the v1.0 and v1.1 outputs will look like, so you are not confused as to why the UI looks a certain way! I thought that the best way to do this would be by inputting an entire transcript of a movie. For this example, I have chosen to copy and paste the [entire transcript of one of my favorites; Dreamworks Animations, "Bee Movie,"](http://www.script-o-rama.com/movie_scripts/a1/bee-movie-script-transcript-seinfeld.html) staring Jerry Seinfeld. Even with the pages of text, the program gave outputs in a matter of seconds!

### NER Initial Screen
You will first be greeted by a friendly message asking you for text to be NERded.

<a href="https://imgur.com/b6nE4Rh">
    <img src="https://i.imgur.com/b6nE4Rh.png" width="400" height="800"  alt="START"/>
</a>

### NER Raw Output
Once you finish typing in your text, you press the button and the first thing you will see (other than the titling) is a raw dict output. It displays the starting index of the special word, the ending index of the special word, the label for the special word, and finally the special word itself. This raw data gives programmers, data analysts, and machine learning programs many opportunities to sort relevant and irrelevant data based on these key words.

<a href="https://imgur.com/eVHkHaC">
    <img src="https://i.imgur.com/eVHkHaC.png" width="400" height="800"  alt="RAW LIST"/>
</a>

### NER Visualizer
Finally for the most beautiful part of the program, the visualizer. Seeing your submitted text annotated through the program and returned as html is incredibly satisfying and it gives you an oppportunity to sort through your text and spot out people, places, or dates you may have previously missed.

<a href="https://imgur.com/iqHPJUC">
    <img src="https://i.imgur.com/iqHPJUC.png" width="400" height="800"  alt="VISUALIZER"/>
</a>

## Technologies
### python3

<a href="https://www.python.org/">
    <img src="https://www.python.org/static/img/python-logo.png" width="400" height="100"  alt="PYTHON"/>
</a>

The current version, as well as the version this project uses, of python is 3.10.5. You may be asking, why python? Python is currently one of the best fit programming languages for machine learning for many reasons: 1) Its simplicity and legibility 2) Easy access to modules/libraries that support machine learning 3) The programming community is in consistent support of the language. More on this topic in the following sections when we begin displaying some code!


### spaCy v3
<a href="https://spacy.io/">
    <img src="https://spacy.io/static/social_default-1d3b50b1eba4c2b06244425ff0c49570.jpg" width="400" height="100" alt="SPACY"/>
</a>

The current version, as well as the version this project uses, of spaCy is 3.3. With easy customization, fast training, and access to larger word vectors than most other Natural Language Processing libraries, it is easy to see why spaCy was chosen over the alternatives.


### Fast API
<a href="https://fastapi.tiangolo.com/">
    <img src="https://fastapi.tiangolo.com/img/logo-margin/logo-teal.png" width="400" height="100" alt="FAST API"/>
</a>

Fast API is a python-based web framework to create Rest API's. If you are new to API's, a Rest API is an interface that allows multiple systems to communicate information securely. 


### h2o_wave
<a href="https://wave.h2o.ai/">
    <img src="https://wave.h2o.ai/img/logo.svg" width="400" height="100" alt="H2O WAVE"/>
</a>

H2O Wave is another python-based web framework to create real time applications with complex visualizations. This is especially important in the field of machine learning and data science as the UI enables users to process data in a simplistic manner and achieve detailed graphics.

### Docker Engine
<a href="https://docs.docker.com/engine/">
    <img src="https://docs.docker.com/images/docker-icon.svg" width="400" height="100" alt="DOCKER ENGINE"/>
</a>

Docker Engine is an open-source containerization engine that allows the user to build their program within a container, allowing others ease of access to program without having to download specific libraries or other necessary components beforehand. Docker Engine also acts as a client-server application with a background process that handles requests. Finally, Docker Engine has a command line interface client that proves incredibly handy for docker newbs like me to debug.

### Docker Compose
<a href="https://docs.docker.com/compose/">
    <img src="https://quintagroup.com/cms/technology/Images/docker-compose-button.jpg" width="400" height="100" alt="DOCKER COMPOSE"/>
</a>

Docker Compose is what allows the whole project to be linked and bundled together. Compose both defines our containers and runs them, all with a single command.

## Conclusion
### Credits
Thank you to Marcel Neuhausler and ISS for the fun and intense project. I have never been tasked with learning so many new programs in such a small amount of time. I really do hope to publish another like this one soon!

### Thanks
I hope you, the viewer of this project, enjoyed my first README and project, and are able to take something from it to use in your own projects! Happy coding :3
-From, Soren S.
