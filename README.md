![GitHub User's stars](https://img.shields.io/github/stars/RajKKapadia?style=for-the-badge)
![GitHub followers](https://img.shields.io/github/followers/RajKKapadia?style=for-the-badge)

# WhatsApp-OpenAI Connection
Hi everyone, this is repository for my personal demo project on connecting Twilio and OpenAI to provide answers to all the users questions using OpenAI GPT-3. This is written in `Python` and served with `Flask`. This bot can only handle:
* text messgaes

### Youtube
I have recorded a quick video on the setup of this chat-bot, in case you want to replicate the work, you can watch it [here](https://youtu.be/uxY3__IkozM).

### What you will need
There are couple of things that you need before you get started following this repository.
* OpenAI API key, since it is open to all, you can create an account [here](https://openai.com/) and access the key.
* You need a Twilio project, you can get `Account SID` and `Auth Token` for that project, we will need this to make requests. You can get it from [here](https://console.twilio.com/).
* API requesting application like Postman, Insomnia, etc.
* NGROK for local testing.

### How to use it
To replicate the work of this repository and run it locally, you need to follow these steps:
* create a `.env` file inside the root directory, create these environmental variables:
    ```
    TWILIO_ACCOUNT_SID=YOUR ACCOUNT SID
    TWILIO_AUTH_TOKEN=YOUR AUTH TOKEN
    OPENAI_API_KEY=YOUR OPENAI API KEY
    FROM=whatsapp:+14155238886
    ```
This FROM variable in the .env file is same for the Twilio WhatsApp Sandbox.
* create a virtual environment and activate it before installing the packages
* install all the required dependencies from the `requirements.txt` file
```python
pip install -r requirements.txt
```
* run the server with either of the following commands
```python
python run.py
```
```python
gunicorn run:app
```
* start NGROK engine on the same port as the python application is running.
* provide the NGROk urlon `Twilio WhatsApp Sandbox` for all incoming request.
* test the setup using your WhatsApp

# About me
I am `Raj Kapadia`, I am passionate about `AI/ML/DL` and their use in different domains, I also love to build `chatbots` using `Google Dialogflow ES/CX`, I have backend development experience with Python[Flask], and NodeJS[Express] For any work, you can reach out to me at...

* [LinkedIn](https://www.linkedin.com/in/rajkkapadia/)
* [Fiverr](https://www.fiverr.com/rajkkapadia​)
* [Upwork](https://www.upwork.com/freelancers/~0176aeacfcff7f1fc2)
* [Youtube](https://www.youtube.com/channel/UCOT01XvBSj12xQsANtTeAcQ)
