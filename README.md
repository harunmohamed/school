<p align="center">
  <a href="https://github.com/harunmohamed/school">
    <img src="https://bit.ly/3bYmo7t" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Bambi School</h3>

  <p align="center">
    A Platform for Near East University Students to join communities around their courses and engage with each other.
    <br />
    <a href="#">View App</a>
    ·
    <a href="#">Report Bug</a>
    ·
    <a href="#">Request Feature</a>
  </p>
</p>


## Features

- Secure registration and authentication.
- Create communities.
- Create community posts.
- Reply to community posts.
- Edit or delete your communities, posts, and replies.
- Join communities.
- Get a feed of posts from your joined communities.
- Upvote or downvote posts and replies.
- Sort communities, posts, and replies by latest or most popular.
- Basic user profiles.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development. See deployment for notes on how to deploy the project.

### Prerequisites

To run this application you need [Python](https://www.python.org/), [pip](https://pip.pypa.io/en/stable/), and [SQLite](https://www.sqlite.org/).

### Local Setup

Clone the project.

```
git clone https://github.com/harunmohamed/school.git
```

Setup a `venv` and use `pip` to install the project dependencies.

```
cd flaskeddit
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

Set the `FLASK_APP` environment variable, create the SQLite database, and start the app. Now you can give the application a try at [http://localhost:5000](http://localhost:5000)!

```
export FLASK_APP=flaskeddit.py
flask cli create_db
flask run
```

You can also serve the application locally using [gunicorn](https://gunicorn.org/).

```
gunicorn "flaskeddit:create_app()"
```

## Testing

Flaskeddit is tested using pytest.

Use `pytest` to run the application's tests.

```
pytest
```

## Deployment

Flaskeddit is hosted on [Heroku](https://www.heroku.com/). To set up the required infrastructure for the project, you can use the [terraform-heroku-flask-postgres](https://github.com/aqche/terraform-heroku-flask-postgres) Terraform module.

The application is automatically deployed using [CircleCI](https://circleci.com/).

You can also use `git` to manually deploy the application.

```
export HEROKU_API_KEY="heroku_api_key"
export HEROKU_APP_NAME="heroku_app_name"
git push https://heroku:$HEROKU_API_KEY@git.heroku.com/$HEROKU_APP_NAME.git master
```

## Built With

- [Flask](http://flask.pocoo.org/) - Python Framework
- [Bootstrap](https://getbootstrap.com/) - CSS Framework

## Contributing

Feel free to submit a pull request!

## Authors

- **Harun Mohamed** - _Author_ - [harunmohamed](https://github.com/harunmohamed)


## License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for more details.

