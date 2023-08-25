# A Simple Flask Shopify App

This is a simple Python-flask 3rd party app built using Shopify API.
## What does this sample do?

Very simply, this sample will create the server-side component for your Shopify app and provide you with some basic tools that you can build on to create a robust commercial application.

## Setup
1. Install dependencies for the Python module flask and request if you have not installed it.
```
pip3 install module_name
```

2. Run the app locally. If you are located in the root directory:
```
python3 src/server.py
```
Leave this running. If new changes fail to appear, restart the server.

3. Set up [ngrok](https://ngrok.com/) by installing it and running it locally.
```
ngrok http 5000
```
Throughout the development process, ngrok should be running in the background. You will not need to restart this, as you will generate a new URL.

4. Set up your Shopify app, by following [these](https://github.com/garettB/shopify-flask-example#app-creation) steps.

5. Create a local `.env` file by copying over the template. 
```
cp ./src/.env.template .env
```

6. Fill out your `.env` file using your Shopify API key and Shopify secret key. Replace `your_server.hostname` with your ngrok base URL. Please don't put quotations around the values.

7. Now, first we have to create a Shopify store to test the app we have created. Install the app onto a Shopify test store by following [these](https://github.com/garettB/shopify-flask-example#ready-to-test) steps.

8. You should be redirected to the admin dashboard of your test store. The URL should be formatted as follows
```
https://{{store_name}}.myshopify.com/admin/apps/{{app_name}}/app_launched
```


For more information, follow this [link](https://github.com/garettB/shopify-flask-example#app-creation).

