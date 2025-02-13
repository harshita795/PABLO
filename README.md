# SNAPBAZAR

## Overview

SNAPBAZAR is a JavaScript project designed to manage user data and images. It provides functionalities for creating new users, searching for images, saving images, adding tags to images, and displaying search history.

## Features

- **Create New User**: Allows for the creation of a new user with a username and email.
- **Search Images**: Enables users to search for images.
- **Save Images**: Allows users to save images.
- **Add Tags to Images**: Users can add tags to specific images.
- **Search Images by Tags**: Enables searching for images based on tags.
- **Display Search History**: Displays the search history of users.

## Getting Started

### Prerequisites

Before you begin, ensure you have met the following requirements:
- Node.js and npm are installed.
- Your operating system is Windows, Linux, or Mac.

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/harshita795/PABLO-776F61.git
    ```
2. Navigate to the project directory:
    ```sh
    cd PABLO-776F61
    ```
3. Install the dependencies:

    ```sh
    npm install
    ```

## Usage

To use this project, follow these steps:

1. Start the server:

    ```sh
    npm start
    ```
2. Use the following API endpoints:
    - `POST /api/users`: Create a new user
    - `GET /api/search/photos`: Search for images
    - `POST /api/photos`: Save images
    - `POST /api/photos/:photoId/tags`: Add tags to images
    - `GET /api/photos/tag/search`: Search images by tags
    - `GET /api/search-history`: Display search history

Example Command:
```sh
curl -X POST http://localhost:3000/api/users -d '{"username": "user1", "email": "user1@example.com"}'
```



# 🚀 Picstoria - A Photo Curation App

![Picstoria Banner](https://source.unsplash.com/1600x400/?photography,nature)

📸 *Picstoria* is a powerful photo curation application that allows users to search, save, tag, and manage photos from the Unsplash API. Built with *Node.js, Express, Sequelize, and SQLite*, this project ensures seamless API interactions and efficient database management.

---

## 📂 Project Setup

### 1️⃣ Install Dependencies 📦
bash
npm install


### 2️⃣ Environment Variables 🌍
Create a .env file in the root directory and add the following:
ini
UNSPLASH_ACCESS_KEY=your_unsplash_access_key


### 3️⃣ Database Setup 🛢️
bash
npx sequelize-cli db:migrate


### 4️⃣ Run the Server 🚀
bash
npm start


---

## 📜 Features & API Endpoints

### 📝 *1. User Management*
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST | /api/users | Create a new user |

### 📷 *2. Photo Search (Unsplash API)*
| Method | Endpoint | Query Params | Description |
|--------|---------|--------------|-------------|
| GET | /api/photos/search | query (e.g., nature) | Search photos from Unsplash |

### 🖼️ *3. Save Photos*
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST | /api/photos | Save photos to collections |

### 🔖 *4. Add Tags to Photos*
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST | /api/photos/:photoId/tags | Add tags to a photo |

### 🔍 *5. Search Photos by Tags & Sort by Date*
| Method | Endpoint | Query Params | Description |
|--------|---------|--------------|-------------|
| GET | /api/photos/tag/search | tags, sort, userId | Search photos by tag and sort |

### 🕵️‍♂️ *6. Track & Display Search History*
| Method | Endpoint | Query Params | Description |
|--------|---------|--------------|-------------|
| GET | /api/search-history | userId | Retrieve user's search history |

---

## 🛠️ Technologies Used

- *Backend*: Node.js, Express.js
- *Database*: SQLite, Sequelize ORM
- *API*: Unsplash API
- *Testing*: Jest

---

## ✅ Running Tests 🧪

To run unit and integration tests, use:
bash
npm test


---

## 🌟 Contributing
Feel free to contribute by submitting pull requests! 😊

---

## 📜 License
This project is licensed under the MIT License. 📝

---

## 📬 Contact
📧 Email: your.email@example.com  
🐦 Twitter: [@yourhandle](https://twitter.com/yourhandle)  
📷 Unsplash: [@yourprofile](https://unsplash.com/@yourpro
