# Planner

This is an **Ultimate Planner Project** (using **UV python package manager**).

![Planner](./Planner.avif)

## Features

- Add and Track Your Routines
- Track Your Habits
- Track Your Sleep
- Track Your Mood
- Organize Your Daily Notes
- Financial Management
- Track Your Daily Studying
- Track Your Goals
- Develop Your Reading
- Learn From Your Day
- etc.

## Tech Stack

- **Backend:** Django, Django REST Framework
- **BacFrontend:** HTML, CSS, Bootstrap
- **Database:** PostgreSQL
- **Other:** Docker,Uv package manager, Shell

## Setup

To run project locally, in production or using Docker you need to setup environment variables first. Rename the `.env.example` to `.env` and fill the required values.

You can also use this command in linux for ease of use to have `.env` file in `/backend` directory as well:

```bash
ln -s ../.env backend/.env
```

### Backend Setup (Django)

1. Install dependencies:
First install [uv package manager](https://docs.astral.sh/uv/getting-started/installation/) (feel free to read [uv documents](https://docs.astral.sh/uv/getting-started/))

   ```bash
   pip install uv
   ```

2. install packages:

   ```bash
   cd backend
   uv sync
   ```

3. Run migrations:

   ```bash
   uv run manage.py makemigrations
   uv run manage.py migrate
   ```

4. Start the backend server:

   ```bash
   uv run manage.py runserver
   ```

### Running with Docker

- Just build and start all services **(recommended)**:
  
   ```bash
   docker compose up --build
   ```

## Project Structure

Brief overview of the main directories and their purposes.

```bash
Template
├── backend          # Django project
├── compose.yaml     # Docker Compose file
├── dockerfiles      # Docker files
├── frontend         # frontend codes
├── .env.example     ## .env.example file which must be
│                    ## modified like mentioned in 'Setup'
├── LICENSE
└── README.md
```

## Contributing

Contributions are always welcome!

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a pull request

## License

This project is licensed under the [MIT](https://choosealicense.com/licenses/mit/).
