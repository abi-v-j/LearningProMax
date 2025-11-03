# 🚀 Node Express API Beginner's Full Guide - Step by Step

A complete step-by-step tutorial to set up Node.js with Express, add middleware like CORS and body-parser, and build simple APIs (no database required).

---

## 📚 Table of Contents

- [🧩 Phase 1: Prerequisites & Setup](#-phase-1-prerequisites--setup)
- [🧩 Phase 2: Clean Up and Create Basic Hello World API](#-phase-2-clean-up-and-create-basic-hello-world-api)
- [🧩 Phase 3: Add Middleware (body-parser & CORS)](#-phase-3-add-middleware-body-parser--cors)
- [🧩 Phase 4: Build Essential API Routes](#-phase-4-build-essential-api-routes)
- [🧩 Phase 5: Advanced API Examples & Testing](#-phase-5-advanced-api-examples--testing)

---

## 🧩 **Phase 1: Prerequisites & Setup**

---

### **Step 1: Install Node.js and npm**

### **1.1 Visit the Official Website**
1. **Open your browser** and go to:
   
    🔗 https://nodejs.org/en/download
   
---

### **1.2 Download Links (Clickable)**
**Choose your operating system:**
- 🪟 **Windows:** [Windows Installer (.msi)](https://nodejs.org/dist/v18.17.0/node-v18.17.0-x64.msi)
- 🍎 **macOS:** [macOS Installer (.pkg)](https://nodejs.org/dist/v18.17.0/node-v18.17.0.pkg)
- 🐧 **Linux:** [Linux Binaries](https://nodejs.org/dist/v18.17.0/node-v18.17.0-linux-x64.tar.xz)

---

### **1.3 Verify Installation**
```bash
# Check Node.js version
node --version
# Check npm version
npm --version
```

---

### **1.4 Alternative Installation Methods**
- 🔗 **Node Version Manager (nvm):** https://github.com/nvm-sh/nvm
- 🔗 **Package Managers:** https://nodejs.org/en/download/package-manager

---

### **1.5 Useful Resources**
- 🔗 [Node.js Documentation](https://nodejs.org/en/docs/)
- 🔗 [npm Documentation](https://docs.npmjs.com/)
- 🔗 [Troubleshooting Guide](https://nodejs.org/en/docs/guides/troubleshooting/)

---

### **1.6 Installation Complete ✅**
You should now see version numbers for both Node.js and npm.  
Your development environment is ready for Express APIs!

---

### **Step 2: Open Terminal / Command Prompt**

### **2.1 For Windows**
- Press `Windows Key + R`
- Type `cmd`
- Press `Enter`

### **2.2 For macOS**
- Press `Command + Space`
- Type `terminal`
- Press `Enter`

### **2.3 For Linux**
- Press `Ctrl + Alt + T`

---

### **Step 3: Create Project Structure**

### **3.1 Create the Main Project Folder**
- Create a new folder called `SimpleAPI` — this will be your main project container.

### **3.2 Enter the Main Folder**
- Open the `SimpleAPI` folder.  
   
    You should now be inside `SimpleAPI`.
   
---

### **Step 4: Open Project in VS Code**

### **4.1 Open VS Code**
- Click the VS Code icon or open via:
    - `Windows Key` → type **Visual Studio Code** → `Enter`
    - `Command + Space` (Mac) → type **Visual Studio Code** → `Enter`

---

### **4.2 Open Folder in VS Code**
**Method 1: File Menu**  
1. Click `File` → `Open Folder...`  
2. Navigate to `SimpleAPI`  
3. Click **Select Folder**  

**Method 2: Drag and Drop**  
1. Open File Explorer/Finder  
2. Drag the `SimpleAPI` folder into VS Code  

**Method 3: Command Line**  
```bash
cd SimpleAPI
```

---

### **Step 5: Initialize Node Project**

### **5.1 Open Terminal in VS Code**
**Method 1:** Press `Ctrl + `` (backtick key above Tab)`  
**Method 2:** Click `Terminal` → `New Terminal`

---

### **5.2 Verify Terminal Location**
Make sure you’re in the correct folder. You should see:  
```
PS C:\YourPath\SimpleAPI>
```
or  
```
/your/path/SimpleAPI $
```
If not, navigate manually:  
```bash
cd SimpleAPI
```

---

### **5.3 Initialize npm Project**
```bash
npm init -y
```
This creates a `package.json` file.

---

### **5.4 Install Express**
```bash
npm install express
```

---

### **5.5 Verify Installation**
Check your project structure:  
```
📁 SimpleAPI
  📁 node_modules
  📄 package-lock.json
  📄 package.json
```

---

### **5.6 Success Confirmation 🎉**
Your Express project is initialized!  
**You have:**  
- ✅ Node.js and npm ready  
- ✅ Empty Express project  
- ✅ Ready to code APIs!

---

### **5.7 Stop / Restart (If Needed)**
No server running yet — we'll start one next!  
✅ **Next Step:** Build your first server 🚀

---

## 🧩 **Phase 2: Clean Up and Create Basic Hello World API**

---

## **Step 1: Create Basic Server File**

### **1.1 Create server.js**
- **In VS Code**, right-click in the left sidebar  
- **Select** `New File`  
- **Name it** `server.js`  
- **Save** (`Ctrl + S`)

### **1.2 Add Basic Express Code**
**In `server.js`, type this code:**  
```javascript
const express = require('express');
const app = express();
const PORT = 3000;

app.get('/', (req, res) => {
  res.send('Hello World from Express!');
});

app.listen(PORT, () => {
  console.log(`Server running on http://localhost:${PORT}`);
});
```
**Save the file** (`Ctrl + S`)

---

## **Step 2: Verify File Structure**
**Your project should now look like this:**  
```
📁 SimpleAPI
  📁 node_modules
  📄 package.json
  📄 package-lock.json
  📄 server.js
```

---

## **Step 3: Start Development Server**

### **3.1 Run the Server**
In your terminal:  
```bash
node server.js
```
Output example:  
```
Server running on http://localhost:3000
```

---

### **3.2 Open Your Browser**
- Go to: [http://localhost:3000](http://localhost:3000)  
- Or copy and paste into your browser

---

### **3.3 Verify Successful Setup**
You should see:  
```
Hello World from Express!
```

---

### **3.4 Test Live Updates**

### **3.4.1 Make a Change**
- **In `server.js`**, change the message:  
```javascript
app.get('/', (req, res) => {
  res.send('Hello from my first API server!');
});
```

### **3.4.2 Restart and Check**
- **Stop server** (`Ctrl + C`)  
- **Restart** (`node server.js`)  
- **Check browser** — it should show the new message!

---

## **Step 4: Final Verification**
**Your basic server.js should look like this:**  
```javascript
const express = require('express');
const app = express();
const PORT = 3000;

app.get('/', (req, res) => {
  res.json({ message: 'Hello World API!' });
});

app.listen(PORT, () => {
  console.log(`Server running on http://localhost:${PORT}`);
});
```
**Test in browser:** Refresh [http://localhost:3000](http://localhost:3000) — you should see JSON: `{"message":"Hello World API!"}`

---

## **Success! 🎉**
**You now have:**  
- ✅ Basic Express server  
- ✅ Simple GET route  
- ✅ JSON response  
**Next:** Add middleware for real-world APIs!

---

## 🧩 **Phase 3: Add Middleware (body-parser & CORS)**

---

## **Step 1: Install Middleware Packages**

### **1.1 Stop Server First**
`Ctrl + C`

---

### **1.2 Install body-parser and cors**
```bash
npm install body-parser cors
```
- **body-parser:** Parses incoming request bodies (e.g., JSON from POST requests)  
- **cors:** Enables cross-origin requests (for frontend-backend communication)

---

## **Step 2: Update server.js with Middleware**

### **2.1 Require and Use Middleware**
**Replace `server.js` content:**  
```javascript
const express = require('express');
const bodyParser = require('body-parser');
const cors = require('cors');
const app = express();
const PORT = 3000;

// Middleware
app.use(bodyParser.json()); // Parse JSON bodies
app.use(cors()); // Enable CORS for all routes

app.get('/', (req, res) => {
  res.json({ message: 'Hello World with Middleware!' });
});

app.listen(PORT, () => {
  console.log(`Server running on http://localhost:${PORT}`);
});
```
**Save** (`Ctrl + S`)

---

## **Step 3: Add a Simple POST Route for Testing**

### **3.1 Add POST Endpoint**
**Add this before `app.listen`:**  
```javascript
app.post('/echo', (req, res) => {
  const { message } = req.body;
  res.json({ echoed: message || 'No message received' });
});
```
**Full server.js now:**  
```javascript
const express = require('express');
const bodyParser = require('body-parser');
const cors = require('cors');
const app = express();
const PORT = 3000;

app.use(bodyParser.json());
app.use(cors());

app.get('/', (req, res) => {
  res.json({ message: 'Hello World with Middleware!' });
});

app.post('/echo', (req, res) => {
  const { message } = req.body;
  res.json({ echoed: message || 'No message received' });
});

app.listen(PORT, () => {
  console.log(`Server running on http://localhost:${PORT}`);
});
```

---

## **Step 4: Test Middleware**

### **4.1 Restart Server**
```bash
node server.js
```

---

### **4.2 Test GET in Browser**
- Visit [http://localhost:3000](http://localhost:3000)  
- Should see: `{"message":"Hello World with Middleware!"}`  
✅ **CORS is working** (no browser errors if testing from another origin later)

---

### **4.3 Test POST with curl (or Postman)**
In a **new terminal** (keep server running):  
```bash
curl -X POST http://localhost:3000/echo \
  -H "Content-Type: application/json" \
  -d '{"message": "Test from curl!"}'
```
Expected output:  
```
{"echoed":"Test from curl!"}
```
✅ **body-parser is working** — JSON body parsed successfully!  
If no curl: Use [Postman](https://www.postman.com/downloads/) or browser dev tools.

---

## **Step 5: Verify Project Structure**
```
📁 SimpleAPI
  📁 node_modules
  📄 package.json
  📄 package-lock.json
  📄 server.js
```

---

## **Success! 🎉**
**You now have:**  
- ✅ Express with body-parser (JSON parsing)  
- ✅ CORS enabled (cross-origin safe)  
- ✅ GET and POST routes working  
**Next:** Build more API routes!

---

## 🧩 **Phase 4: Build Essential API Routes**

---

## **Step 1: Create Routes for CRUD-like Operations (No DB)**

### **1.1 Stop Server**
`Ctrl + C`

---

### **1.2 Update server.js with Routes**
**Replace routes section:**  
```javascript
// In-memory "database" (array for demo)
let todos = [
  { id: 1, task: 'Learn Express', completed: false },
  { id: 2, task: 'Build API', completed: true }
];

// GET all todos
app.get('/todos', (req, res) => {
  res.json(todos);
});

// GET single todo by ID
app.get('/todos/:id', (req, res) => {
  const id = parseInt(req.params.id);
  const todo = todos.find(t => t.id === id);
  if (todo) {
    res.json(todo);
  } else {
    res.status(404).json({ error: 'Todo not found' });
  }
});

// POST new todo
app.post('/todos', (req, res) => {
  const { task } = req.body;
  if (!task) {
    return res.status(400).json({ error: 'Task required' });
  }
  const newTodo = {
    id: todos.length + 1,
    task,
    completed: false
  };
  todos.push(newTodo);
  res.status(201).json(newTodo);
});

// PUT update todo
app.put('/todos/:id', (req, res) => {
  const id = parseInt(req.params.id);
  const { task, completed } = req.body;
  const todoIndex = todos.findIndex(t => t.id === id);
  if (todoIndex === -1) {
    return res.status(404).json({ error: 'Todo not found' });
  }
  todos[todoIndex] = { ...todos[todoIndex], task, completed };
  res.json(todos[todoIndex]);
});

// DELETE todo
app.delete('/todos/:id', (req, res) => {
  const id = parseInt(req.params.id);
  const todoIndex = todos.findIndex(t => t.id === id);
  if (todoIndex === -1) {
    return res.status(404).json({ error: 'Todo not found' });
  }
  todos.splice(todoIndex, 1);
  res.json({ message: 'Todo deleted' });
});
```
**Full server.js:**  
```javascript
const express = require('express');
const bodyParser = require('body-parser');
const cors = require('cors');
const app = express();
const PORT = 3000;

app.use(bodyParser.json());
app.use(cors());

let todos = [
  { id: 1, task: 'Learn Express', completed: false },
  { id: 2, task: 'Build API', completed: true }
];

app.get('/', (req, res) => {
  res.json({ message: 'Todo API Ready!' });
});

app.get('/todos', (req, res) => {
  res.json(todos);
});

app.get('/todos/:id', (req, res) => {
  const id = parseInt(req.params.id);
  const todo = todos.find(t => t.id === id);
  if (todo) {
    res.json(todo);
  } else {
    res.status(404).json({ error: 'Todo not found' });
  }
});

app.post('/todos', (req, res) => {
  const { task } = req.body;
  if (!task) {
    return res.status(400).json({ error: 'Task required' });
  }
  const newTodo = {
    id: todos.length + 1,
    task,
    completed: false
  };
  todos.push(newTodo);
  res.status(201).json(newTodo);
});

app.put('/todos/:id', (req, res) => {
  const id = parseInt(req.params.id);
  const { task, completed } = req.body;
  const todoIndex = todos.findIndex(t => t.id === id);
  if (todoIndex === -1) {
    return res.status(404).json({ error: 'Todo not found' });
  }
  todos[todoIndex] = { ...todos[todoIndex], task, completed };
  res.json(todos[todoIndex]);
});

app.delete('/todos/:id', (req, res) => {
  const id = parseInt(req.params.id);
  const todoIndex = todos.findIndex(t => t.id === id);
  if (todoIndex === -1) {
    return res.status(404).json({ error: 'Todo not found' });
  }
  todos.splice(todoIndex, 1);
  res.json({ message: 'Todo deleted' });
});

app.listen(PORT, () => {
  console.log(`Server running on http://localhost:${PORT}`);
});
```
**Save** (`Ctrl + S`)

---

## **Step 2: Restart and Test Routes**

### **2.1 Start Server**
```bash
node server.js
```

---

### **2.2 Test GET All**
- Browser: [http://localhost:3000/todos](http://localhost:3000/todos)  
- Expected: JSON array with 2 todos

---

### **2.3 Test GET Single**
- Browser: [http://localhost:3000/todos/1](http://localhost:3000/todos/1)  
- Expected: `{"id":1,"task":"Learn Express","completed":false}`  
- Try invalid ID: `/todos/999` → `{"error":"Todo not found"}`

---

### **2.4 Test POST**
```bash
curl -X POST http://localhost:3000/todos \
  -H "Content-Type: application/json" \
  -d '{"task": "Test POST"}'
```
Expected: `{"id":3,"task":"Test POST","completed":false}`  
Refresh `/todos` — new item added!

---

### **2.5 Test PUT**
```bash
curl -X PUT http://localhost:3000/todos/3 \
  -H "Content-Type: application/json" \
  -d '{"completed": true}'
```
Expected: Updated todo JSON

---

### **2.6 Test DELETE**
```bash
curl -X DELETE http://localhost:3000/todos/3
```
Expected: `{"message":"Todo deleted"}`  
Refresh `/todos` — item gone!

---

## **Success! 🎉**
**You now have:**  
- ✅ Full CRUD API (in-memory)  
- ✅ Error handling (404, 400)  
- ✅ JSON responses  
**Next:** Advanced examples and tools!

---

## 🧩 **Phase 5: Advanced API Examples & Testing**

---

## **Step 1: Add Query Params & Validation**

### **1.1 Stop Server**
`Ctrl + C`

---

### **1.2 Update server.js with Advanced Features**
**Add these routes before `app.listen`:**  
```javascript
// GET todos with query params (e.g., ?completed=true)
app.get('/todos/filter', (req, res) => {
  const { completed } = req.query;
  const filtered = todos.filter(t => completed === undefined || t.completed === (completed === 'true'));
  res.json(filtered);
});

// Middleware for logging requests
app.use((req, res, next) => {
  console.log(`${req.method} ${req.path} - ${new Date().toISOString()}`);
  next();
});

// Error handling middleware (add at end, before listen)
app.use((err, req, res, next) => {
  console.error(err.stack);
  res.status(500).json({ error: 'Something went wrong!' });
});
```
**Also update POST for better validation:**  
```javascript
app.post('/todos', (req, res) => {
  const { task } = req.body;
  if (!task || typeof task !== 'string' || task.trim().length < 3) {
    return res.status(400).json({ error: 'Task must be a string with at least 3 characters' });
  }
  const newTodo = {
    id: Math.max(...todos.map(t => t.id)) + 1, // Better ID generation
    task: task.trim(),
    completed: false
  };
  todos.push(newTodo);
  res.status(201).json(newTodo);
});
```
**Save** (`Ctrl + S`)

---

## **Step 2: Install Nodemon for Auto-Restart**

### **2.1 Install Dev Dependency**
```bash
npm install --save-dev nodemon
```

### **2.2 Update package.json Scripts**
**Open `package.json`, add under `"scripts"`:**
```json
{
  "scripts": {
    "start": "node server.js",
    "dev": "nodemon server.js"
  }
}
```
**Save** (`Ctrl + S`)

---

## **Step 3: Test Advanced Features**

### **3.1 Start with Nodemon**
```bash
npm run dev
```
Now changes auto-restart the server!

---

### **3.2 Test Query Params**
- Browser: [http://localhost:3000/todos/filter?completed=true](http://localhost:3000/todos/filter?completed=true)  
- Expected: Only completed todos  
- Check terminal: Logs show requests!

---

### **3.3 Test Validation**
```bash
curl -X POST http://localhost:3000/todos \
  -H "Content-Type: application/json" \
  -d '{"task": "a"}'  # Too short
```
Expected: `{"error":"Task must be a string with at least 3 characters"}`

---

## **Step 4: Create a New API Project (User API)**

### **4.1 Create New Folder**
```bash
cd ..
mkdir UserAPI
cd UserAPI
npm init -y
npm install express body-parser cors
npm install --save-dev nodemon
```

### **4.2 Copy & Adapt server.js**
Create `server.js` with user-focused routes:  
```javascript
const express = require('express');
const bodyParser = require('body-parser');
const cors = require('cors');
const app = express();
const PORT = 3001;

app.use(bodyParser.json());
app.use(cors());

let users = [
  { id: 1, name: 'Alice', email: 'alice@example.com', age: 28 },
  { id: 2, name: 'Bob', email: 'bob@example.com', age: 32 }
];

app.get('/', (req, res) => {
  res.json({ message: 'User API Ready!' });
});

app.get('/users', (req, res) => {
  res.json(users);
});

app.get('/users/:id', (req, res) => {
  const id = parseInt(req.params.id);
  const user = users.find(u => u.id === id);
  if (user) res.json(user);
  else res.status(404).json({ error: 'User not found' });
});

app.post('/users', (req, res) => {
  const { name, email, age } = req.body;
  if (!name || !email || age < 0) {
    return res.status(400).json({ error: 'Invalid data' });
  }
  const newUser = { id: users.length + 1, name, email, age };
  users.push(newUser);
  res.status(201).json(newUser);
});

app.listen(PORT, () => {
  console.log(`User API on http://localhost:${PORT}`);
});
```
Update `package.json` scripts as before.

---

### **4.3 Run and Test**
```bash
npm run dev
```
- GET: [http://localhost:3001/users](http://localhost:3001/users)  
- POST example:  
```bash
curl -X POST http://localhost:3001/users \
  -H "Content-Type: application/json" \
  -d '{"name": "Charlie", "email": "charlie@example.com", "age": 25}'
```

---

## **Step 5: Essential Testing Tools**

### **5.1 Browser for GET**
Use browser for simple GET requests.

### **5.2 curl for All Methods**
- GET: `curl http://localhost:3000/todos`  
- POST/PUT/DELETE: As shown above.

### **5.3 Postman (Recommended)**
- 🔗 [Download Postman](https://www.postman.com/downloads/)  
- Create collections for your APIs  
- Test with GUI: Headers, body, auth (future-proof)

### **5.4 VS Code Extensions**
- Install: "Thunder Client" for API testing inside VS Code

---

## **Navigation & Multi-Project Tips**
To run multiple servers:  
- Use different ports (e.g., 3000, 3001)  
- `npm run dev` in separate terminals  
**Pro Tip:** Add `.env` file later for ports/secrets (install `dotenv`).

---

## **✅ Phase 5 Complete!**

### **🎯 What You've Learned:**
**Essential Express API Skills:**  
1. **Basic Server Setup** - Express app, routes, JSON responses  
2. **Middleware Mastery** - body-parser for bodies, CORS for cross-origin  
3. **CRUD Routes** - GET/POST/PUT/DELETE with params/queries  
4. **Error Handling** - Status codes, validation  
5. **Dev Tools** - Nodemon, curl, Postman  

### **🚀 Key Benefits:**
- ✅ **Fast APIs** - Lightweight, no DB needed for prototypes  
- ✅ **Secure Basics** - CORS prevents issues  
- ✅ **Scalable** - Easy to add DB later (e.g., MongoDB)  
- ✅ **Testable** - Quick verification with tools  
- ✅ **Real-World Ready** - In-memory data for learning  

### **💡 Pro Tips:**
- Always use `bodyParser.json()` for POST/PUT  
- Enable CORS early for frontend integration  
- Log requests for debugging  
- Validate inputs to avoid errors  
- Use Nodemon for dev: `npm run dev`  

**Run `npm run dev` and test your APIs — you're now an Express pro! 🚀**