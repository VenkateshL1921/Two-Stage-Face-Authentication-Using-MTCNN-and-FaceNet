# Two Stage Face Authentication Using MTCNN and FaceNet

## Problem Statement
Build a system that authenticates the user based on the user details and face embeddings of the user.  

## Approach 
Building a system which is able to login the user if user is already register in system and then authenticate and grant permission/entry based on the similarity of face embedding stored in database and current face embedding. If user is not already registered, then redirect user to register page.
This is a two stage face authentication system which using MTCNN for face detection and FaceNet for extracting face embeddings. 
 
## Tech stack
1. Python
2. Deep learning
3. Fastapi 
4. MongoDB

## Architecture 
![Architecture](https://github.com/VenkateshL1921/Two-Stage-Face-Authentication-Using-MTCNN-and-FaceNet/assets/108605062/7c8105ba-328e-4fb3-81ef-24a4175abaeb)

## Running the system

### clone the repo
```
git clone https://github.com/VenkateshL1921/Two-Stage-Face-Authentication-Using-MTCNN-and-FaceNet.git
```

### create a virtual environment and activate it
```
a. python3 -m venv venv
b. source venv/bin/activate
```

### Install the libraries
```
pip install -r requirements.txt
```

### create a .env file and set the following environement variables
```
SECRET_KEY=KlgH6AzYDeZeGwD288to79I3vTHT8wp7
ALGORITHM=HS256
DATABASE_NAME='UserDB'
USER_COLLECTION_NAME='UserCollection'
EMBEDDING_COLLECTION_NAME='EmbeddingCollection'
MONGODB_URL_KEY= 
```

### Run the project
```
python3 app.py
```

