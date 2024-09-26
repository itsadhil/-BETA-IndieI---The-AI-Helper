
# (BETA) IndieI: The AI Helper
![Alt Text](https://i.giphy.com/media/v1.Y2lkPTc5MGI3NjExNHpyOWV0NDZnaWpxazUycmxoa3J0ZHptZDUyMXg1YzBqczUxemo3YyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/3PDvpg23RRZYWjGhQB/giphy.gif)

Here’s how the README structure will look with the added **Warning** section:

---

### Introduction

This project is an AI-powered chatbot application designed to interact with users through a web interface, powered by **React** on the front end and **FastAPI** on the backend. The chatbot leverages various AI and automation capabilities to assist users in performing tasks, fetching information, and even posting content directly to LinkedIn.

At its core, this chatbot is built to provide seamless interactions by understanding user queries and responding intelligently. It is capable of performing tasks such as:

- **Web scraping**: Extracting content from the web based on user queries and returning relevant information.
- **LinkedIn integration**: Allowing users to retrieve LinkedIn profiles and create posts on their LinkedIn account through the chatbot interface.
- **File uploads**: Supporting file attachments (such as images), enabling users to include media in their LinkedIn posts.
- **Real-time communication**: Using WebSockets to ensure smooth, dynamic conversations between the user and the AI without constant page reloads.

The chatbot has been designed to assist in real-world tasks such as content creation, social media management, and automation, while offering a user-friendly interface for interaction. Whether it's searching for web data or drafting professional content for LinkedIn, the chatbot streamlines these actions with a conversational interface.

---

### Warning

**Please note**: 
- The **LinkedIn profile retrieval** and **LinkedIn posting** features of this bot are not demonstrated here due to the potential violation of LinkedIn's Terms of Service (TOS). 
- To avoid any issues, these functionalities have been restricted for public demonstration. 
- If you wish to explore these features, you can clone the repository and run the bot locally using your own LinkedIn credentials to test these capabilities.

---

### Features

This AI-powered chatbot comes packed with several useful features, designed to simplify web interaction, automate tasks, and enhance user engagement. Below is a list of its key features:

![Alt Text](https://i.giphy.com/media/v1.Y2lkPTc5MGI3NjExNDZ4eG53N2Vjb25lcWlneHdsNDlidmd1emNoN2ZlZHU1bmZ2c3JtMSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/zXjU2KAdPyokEKx5ZQ/giphy.gif)

1. **Web Scraping**:
   - Users can input queries, and the bot scrapes relevant information from the web.
   - Automatically fetches summaries of web content and displays them in the chat.

2. **LinkedIn Profile Fetching**:
   - Users can request information about LinkedIn profiles using their LinkedIn credentials.
   - Retrieves profile data such as work experience, education, and other relevant sections (restricted for demo purposes).

3. **LinkedIn Post Creation**:
   - The bot can generate content for LinkedIn posts based on the user's topic request.
   - Allows the user to upload images to accompany the post.
   - Directly posts the content to the user’s LinkedIn profile using LinkedIn API (restricted for demo purposes).

4. **File Uploads**:
   - Supports file uploads (e.g., images) which can be included in LinkedIn posts.
   - The uploaded files are displayed within the chat interface for visual feedback.

5. **Real-time Interaction**:
   - Communication with the chatbot is facilitated via WebSockets, enabling real-time interaction.
   - Users can have smooth and dynamic conversations without page reloads or interruptions.

6. **Dark Mode**:
   - The interface includes a dark mode option for a comfortable user experience.
   - Users can toggle dark mode from the options menu.

7. **Custom Cookie Management**:
   - Users can input their `li_at` and `JSESSION` cookies to authenticate LinkedIn requests.
   - This allows the bot to perform LinkedIn tasks on behalf of the user.

8. **File Attachment (Clip Icon)**:
   - A clip icon is present in the chat, enabling users to attach files (e.g., images).
   - The attached images are shown within the chat as part of the conversation.

---

### How to Use

Follow these steps to run and interact with the AI-powered chatbot:

1. **Clone the Repository**:
   - Clone this repository to your local machine using:
     ```bash
     git clone https://github.com/your-repo/your-project.git
     ```

2. **Install Dependencies**:
   - Navigate to the project directory and install the necessary dependencies for both the backend and frontend.
     ```bash
     # For the backend (FastAPI, WebSockets, LinkedIn API, etc.):
     pip install -r requirements.txt

     # For the frontend (React):
     cd frontend
     npm install
     ```

3. **Run the Backend API**:
   - Start the FastAPI backend server, which handles the web scraping, LinkedIn profile fetching, and LinkedIn posting features. Make sure to run all required Python scripts to ensure the API functions correctly.
     ```bash
     uvicorn main:app --reload --host 0.0.0.0 --port 9090
     ```
   - Ensure that `main.py` and other relevant Python scripts are running for the API to work.

4. **Run the WebSocket Server**:
   - Open another terminal window to start the WebSocket server that powers the chatbot’s real-time interaction.
     ```bash
     python websocket_server.py
     ```

5. **Run the Frontend (React)**:
   - After setting up the backend, start the React frontend, which provides the user interface for interacting with the bot.
     ```bash
     cd frontend
     npm start
     ```

6. **Interact with the Chatbot**:
   - Open your browser and navigate to `http://localhost:3000`.
   - You’ll see the chat interface where you can start interacting with the bot by typing messages.

7. **Using the Web Scraping Feature**:
   - Type something like "Search for the latest news about AI," and the bot will retrieve and display information from the web.

8. **Using the LinkedIn Profile Fetching Feature**:
   - Type "Fetch LinkedIn profile for {username}," and the bot will pull the requested profile data if you have provided valid LinkedIn authentication cookies.

9. **Creating LinkedIn Posts**:
   - Type "I want to post on LinkedIn about {your topic}," and the bot will generate content based on your input.
   - If you want to add an image to the post, you can upload one by clicking the paper clip icon.
   - If you’ve provided valid LinkedIn credentials, the bot will post directly to your profile.

10. **Dark Mode**:
    - You can toggle dark mode by clicking the **Options** button in the sidebar and switching the **Dark Mode** toggle.

11. **Custom Cookie Authentication**:
    - To interact with LinkedIn, you’ll need to enter your `li_at` and `JSESSION` cookies in the **Options** section for authentication.

---






