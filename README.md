# Streaming Overseer Deployment Instructions

**Streaming Overseer** is a tool designed to monitor specified Telegram channels for messages containing certain keywords and automatically forward them to your private channel. It has a user-friendly graphical interface, and it allows to manage multiple monitoring sessions simultaneously, making it easier to automate keeping track of relevant messages across various channels.

---
## Prerequisites
Before you begin, please ensure you have the following installed on your computer:
1. **Git**: A tool used to download the application files.
   - **Download Link**: [Git Download](https://git-scm.com/downloads)
   - **Installation Instructions**: Follow the prompts in the installer.
2. **Docker Desktop**: Software that allows you to run applications in containers without complex setup.
   - **Download Link**: [Docker Desktop Download](https://www.docker.com/products/docker-desktop)
   - **Installation Instructions**: Choose the version for your operating system (Windows or macOS) and follow the installation steps.
---
## Deployment Steps
### **Download the Application Files first**
#### **Option A: Using the Command Line (Recommended)**:
1. **Open the Command Prompt or Terminal:**
   - **Windows:**
      - Click the **Start** button.
      - Type `cmd` and press **Enter**.
   - **Mac:**
      - Open **Finder**.
      - Go to **Applications** > **Utilities**.
      - Double-click on **Terminal**.
2. **Navigate to Your Desired Folder**:\
Decide where you want to store the application (e.g., Desktop or Documents).
    - In the command prompt, type: `cd Desktop` *Replace Desktop with your chosen folder if different.*
3. **Download the Application Files:**
    - Type the following command and press **Enter**: `git clone https://github.com/afolivieri/streaming-overseer-docker` *This command downloads the application files into a folder named `streaming-overseer-docker`*
    - `cd streaming-overseer-docker`
4. **Navigate to the Application Folder:**
   - Enter the following command `cd streaming-overseer-docker`
#### **Option B: Downloading the ZIP File (Alternative)**
1. **Visit the Application Repository:**
   - Open your web browser and go to [https://github.com/afolivieri/streaming-overseer-docker](https://github.com/afolivieri/streaming-overseer-docker)
2. **Download the ZIP File:**
   - Click on the green **Code** button
   - Select **Download ZIP**
   - Once downloaded, locate the ZIP file (usually in your Downloads folder)
3. **Extract the ZIP File:**
   - Right-click on the ZIP file and select **Extract All** (Windows) or **Open With** > **Archive Utility** (Mac).
   - Choose a destination folder and extract the files
   - The extracted folder will be named `streaming-overseer-docker-main`. You can rename it to `streaming-overseer-docker` for consistency
---
### **Start the Application**
#### **First Start of the Application**
1. **Open Docker Desktop:**
   - Find Docker Desktop in your applications or programs and open it
   - Wait a few moments for Docker to initialize
2. **Ensure Docker Desktop is Running:**
   - Docker must be running in the background for the application to work
3. **Start the Application Using Command Line:**
   - **Note:** You need to perform this step even if you used Option B above
   - **In the Command Prompt or Terminal**, navigate to the application folder if you're not already there using `cd streaming-overseer-docker`
   - Start the application by typing `docker-compose up`
   - Press **Enter**
   - This command tells Docker to set up and start the application
   - The first time you run this, it may take several minutes as Docker downloads necessary components
   - **Keep this window open** while the application is running
#### **Starting the Application in the Future**
After the initial setup, you can start the application more quickly:
- Navigate to the application folder if needed with `cd streaming-overseer-docker`
- Start the application by typing `docker-compose start`
- Press **Enter**.
- This command starts the application without rebuilding it
---
### **Access the Application in Your Browser**
1. **Open Your Web Browser:**
   - Use any modern browser like **Chrome**, **Firefox**, **Edge**, or **Safari**
2. **Access the Frontend (User Interface):**
   - In the address bar, type `http://localhost:3000`
   - Press **Enter**
   - You should see the **Streaming Overseer** application interface\
   **Important Note:**
   - **Use `http://localhost:3000` exactly**
   - **Do not use `http://127.0.0.1:3000` or any other variation**, as the application is set up to work only with `localhost`
3. **Access the Backend (API) [Optional]:**
   - For advanced users or developers, the backend API is available at `http://localhost:8000`
---
## **Detailed Instructions for the use of the application**
Within the application interface, look for an **Instructions** button located in the **top right corner** of the application. Click on it to access a comprehensive user guide.

---
