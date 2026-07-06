# Flask GitHub OAuth Demo

A simple Flask application that demonstrates authentication with GitHub using OAuth 2.0.

## Features

- Sign in with GitHub
- Retrieve and display the authenticated user's GitHub username
- Session-based authentication
- Logout functionality

## Tech Stack

- Python
- Flask
- OAuth 2.0
- Requests-OAuthlib
- python-dotenv

## Installation

### 1. Clone the repository

```bash
git clone git@github.com:Mati-Joseph/github-auth-login.git
cd github-auth-login
```

### 2. Create and activate a virtual environment

```bash
pipenv shell
```

or

```bash
python -m venv .venv
source .venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Create a GitHub OAuth App

Create an OAuth application in GitHub Developer Settings and configure:

- Homepage URL: `http://127.0.0.1:5000/`
- Authorization Callback URL: `http://127.0.0.1:5000/callback`

### 5. Create a `.env` file

```env
CLIENT_ID=your_github_client_id
CLIENT_SECRET=your_github_client_secret
REDIRECT_URI=http://127.0.0.1:5000/callback
```

## Run the Application

```bash
python app.py
```

Open your browser and visit:

```text
http://127.0.0.1:5000
```

## Project Structure

```text
.
├── app.py
├── .env
├── requirements.txt
├── templates
│   ├── index.html
│   └── access_denied.html
└── README.md
```

## License

This project is intended for learning and demonstration purposes.
