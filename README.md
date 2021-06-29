# Django Email App

Automated contact form made with Django, Django environ and your personal email address.

## Features

- Let's you send mails with your personal email account

- Django settings depending on environmental variables

- Automated contact form with the following fields:
  - `name`
  - `email`
  - `subject`
  - `message`

## Requirements

- [Python 3](https://www.python.org/downloads/)

## Set Up

Clone the repository and enter to the project folder:

```bash
git clone https://github.com/DaniDiazTech/Email-Django-app.git

cd Email-Django-app/EmailProject/
```

Create a virtual environment and activate it:

```bash
python -m venv .venv && source .venv/bin/activate
```

Install the project dependencies with the following command:

```bash
pip install -r requirements.txt
```

Enter to the project settings folder (`EmailProject/EmailProject`), and create an `.env` file with the following information:

```python
EMAIL_HOST=smtp.gmail.com
EMAIL_HOST_USER=YourEmail@address
EMAIL_HOST_PASSWORD=YourAppPassword
RECIPIENT_ADDRESS=TheRecieverOfTheMails
```

Where the `EMAIL_HOST` depends on your personal email provider SMTP server.

Finally, run the server and visit your [localhost](http://localhost:8000).

```bash
ls
manage.py # Make sure you're inside the directory where manage.py is located

python manage.py runserver
```
