# FabFits-AI-AR-Fashion-Website
FabFits is a pioneering e-commerce platform designed to redefine the fashion shopping experience. Seamlessly blending modern technology with the latest trends, FabFits offers a dynamic and personalized journey for fashion enthusiasts. From cutting-edge AI features like voice and image search to immersive augmented reality try-ons.

Running a MERN (MongoDB, Express.js, React, Node.js) project in Visual Studio Code (VS Code) involves setting up the environment, installing necessary dependencies, and using appropriate commands to run both the backend (Node.js/Express) and frontend (React) parts of the application. Here are the steps to run a MERN project in VS Code:

### Prerequisites
1. **Node.js** and **npm** installed on your system.
2. **MongoDB** installed and running on your local machine or a cloud-based MongoDB instance (like MongoDB Atlas).

### Steps

1. **Open VS Code:**
   - Launch Visual Studio Code.

2. **Open the Project Folder:**
   - Open your MERN project folder in VS Code. You can do this by selecting `File > Open Folder` and navigating to your project directory.

3. **Install Backend Dependencies:**
   - Open the terminal in VS Code (`View > Terminal` or `Ctrl + `) and navigate to your backend directory (usually the root directory of your project).
   - Run the following command to install the backend dependencies specified in `package.json`:
     ```bash
     npm install
     ```

4. **Install Frontend Dependencies:**
   - Navigate to your frontend directory (usually a subdirectory like `client` or `frontend`).
   - Run the following command to install the frontend dependencies specified in `package.json`:
     ```bash
     npm install
     ```

5. **Set Up Environment Variables:**
   - Create a `.env` file in your backend directory and add any necessary environment variables (e.g., database connection strings, API keys). For example:
     ```
     PORT=5000
     MONGO_URI=mongodb://localhost:27017/yourdbname
     ```

6. **Start the MongoDB Server:**
   - If you are running MongoDB locally, make sure the MongoDB server is started. You can start it from the terminal:
     ```bash
     mongod
     ```
   - If you are using a cloud-based MongoDB instance, ensure your connection string in the `.env` file is correct.

7. **Run the Backend Server:**
   - In the terminal, navigate to the backend directory and run:
     ```bash
     npm start
     ```
   - Alternatively, if you have a development script in `package.json` (like `nodemon` for auto-reloading), you can run:
     ```bash
     npm run dev
     ```

8. **Run the Frontend Development Server:**
   - In the terminal, navigate to the frontend directory and run:
     ```bash
     npm start
     ```
   - This will start the React development server, and the application should open in your default web browser, typically at `http://localhost:3000`.

### Example Project Structure
Here is an example of a typical MERN project structure:

```
my-mern-project/
├── backend/
│   ├── node_modules/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── .env
│   ├── package.json
│   └── server.js
└── frontend/
    ├── node_modules/
    ├── public/
    ├── src/
    ├── .env
    ├── package.json
    └── README.md
```

### Additional Tips
- **Debugging:** You can set up breakpoints and debug your code in VS Code. Configure the debugger by creating a `.vscode/launch.json` file.
- **Linting and Formatting:** Use extensions like ESLint and Prettier for code linting and formatting.
- **Git Integration:** VS Code has built-in Git support for version control.

By following these steps, you should be able to run and manage your MERN project effectively in Visual Studio Code.
