# NOVA: AI-Driven Adaptive Learning System

NOVA is an AI-powered, adaptive learning platform built on the [Full-Stack FastAPI Template](https://github.com/fastapi/full-stack-fastapi-template). It is designed to assist users in improving their knowledge and skills through summarization, Q&A generation, and personalized learning pathways. Leveraging cutting-edge machine learning models, NOVA offers an intelligent and customizable learning experience.


[//]: # (<a href="https://github.com/fastapi/full-stack-fastapi-template/actions?query=workflow%3ATest" target="_blank"><img src="https://github.com/fastapi/full-stack-fastapi-template/workflows/Test/badge.svg" alt="Test"></a>)

[//]: # (<a href="https://coverage-badge.samuelcolvin.workers.dev/redirect/fastapi/full-stack-fastapi-template" target="_blank"><img src="https://coverage-badge.samuelcolvin.workers.dev/fastapi/full-stack-fastapi-template.svg" alt="Coverage"></a>)

## Technology Stack and Features

- ⚡ [**FastAPI**](https://fastapi.tiangolo.com) for the Python backend API.
    - 🧰 [SQLModel](https://sqlmodel.tiangolo.com) for the Python SQL database interactions (ORM).
    - 🔍 [Pydantic](https://docs.pydantic.dev), used by FastAPI, for the data validation and settings management.
    - 💾 [PostgreSQL](https://www.postgresql.org) as the SQL database.
- 🚀 [React](https://react.dev) for the frontend.
    - 💃 Using TypeScript, hooks, Vite, and other parts of a modern frontend stack.
    - 🎨 [Chakra UI](https://chakra-ui.com) for the frontend components.
    - 🤖 An automatically generated frontend client.
    - 🧪 [Playwright](https://playwright.dev) for End-to-End testing.
    - 🦇 Dark mode support.
- 🐋 [Docker Compose](https://www.docker.com) for development and production.
- 🔒 Secure password hashing by default.
- 🔑 JWT (JSON Web Token) authentication.
- 📫 Email based password recovery.
- ✅ Tests with [Pytest](https://pytest.org).
- 📞 [Traefik](https://traefik.io) as a reverse proxy / load balancer.
- 🚢 Deployment instructions using Docker Compose, including how to set up a frontend Traefik proxy to handle automatic HTTPS certificates.
- 🏭 CI (continuous integration) and CD (continuous deployment) based on GitHub Actions.

[//]: # (### Dashboard Login)

[//]: # ()
[//]: # ([![API docs]&#40;img/login.png&#41;]&#40;https://github.com/fastapi/full-stack-fastapi-template&#41;)

[//]: # ()
[//]: # (### Dashboard - Admin)

[//]: # ()
[//]: # ([![API docs]&#40;img/dashboard.png&#41;]&#40;https://github.com/fastapi/full-stack-fastapi-template&#41;)

[//]: # ()
[//]: # (### Dashboard - Create User)

[//]: # ()
[//]: # ([![API docs]&#40;img/dashboard-create.png&#41;]&#40;https://github.com/fastapi/full-stack-fastapi-template&#41;)

[//]: # ()
[//]: # (### Dashboard - Items)

[//]: # ()
[//]: # ([![API docs]&#40;img/dashboard-items.png&#41;]&#40;https://github.com/fastapi/full-stack-fastapi-template&#41;)

[//]: # ()
[//]: # (### Dashboard - User Settings)

[//]: # ()
[//]: # ([![API docs]&#40;img/dashboard-user-settings.png&#41;]&#40;https://github.com/fastapi/full-stack-fastapi-template&#41;)

[//]: # ()
[//]: # (### Dashboard - Dark Mode)

[//]: # ()
[//]: # ([![API docs]&#40;img/dashboard-dark.png&#41;]&#40;https://github.com/fastapi/full-stack-fastapi-template&#41;)

[//]: # ()
[//]: # (### Interactive API Documentation)

[//]: # ()
[//]: # ([![API docs]&#40;img/docs.png&#41;]&#40;https://github.com/fastapi/full-stack-fastapi-template&#41;)

[//]: # ()
[//]: # (## How To Use It)

[//]: # ()
[//]: # (You can **just fork or clone** this repository and use it as is.)

[//]: # ()
[//]: # (✨ It just works. ✨)

[//]: # ()
[//]: # (### How to Use a Private Repository)

[//]: # ()
[//]: # (If you want to have a private repository, GitHub won't allow you to simply fork it as it doesn't allow changing the visibility of forks.)

[//]: # ()
[//]: # (But you can do the following:)

[//]: # ()
[//]: # (- Create a new GitHub repo, for example `my-full-stack`.)

[//]: # (- Clone this repository manually, set the name with the name of the project you want to use, for example `my-full-stack`:)

[//]: # ()
[//]: # (```bash)

[//]: # (git clone git@github.com:fastapi/full-stack-fastapi-template.git my-full-stack)

[//]: # (```)

[//]: # ()
[//]: # (- Enter into the new directory:)

[//]: # ()
[//]: # (```bash)

[//]: # (cd my-full-stack)

[//]: # (```)

[//]: # ()
[//]: # (- Set the new origin to your new repository, copy it from the GitHub interface, for example:)

[//]: # ()
[//]: # (```bash)

[//]: # (git remote set-url origin git@github.com:octocat/my-full-stack.git)

[//]: # (```)

[//]: # ()
[//]: # (- Add this repo as another "remote" to allow you to get updates later:)

[//]: # ()
[//]: # (```bash)

[//]: # (git remote add upstream git@github.com:fastapi/full-stack-fastapi-template.git)

[//]: # (```)

[//]: # ()
[//]: # (- Push the code to your new repository:)

[//]: # ()
[//]: # (```bash)

[//]: # (git push -u origin master)

[//]: # (```)

[//]: # ()
[//]: # (### Update From the Original Template)

[//]: # ()
[//]: # (After cloning the repository, and after doing changes, you might want to get the latest changes from this original template.)

[//]: # ()
[//]: # (- Make sure you added the original repository as a remote, you can check it with:)

[//]: # ()
[//]: # (```bash)

[//]: # (git remote -v)

[//]: # ()
[//]: # (origin    git@github.com:octocat/my-full-stack.git &#40;fetch&#41;)

[//]: # (origin    git@github.com:octocat/my-full-stack.git &#40;push&#41;)

[//]: # (upstream    git@github.com:fastapi/full-stack-fastapi-template.git &#40;fetch&#41;)

[//]: # (upstream    git@github.com:fastapi/full-stack-fastapi-template.git &#40;push&#41;)

[//]: # (```)

[//]: # ()
[//]: # (- Pull the latest changes without merging:)

[//]: # ()
[//]: # (```bash)

[//]: # (git pull --no-commit upstream master)

[//]: # (```)

[//]: # ()
[//]: # (This will download the latest changes from this template without committing them, that way you can check everything is right before committing.)

[//]: # ()
[//]: # (- If there are conflicts, solve them in your editor.)

[//]: # ()
[//]: # (- Once you are done, commit the changes:)

[//]: # ()
[//]: # (```bash)

[//]: # (git merge --continue)

[//]: # (```)

[//]: # ()
[//]: # (### Configure)

[//]: # ()
[//]: # (You can then update configs in the `.env` files to customize your configurations.)

[//]: # ()
[//]: # (Before deploying it, make sure you change at least the values for:)

[//]: # ()
[//]: # (- `SECRET_KEY`)

[//]: # (- `FIRST_SUPERUSER_PASSWORD`)

[//]: # (- `POSTGRES_PASSWORD`)

[//]: # ()
[//]: # (You can &#40;and should&#41; pass these as environment variables from secrets.)

[//]: # ()
[//]: # (Read the [deployment.md]&#40;./deployment.md&#41; docs for more details.)

[//]: # ()
[//]: # (### Generate Secret Keys)

[//]: # ()
[//]: # (Some environment variables in the `.env` file have a default value of `changethis`.)

[//]: # ()
[//]: # (You have to change them with a secret key, to generate secret keys you can run the following command:)

[//]: # ()
[//]: # (```bash)

[//]: # (python -c "import secrets; print&#40;secrets.token_urlsafe&#40;32&#41;&#41;")

[//]: # (```)

[//]: # ()
[//]: # (Copy the content and use that as password / secret key. And run that again to generate another secure key.)

[//]: # ()
[//]: # (## How To Use It - Alternative With Copier)

[//]: # ()
[//]: # (This repository also supports generating a new project using [Copier]&#40;https://copier.readthedocs.io&#41;.)

[//]: # ()
[//]: # (It will copy all the files, ask you configuration questions, and update the `.env` files with your answers.)

[//]: # ()
[//]: # (### Install Copier)

[//]: # ()
[//]: # (You can install Copier with:)

[//]: # ()
[//]: # (```bash)

[//]: # (pip install copier)

[//]: # (```)

[//]: # ()
[//]: # (Or better, if you have [`pipx`]&#40;https://pipx.pypa.io/&#41;, you can run it with:)

[//]: # ()
[//]: # (```bash)

[//]: # (pipx install copier)

[//]: # (```)

[//]: # ()
[//]: # (**Note**: If you have `pipx`, installing copier is optional, you could run it directly.)

[//]: # ()
[//]: # (### Generate a Project With Copier)

[//]: # ()
[//]: # (Decide a name for your new project's directory, you will use it below. For example, `my-awesome-project`.)

[//]: # ()
[//]: # (Go to the directory that will be the parent of your project, and run the command with your project's name:)

[//]: # ()
[//]: # (```bash)

[//]: # (copier copy https://github.com/fastapi/full-stack-fastapi-template my-awesome-project --trust)

[//]: # (```)

[//]: # ()
[//]: # (If you have `pipx` and you didn't install `copier`, you can run it directly:)

[//]: # ()
[//]: # (```bash)

[//]: # (pipx run copier copy https://github.com/fastapi/full-stack-fastapi-template my-awesome-project --trust)

[//]: # (```)

[//]: # ()
[//]: # (**Note** the `--trust` option is necessary to be able to execute a [post-creation script]&#40;https://github.com/fastapi/full-stack-fastapi-template/blob/master/.copier/update_dotenv.py&#41; that updates your `.env` files.)

[//]: # ()
[//]: # (### Input Variables)

[//]: # ()
[//]: # (Copier will ask you for some data, you might want to have at hand before generating the project.)

[//]: # ()
[//]: # (But don't worry, you can just update any of that in the `.env` files afterwards.)

[//]: # ()
[//]: # (The input variables, with their default values &#40;some auto generated&#41; are:)

[//]: # ()
[//]: # (- `project_name`: &#40;default: `"FastAPI Project"`&#41; The name of the project, shown to API users &#40;in .env&#41;.)

[//]: # (- `stack_name`: &#40;default: `"fastapi-project"`&#41; The name of the stack used for Docker Compose labels and project name &#40;no spaces, no periods&#41; &#40;in .env&#41;.)

[//]: # (- `secret_key`: &#40;default: `"changethis"`&#41; The secret key for the project, used for security, stored in .env, you can generate one with the method above.)

[//]: # (- `first_superuser`: &#40;default: `"admin@example.com"`&#41; The email of the first superuser &#40;in .env&#41;.)

[//]: # (- `first_superuser_password`: &#40;default: `"changethis"`&#41; The password of the first superuser &#40;in .env&#41;.)

[//]: # (- `smtp_host`: &#40;default: ""&#41; The SMTP server host to send emails, you can set it later in .env.)

[//]: # (- `smtp_user`: &#40;default: ""&#41; The SMTP server user to send emails, you can set it later in .env.)

[//]: # (- `smtp_password`: &#40;default: ""&#41; The SMTP server password to send emails, you can set it later in .env.)

[//]: # (- `emails_from_email`: &#40;default: `"info@example.com"`&#41; The email account to send emails from, you can set it later in .env.)

[//]: # (- `postgres_password`: &#40;default: `"changethis"`&#41; The password for the PostgreSQL database, stored in .env, you can generate one with the method above.)

[//]: # (- `sentry_dsn`: &#40;default: ""&#41; The DSN for Sentry, if you are using it, you can set it later in .env.)

## Backend Development

Backend docs: [backend/README.md](./backend/README.md).

## Frontend Development

Frontend docs: [frontend/README.md](./frontend/README.md).

## Deployment

Deployment docs: [deployment.md](./deployment.md).

## Development

General development docs: [development.md](./development.md).

This includes using Docker Compose, custom local domains, `.env` configurations, etc.

## Release Notes

Check the file [release-notes.md](./release-notes.md).

## License

NOVA is licensed under the terms of the MIT license.
