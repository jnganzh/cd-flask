# Continuous Delivery with Flask Google Cloud Platform Hello-ml

Source code to set up a Continuous Delivery Flask app

## Replicate this project

**1. Open the Google Cloud Platform Console then activate Cloud Shell.**

**2. Run the following code in the Cloud Shell.**

### Clone the repo and enter the directory

```
gcloud config set project $GOOGLE_CLOUD_PROJECT
git clone git@github.com:jnganzh/cd-flask.git
cd cd-flask-app
```

### Create a virtual environment

```
virtualenv --python $(which python3) venv
source venv/bin/activate
```
### Install the required packages

```
make install
```

**3. View the Flask code in python in the main.py file, make any required changes.**

```
python main.py
```

**4. Follow on the link and play around with the website. The following website routes are available:**

/pandas
/wikipedia/<search term>
/html
/crypto
  
**5. When satisfied deploy the code to the cloud with the following command:**

```
gcloud app deploy
```

**6. Set up the continuous delivery by linking the repo to cloud build on google cloud platform, triggering it when you push anything to github.**

For more info click [here](https://cloud.google.com/source-repositories/docs/quickstart-triggering-builds-with-source-repositories).
