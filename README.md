# Instagram & YouTube Downloader Bot

A Telegram bot built with Python that helps users download supported media from Instagram and YouTube directly through Telegram.

This project demonstrates practical experience with asynchronous programming, modular application architecture, database integration, and Telegram bot development.

## Features

- **Instagram Downloads** — Process supported Instagram media links.
- **YouTube Downloads** — Process supported YouTube video links.
- **Video Quality Selection** — Support for selecting video resolution where available.
- **Database Integration** — Store and manage user-related data.
- **Middleware** — Handle user registration and request rate limiting.
- **Admin Functionality** — Separate administrative handlers.
- **Interactive Interface** — Use Telegram commands and inline keyboards.
- **Modular Codebase** — Separate application components for maintainability.
- **Asynchronous Operations** — Use Python's asynchronous programming capabilities.

## Technologies

- Python
- aiogram 3
- SQLite
- aiosqlite
- yt-dlp
- Instaloader
- aiohttp
- python-dotenv
- aiofiles

## Project Structure

```text
Instagram-and-Youtube-Downloader/
├── data/
├── handlers/
├── keyboards/
├── middlewares/
├── services/
├── states/
├── test_downloads/
├── config.py
├── database.py
├── main.py
├── requirements.txt
└── README.md
```

## Getting Started

### Prerequisites

- Python installed on your computer
- pip
- A Telegram bot token obtained through [@BotFather](https://t.me/BotFather)

### Installation

**1. Clone the repository**

```bash
git clone https://github.com/moonlycrush/Instagram-and-Youtube-Downloader.git
cd Instagram-and-Youtube-Downloader
```

**2. Create a virtual environment**

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

On macOS or Linux:

```bash
source venv/bin/activate
```

**3. Install dependencies**

```bash
pip install -r requirements.txt
```

**4. Configure the bot**

Configure your Telegram bot token using the environment variable or configuration method expected by the application.

For local development, keep secrets in a `.env` file and exclude it from Git using `.gitignore`.

Example `.env` entry:

```env
BOT_TOKEN=your_telegram_bot_token
```

Never publish your actual bot token in source code, screenshots, or repository files.

**5. Start the bot**

```bash
python main.py
```

## Architecture

The application is organized into separate modules:

- `handlers/` — Processes Telegram commands and user interactions.
- `keyboards/` — Defines interactive Telegram keyboards.
- `middlewares/` — Handles registration and request-rate control.
- `services/` — Contains supporting application services.
- `states/` — Organizes conversational states.
- `database.py` — Provides database-related functionality.
- `config.py` — Holds application configuration.
- `main.py` — Entry point for starting the bot.

This structure helps separate responsibilities and makes the application easier to maintain and extend.

## Potential Improvements

- Add a managed download queue for concurrent requests.
- Improve error handling and user-facing download progress.
- Add automated tests for download services and database operations.
- Implement structured logging and performance monitoring.
- Introduce configurable download limits and file-size validation.
- Containerize the application with Docker.

## Responsible Use

This project is intended for educational and personal use. Users should respect copyright, privacy, and the terms of service of the platforms involved. Download only content they are authorized to access and save.

## Author

**GitHub:** [@moonlycrush](https://github.com/moonlycrush)

---

*Developed with Python and aiogram.*
