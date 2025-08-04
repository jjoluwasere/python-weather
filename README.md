# Flask Weather App

This is a beginner-friendly Flask web application that displays current weather information for any city using the OpenWeatherMap API.

You can search a city, see the current temperature, weather conditions, and get a graceful fallback if the city is not found.

---

## Live Demo

🔗 [https://python-weather-g3rp.onrender.com/weather?city=London](https://python-weather-g3rp.onrender.com/weather?city=London)

---

## Features

-  Search weather by city
-  See temperature, conditions, and "feels like" data
-  Handles invalid cities
-  Clean UI with basic styling
-  Easy to deploy on [Render](https://render.com)

---
<br>
<br>

## Technologies Used
<br>

-  Python 3
-  Flask
-  Requests (API calls)
-  Waitress (production-ready WSGI server)
-  OpenWeatherMap API
-  HTML5 & CSS3

<br>

## Set Up a Virtual Environment (Optional but Recommended)
<br>

python -m venv venv
source venv/bin/activate  # (macOS/Linux)
<br>

## Install dependencies
<br>

pip install -r requirements.txt
<br>

## Get an OpenWeatherMap API Key
<br>

-  Go to https://openweathermap.org/api
-  Sign up and get a free API key
<br>

## Create a .env file
<br>

-  Create a .env file in the project root and add the line:
-  API_KEY=your_openweathermap_api_key
<br>

---

## Deploying to Render
<br>
You can deploy this app for free using <a href="https://render.com" target="_blank">Render</a>:

<ol>
  <li><strong>Push your code to a GitHub repository.</strong></li>
  <li>Go to <a href="https://render.com">https://render.com</a> and sign up or log in.</li>
  <li>Click <strong>"New" → "Web Service"</strong>.</li>
  <li>Connect your GitHub repo and choose this project.</li>
  <li>Fill in the deploy settings as follows:<br><br>
    <code>Environment:</code> Python<br>
    <code>Build Command:</code> <code>pip install -r requirements.txt</code><br>
    <code>Start Command:</code> <code>python server.py</code>
  </li>
  <li>Add your API key under <strong>Environment → Environment Variables</strong>:<br><br>
    <code>Key:</code> <code>API_KEY</code><br>
    <code>Value:</code> <code>your_openweathermap_api_key</code>
  </li>
  <li>Click <strong>"Create Web Service"</strong>.</li>
</ol>

Render will automatically build and host your app at a public URL like:<br>
<code>https://your-app-name.onrender.com</code>

<br>

Try accessing:<br>
<code>https://your-app-name.onrender.com/weather?city=London</code><br>
or simply:<br>
<code>https://your-app-name.onrender.com/</code>
