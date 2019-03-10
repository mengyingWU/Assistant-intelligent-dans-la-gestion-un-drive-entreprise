# Assistant-intelligent-dans-la-gestion-d-un-drive-d-entreprise
## Tutorial on how to run a Flask-based application on Google App Engine

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
## Deployment
+ [Quickstart in Google App Engine](https://cloud.google.com/appengine/docs/standard/python3/quickstart)
## References
+ <a href="https://developers.google.com/appengine/downloads" target="_blank">Google App Engine SDK</a>
+ <a href="https://pypi.org/project/python-docx" target="_blank">python-docx</a>
+ <a href="https://pypi.org/project/PyDrive" target="_blank">Pydrive</a>
+ <a href="https://pypi.org/project/python-pptx" target="_blank">python-pptx</a>
+ <a href="https://pypi.org/project/pdfminer3k" target="_blank">pdfminer3k</a>
+ <a href="https://pypi.org/project/python-pptx" target="_blank">python-pptx</a>
+ <a href="https://pypi.org/project/langdetect" target="_blank">langdetect</a>


