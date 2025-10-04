# Nimbus Submission Guide: Running Node.js MongoDB Projects

This guide explains how to set up and run your Node.js MongoDB experiments on Nimbus, step by step. Follow these instructions for each project.

---

## 1. Clone the Project

Open Nimbus and start a terminal. Run:
```bash
git clone https://github.com/HarshJain69/Mongodb_exp5_FullStack.git
```

## 2. Enter the Project Folder
```bash
cd Mongodb_exp5_FullStack
```

## 3. Install Dependencies
```bash
npm install
```

## 4. Create the `.env` File
- In the project folder, create a file named `.env`
- Add your MongoDB connection string and any other required variables. Example:
  ```env
  MONGO_URI=mongodb+srv://yourusername:yourpassword@cluster0.mongodb.net/?retryWrites=true&w=majority
  PORT=3000
  ```

## 5. Start the Server
```bash
npm start
```

## 6. Run Experiment Scripts in a New Terminal
Open a second terminal in Nimbus and run:
- For Experiment 5:
  ```bash
  node crudScript.js
  ```
- For Experiment 6:
  ```bash
  node catalogDemo.js
  ```
- For Student Management (Experiment 5.2):
  ```bash
  node studentCrudScript.js
  ```

## 7. View Your Database
- Use MongoDB Compass or MongoDB Atlas web interface
- Log in and view your cluster, databases, and collections
- You will see the data created by your scripts

---

## Repeat for All Projects
Follow the same steps for each Node.js MongoDB project you want to submit on Nimbus.

**You are ready for Nimbus submission!**
