# Assistant intelligent dans la gestion d’un drive d’entreprise
## Installation
+ Python 3
+ [Google Cloud SDK 226.0.0](https://cloud.google.com/sdk/install)
## Preparation
./
```
├─ main.py                # Web application router
├─ process.py           # Request handler
├─ nltk_data              # nltk package 
├─ profiles_fr_en       # language profiles
├─ settings                # google cloud storage credential
├─ static                    # css, js, pictures
├─ templates             # html files
├─ requirements.txt   # web application dependencies 
├─ app.yaml               # GAE app config
└─ cron.yaml              # GAE Cron jobs config
```
requirements.txt
```
+ Flask==1.0.2
+ nltk==3.4
+ pandas==0.23.4
+ gensim==3.7.0
+ scikit-learn==0.20.3
+ PyDrive==1.3.1
+ stop-words==2018.7.23
+ PyYAML==3.13
+ pdfminer3k==1.3.1
+ python-pptx==0.6.17
+ python-docx==0.8.10
+ langdetect==1.0.7
+ google-cloud-storage==1.14.0
+ xlrd==1.2.0
+ SQLAlchemy==1.2.18
+ PyMySQL==0.9.3
+ gunicorn==19.7.1
```
## Deployment on local machine
Create an isolated Python environment in a directory external to the project and activate it:
```bash
$ python3 install --upgrade virtualenv
$ cd your-project
$ virtualenv --python python3 env
# activate the virtual environment
$ source env/bin/activate 
```
Install dependencies:
```bash
$ pip3 install -r requirements.txt
```
Run the application:
```bash
$ python3 main.py
```
In your web browser, enter the following address:
```
http://localhost:8080
```
Learn more about Google App Engine
+ [Quickstart in Google App Engine](https://cloud.google.com/appengine/docs/standard/python3/quickstart)

## Deployment on Google Cloud Platform
Create a Google Cloud Projet
+  <a href="https://cloud.google.com/resource-manager/docs/creating-managing-projects" target="_blank">Tutorial</a>

Google Cloud SDK workflow
```bash
# install init Google Cloud SDK, login your google account, choose project, etc...
$ gcloud init

# Go to application root directory:
$ cd /application-root-directory

#deploy web application on Google Cloud
$ gcloud app deploy app.yaml

#deploy cron jobs
$ gcloud app deploy cron.yaml
```
## Block Diagram
![image](https://github.com/mengyingWU/Assistant-intelligent-dans-la-gestion-d-un-drive-d-entreprise/blob/master/image.png)

## User Manul


## References
+ <a href="https://developers.google.com/appengine/downloads" target="_blank">Google App Engine SDK</a>
+ <a href="https://pypi.org/project/python-docx" target="_blank">python-docx</a>
+ <a href="https://pypi.org/project/PyDrive" target="_blank">Pydrive</a>
+ <a href="https://pypi.org/project/python-pptx" target="_blank">python-pptx</a>
+ <a href="https://pypi.org/project/pdfminer3k" target="_blank">pdfminer3k</a>
+ <a href="https://pypi.org/project/python-pptx" target="_blank">python-pptx</a>
+ <a href="https://pypi.org/project/langdetect" target="_blank">langdetect</a>
