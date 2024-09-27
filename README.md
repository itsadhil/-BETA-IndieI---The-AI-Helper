
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
- The **LinkedIn profile retrieval** feature of this bot are not demonstrated here due to the potential violation of LinkedIn's Terms of Service (TOS).
- This scraper is made just because we couldnt get our comapny verified, If you have a verified Linkedin company, Use it in the linkedin_api.py code and The Bot Will work fine without breaking TOS.
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

12 **Memory and Context Handling**:
   - The bot can remember past interactions and use them to provide context-aware responses.
   - User queries are stored in a memory file (JSON format) to ensure personalized interactions based on prior conversations.

13. **Network Packet Analysis (Beta)**:
   - IndieI can now interface with network devices to analyze packet transmissions.
   - Users can visualize packet transmission statistics in real-time, such as packets per second and device-specific network traffic.

14. **Topic-Based Post Scheduling for LinkedIn**:
   - Users can instruct the bot to create and schedule posts on LinkedIn on specific topics at predefined times.
   - Supports both text-based and multimedia posts, including image attachments.

15. **Enhanced Pattern Matching for Search Results**:
   - IndieI uses advanced pattern-matching algorithms to rank and filter search results, delivering the most relevant web content.
   - Users can expect more accurate results based on their queries by assigning points to matched keywords in search results.

16. **Expanded Language Model Integration (LLaMA 3.1)**:
   - Powered by the LLaMA 3.1 model, IndieI provides detailed and thorough summaries from web content and LinkedIn profile information.
   - The model supports large text inputs by dividing them into manageable sections and summarizing each part before merging the content.

17. **Enhanced LinkedIn Posting with Image Support**:
   - Users can now directly upload images through the chat interface and include them in LinkedIn posts.
   - The bot handles image processing and LinkedIn API integration to publish the posts.

18. **LangChain for Advanced Memory**:
   - IndieI uses LangChain to give the bot enhanced memory capabilities, ensuring a more personalized and continuous experience across multiple sessions

### Future Upgrades

IndieI has an ambitious roadmap, with several exciting upgrades planned for future releases:

1. **OpenAI API Integration**:
   - IndieI will be integrated with the OpenAI API, allowing access to a broader range of AI models such as GPT-4 and beyond.
   - This will enhance the bot’s ability to generate creative and high-quality content, perform more complex reasoning tasks, and provide even more detailed and nuanced responses.

2. **Multi-Platform Social Media Support**:
   - In addition to LinkedIn, future upgrades will include support for other social media platforms like Twitter, Instagram, and Facebook, enabling users to automate posts, fetch profiles, and manage content across multiple channels.

3. **Voice Interaction Support**:
   - IndieI will be enhanced with voice interaction capabilities, allowing users to communicate with the bot via voice commands, improving accessibility and providing a more natural conversation experience.

4. **Task Scheduling and Workflow Automation**:
   - Users will be able to schedule and automate tasks across a wider array of platforms, enabling the bot to handle repetitive actions like checking emails, setting reminders, and managing calendar events.

5. **Advanced Data Visualization**:
   - Future versions will include enhanced data visualization features, allowing users to view graphs, charts, and dashboards for various data points, including web scraping results, network traffic, and more.

6. **Custom AI Model Training**:
   - IndieI will support user-specific AI model training, enabling individuals or businesses to train the bot on proprietary data for more specialized and accurate responses tailored to specific industries or use cases.

---

With these future upgrades, IndieI aims to become a truly comprehensive AI assistant, capable of automating tasks, generating content, and providing insightful responses across a multitude of platforms. The integration with OpenAI APIs and other cutting-edge technologies will ensure that IndieI remains at the forefront of AI advancements, offering users a continuously evolving and highly intelligent assistant.

---

   ### Conclusion

IndieI is an innovative AI-powered assistant that brings together cutting-edge technologies such as FastAPI, React, and advanced language models like LLaMA to provide seamless user interactions and task automation. With features like web scraping, LinkedIn integration, file uploads, real-time communication, and intelligent memory handling, IndieI is designed to simplify and enhance workflows across various domains. Whether it's automating social media management, extracting web data, or interacting in real-time, IndieI is a versatile tool built to assist users in accomplishing tasks more efficiently.

The project continues to evolve, with exciting new capabilities like network packet analysis and advanced LinkedIn post scheduling, making IndieI a powerful AI helper for personal and professional use. By integrating memory and context handling through LangChain and advanced pattern matching for search accuracy, IndieI offers a personalized, user-friendly experience that grows with each interaction.






