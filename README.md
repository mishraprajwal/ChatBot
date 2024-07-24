# AskMeGPT

ChatBot is an interactive web application built using modern web technologies, designed to provide seamless chat interactions. This project leverages the power of OpenAI's GPT models to deliver intelligent responses to user inputs.

## Table of Contents

- [Features](#features)
- [Demo](#demo)
- [Installation](#installation)
- [Usage](#usage)
- [Technologies Used](#technologies-used)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Features

- **User Authentication**: Secure user registration and login.
- **Chat Functionality**: Real-time chat with AI-powered responses.
- **User Session Management**: Persistent user sessions with JWT-based authentication.
- **Responsive Design**: Accessible on both desktop and mobile devices.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/mishraprajwal/ChatBot.git
    cd ChatBot
    ```

2. Install the server-side dependencies:
    ```bash
    cd backend
    npm install
    ```

3. Install the client-side dependencies:
    ```bash
    cd ../frontend
    npm install
    ```

4. Create a `.env` file in the `backend` directory and add the following environment variables:
    ```env
    PORT=5001
    MONGO_URI=your_mongodb_connection_string
    JWT_SECRET=your_jwt_secret
    COOKIE_SECRET=your_cookie_secret
    OPENAI_API_KEY=your_openai_api_key
    ```

5. Start the development servers:
    ```bash
    # In the backend directory
    npm run dev

    # In the frontend directory
    npm run dev
    ```

## Usage

1. Open your browser and navigate to `http://localhost:5173`.
2. Register a new account or log in with your existing credentials.
3. Start chatting with the AI-powered bot.

## Technologies Used

### Backend
- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT for authentication

### Frontend
- React
- TypeScript
- Material-UI
- Axios

### AI Model
- OpenAI GPT-4

## API Endpoints

### User Routes

- `POST /api/v1/user/signup` - Register a new user
- `POST /api/v1/user/login` - User login
- `GET /api/v1/user/auth-status` - Check authentication status
- `GET /api/v1/user/logout` - User logout

### Chat Routes

- `POST /api/v1/chat/new` - Generate a new chat message
- `GET /api/v1/chat/all-chats` - Get all chat messages
- `DELETE /api/v1/chat/delete` - Delete all chat messages

## Contributing

We welcome contributions to this project. To contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add new feature'`).
5. Push to the branch (`git push origin feature-branch`).
6. Create a new Pull Request.

Please make sure to update tests as appropriate.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- [OpenAI](https://openai.com/) for providing the AI model.
- [Material-UI](https://mui.com/) for the UI components.
- All contributors and supporters of this project.
