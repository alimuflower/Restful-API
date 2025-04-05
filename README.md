CIS376 - Software Engineering II
Winter 2025
Assignment 02 - RESTful API for Favorite Tweets
Ali Almuthafar

---

📁 Project Overview

This project implements a RESTful API using Python and Flask that reads a JSON archive of favorite tweets and provides endpoints to access tweet and user information. The JSON file (`favs.json`) contains tweets exported from Twitter.

---

📂 Project Structure

CIS376-Assignment02-TweetAPI/
├── app/
│   ├── app.py         # Main Flask app with all API routes
│   ├── favs.json      # JSON file of favorite tweets (from assignment link)
├── requirements.txt   # Flask dependency
├── README.txt         # This instruction file

---

⚙️ How to Set Up and Run

1. Open Command Prompt
2. Navigate to the project folder:
   cd C:\Users\<alililmu>\CIS376-Assignment02-TweetAPI

3. Create and activate the virtual environment:
   python -m venv venv
   venv\Scripts\activate

4. Install required packages:
   pip install -r requirements.txt

5. Navigate to the `app` folder:
   cd app

6. Run the Flask application:
   python app.py

You should see:
 * Running on http://127.0.0.1:5000/

---

 API Endpoints

1. GET /tweets
   → Returns all tweets with created_at, id, and text.

2. GET /tweets/links
   → Returns all external links found in tweet text, grouped by tweet id.

3. GET /tweets/<tweet_id>
   → Returns details of a specific tweet (created_at, text, screen_name).

4. GET /users/<screen_name>
   → Returns user profile info: location, description, followers, and friends count.

---



- http://127.0.0.1:5000/tweets
- http://127.0.0.1:5000/tweets/links
- http://127.0.0.1:5000/tweets/1513101571237437441
- http://127.0.0.1:5000/users/foyzulhassan

