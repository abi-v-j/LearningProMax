

# 🚀 React Beginner's Full Guide with Vite - Step by Step

A complete step-by-step tutorial to set up React using Vite, build simple apps, and master React props.

---


## 📚 Table of Contents
- [🧩 Phase 1: Prerequisites & Setup](#-phase-1-prerequisites--setup)
- [🧩 Phase 2: Clean Up and Create Hello World](#-phase-2-clean-up-and-create-hello-world)
- [🧩 Phase 3: Create Another React App (Counter App)](#-phase-3-create-another-react-app-counter-app)
- [🧩 Phase 4: React Props Mastery](#-phase-4-react-props-mastery)
- [🧩 Phase 5: Essential React Hooks Mastery](#-phase-5-essential-react-hooks-mastery)

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

Your development environment is ready for React!

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

- Create a new folder called `ToDo` — this will be your main project container.

### **3.2 Enter the Main Folder**

- Open the `ToDo` folder.

### **3.3 Create the Client Folder**

- Inside the `ToDo` folder, create another new folder called `client`.
    
    This `client` folder will hold your React application.
    

### **3.4 Enter the Client Folder**

- Open the `client` folder you just created.
    
    You should now be inside `ToDo/client`.
    

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
2. Navigate to `ToDo/client`
3. Click **Select Folder**

**Method 2: Drag and Drop**

1. Open File Explorer/Finder
2. Drag the `client` folder into VS Code

**Method 3: Command Line**

```bash
cd ToDo/client

```

---

### **Step 5: Create React App with Vite**

### **5.1 Open Terminal in VS Code**

**Method 1:** Press `Ctrl + `` (backtick key above Tab)`

**Method 2:** Click `Terminal` → `New Terminal`

---

### **5.2 Verify Terminal Location**

Make sure you’re in the correct folder. You should see:

```
PS C:\YourPath\ToDo\client>

```

or

```
/your/path/ToDo/client $

```

If not, navigate manually:

```bash
cd ToDo/client

```

---

### **5.3 Run Vite Creation Command**

```bash
npm create vite@latest

```

You’ll see:

```
✔ Project name: 

```

---

### **5.4 Enter Project Name**

- Type: <space> <.(dot)> Eg: .
- Press `Enter`

---

### **5.5 Select Framework**

- Choose `React`
- Press `Enter`

---

### **5.6 Select Package**

- Press`tab`
- Press `Enter`

---

### **5.7 Select Variant**

- Choose `JavaScript`
- Press `Enter`

---

### **5.8 Wait for Project Creation**

Output:

```
Scaffolding project in /path/to/my-first-react-app...
Done. Now run:
  cd my-first-react-app
  npm install
  npm run dev

```

---

### **5.9 Install Dependencies**

```bash
npm install

```

---

### **5.10 Start Development Server**

```bash
npm run dev

```

Output example:

```
VITE v4.4.9  ready in 320 ms
➜  Local:   http://localhost:5173/

```

---

### **5.11 Open Your Browser**

- Click: [http://localhost:5173](http://localhost:5173/)
- Or copy and paste into your browser

---

### **5.12 Verify Successful Setup**

You should see:

```
Vite + React
count is 0
Edit src/App.jsx and save to test HMR

```

---

### **5.13 Success Confirmation 🎉**

Your React app is now running!

**You have:**

- ✅ React development environment
- ✅ Local development server
- ✅ Ready to code!

---

### **5.14 Stop / Restart the Server**

To stop:

```bash
Ctrl + C

```

✅ **Next Step:** Start learning React components and JSX 🚀

## 🧩 **Phase 2: Clean Up and Create Hello World**


## **Step 1: Clean Up Files**

### **1.1 Clear App.jsx Content**

- **Open** `src/App.jsx` in VS Code
- **Select all** code (`Ctrl + A`)
- **Delete everything** (`Delete` key)
- **Save** the file (`Ctrl + S`)

### **1.2 Clear main.jsx Content**

- **Open** `src/main.jsx` in VS Code
- **Select all** code (`Ctrl + A`)
- **Delete everything** (`Delete` key)
- **Save** the file (`Ctrl + S`)

### **1.3 Delete CSS Files**

- **Right-click** on `src/App.css` in left sidebar
- **Select** `Delete`
- **Confirm** deletion
- **Right-click** on `src/index.css` in left sidebar
- **Select** `Delete`
- **Confirm** deletion

### **1.4 Delete Asset Images**

- **Expand** `src/assets` folder
- **Right-click** on `react.svg`
- **Select** `Delete`
- **Confirm** deletion

### **1.5 Delete Public Images**

- **Expand** `public` folder
- **Right-click** on `vite.svg`
- **Select** `Delete`
- **Confirm** deletion

## **Step 2: Create Clean Hello World**

### **2.1 Create New App.jsx**

**In `src/App.jsx`, type this code:**

```jsx
import React from 'react'

const App = () => {
  return (
    <div>Hello World</div>
  )
}

export default App
```

**Save the file** (`Ctrl + S`)

### **2.2 Create New main.jsx**

**In `src/main.jsx`, type this code:**

```jsx
import { createRoot } from 'react-dom/client'
import App from './App.jsx'

createRoot(document.getElementById('root')).render(
    <App />
)

```

**Save the file** (`Ctrl + S`)

## **Step 3: Verify File Structure**

**Your project should now look like this:**

text

```
📁 client
  📁 node_modules
  📁 public
  📁 src
    📄 App.jsx
    📄 main.jsx
  📄 .gitignore
  📄 index.html
  📄 package-lock.json
  📄 package.json
  📄 vite.config.js
```

## **Step 4: Check Browser Result**

**Look at your browser at `http://localhost:5173`**

- You should see only: **"Hello World!"**
- And: **"My first clean React app"**
- No more logos, counters, or default Vite content

## **Step 5: Test Live Updates**

### **5.1 Make a Change**

- **In `src/App.jsx`**, change the text:

```jsx
import React from 'react'

const App = () => {
  return (
    <div>Hello World</div>
    <p>Welcome to my clean React setup</p>
      <button>Test Button</button>
  )
}

export default App
```

### **5.2 Save and Check**

- **Save** the file (`Ctrl + S`)
- **Check browser** - it should instantly show the button!

## **Step 6: Final Verification**

**Your clean App.jsx should look like this:**

```jsx
import React, { useState } from "react";

export default function App() {
  const [todos, setTodos] = useState([]);
  const [text, setText] = useState("");

  const addTodo = () => {
    if (text.trim() === "") return;
    setTodos([...todos, text]);
    setText("");
  };

  const removeTodo = (index) => {
    setTodos(todos.filter((_, i) => i !== index));
  };

  const editTodo = (index) => {
    const newText = prompt("Edit todo", todos[index]);
    if (newText !== null && newText.trim() !== "") {
      const updated = [...todos];
      updated[index] = newText;
      setTodos(updated);
    }
  };

  return (
    <div>
      <h1>Todo App</h1>
      <input
        value={text}
        onChange={(e) => setText(e.target.value)}
        placeholder="Enter todo"
      />
      <button onClick={addTodo}>Add</button>

      <table>
        <thead>
          <tr>
            <th>#</th>
            <th>Task</th>
            <th>Action</th>
          </tr>
        </thead>
        <tbody>
          {todos.length === 0 ? (
            <tr>
              <td colSpan="3">No todos</td>
            </tr>
          ) : (
            todos.map((todo, i) => (
              <tr key={i}>
                <td>{i + 1}</td>
                <td>{todo}</td>
                <td>
                  <button onClick={() => editTodo(i)}>Edit</button>
                  <button onClick={() => removeTodo(i)}>Remove</button>
                </td>
              </tr>
            ))
          )}
        </tbody>
      </table>
    </div>
  );
}
```

**Your clean main.jsx should look like this:**

```jsx
import { createRoot } from 'react-dom/client'
import App from './App.jsx'

createRoot(document.getElementById('root')).render(
    <App />
)

```

## **Success! 🎉**

**You now have:**

- ✅ Clean React project structure
- ✅ Simple "Hello World" display
- ✅ Working live updates

**Next:** You can start building your Todo components!

## 🧩 **Phase 3: Create Another React App (Counter App)**



---

## **Step 1: Create New Project Structure**

---

### **1.1 Create New Folder for Counter App**

Create a new folder for your new project:

```bash
mkdir Counter
cd Counter

```

---

## **Step 2: Set Up React App Using Vite**

Run the Vite creation command:

```bash
npm create vite@latest

```

When prompted:

- **Project name:** `.`
- **Framework:** `React`
- **Variant:** `JavaScript`

Then install dependencies:

```bash
npm install

```

And start the development server:

```bash
npm run dev

```

---

## **Step 3: Clean Project Files**

Just like in Phase 2, clean up your setup:

1. Delete `App.css`, `index.css`, and all images inside `src/assets` and `public`.
2. Clear `App.jsx` and `main.jsx` to prepare for fresh code.

---

## **Step 4: Create the Counter App**

### **4.1 App.jsx**

Replace the content of `src/App.jsx` with this:

```jsx
import React, { useState } from "react";

const App = () => {
  const [count, setCount] = useState(0);

  return (
    <div style={{ padding: "20px", textAlign: "center" }}>
      <h1>Counter App</h1>
      <p style={{ fontSize: "48px", fontWeight: "bold", margin: "20px 0" }}>
        {count}
      </p>

      <div style={{ display: "flex", gap: "10px", justifyContent: "center" }}>
        <button
          onClick={() => setCount(count - 1)}
          style={{
            padding: "10px 20px",
            fontSize: "18px",
            backgroundColor: "#dc3545",
            color: "white",
            border: "none",
            borderRadius: "5px",
            cursor: "pointer",
          }}
        >
          -
        </button>

        <button
          onClick={() => setCount(0)}
          style={{
            padding: "10px 20px",
            fontSize: "18px",
            backgroundColor: "#6c757d",
            color: "white",
            border: "none",
            borderRadius: "5px",
            cursor: "pointer",
          }}
        >
          Reset
        </button>

        <button
          onClick={() => setCount(count + 1)}
          style={{
            padding: "10px 20px",
            fontSize: "18px",
            backgroundColor: "#28a745",
            color: "white",
            border: "none",
            borderRadius: "5px",
            cursor: "pointer",
          }}
        >
          +
        </button>
      </div>
    </div>
  );
};

export default App;

```

---

### **4.2 main.jsx**

```jsx
import { createRoot } from 'react-dom/client'
import App from './App.jsx'

createRoot(document.getElementById('root')).render(
    <App />
)

```

---

## **Step 5: Verify Your Counter App**

Run your app:

```bash
npm run dev

```

Visit → [http://localhost:5173](http://localhost:5173/)

✅ You should see:

- A **Counter App title**
- A number displayed (starting from 0)
- Three buttons: **“–”**, **“Reset”**, and **“+”**

Click the buttons to test:

- ➖ Decreases count
- 🔁 Resets count to 0
- ➕ Increases count

---

## ✅ **Success!**

You now have:

- 🧮 A **fully working Counter App**
- ⚡ Built with **React + Vite**
- 🧹 A clean project structure

## 🧩 Phase 4: React Props Mastery

---

## **Step 1: Create Props Project**

bash

```
mkdir ReactProps
cd ReactProps
npm create vite@latest .
# Select: React → JavaScript
npm install
npm run dev
```

---

## **📚 Props Fundamentals**

### **What are Props?**

- **Props** (properties) are data passed from parent to child components
- **Read-only** - components cannot modify their own props
- **Unidirectional** - data flows down from parent to child
- **Any data type** - strings, numbers, arrays, objects, functions, JSX

### **🛠 Basic Syntax**

jsx

```
// Parent Component
<ChildComponent name="John" age={25} />// Child Component
const ChildComponent = (props) => {
  return <div>Hello {props.name}, age {props.age}</div>}

// OR with destructuring
const ChildComponent = ({ name, age }) => {
  return <div>Hello {name}, age {age}</div>}
```

---

## **Example 1: Basic Props**

**Create `BasicPropsExample.jsx`:**

jsx

```
import React from 'react'

// Child Component
const UserCard = ({ name, age, email, isOnline }) => {
  return (
    <div style={{
      border: '1px solid #ccc',
      padding: '20px',
      margin: '10px',
      borderRadius: '8px',
      backgroundColor: isOnline ? '#e8f5e8' : '#f5f5f5'
    }}>
      <h3>{name}</h3>
      <p>Age: {age}</p>
      <p>Email: {email}</p>
      <p>Status: {isOnline ? '🟢 Online' : '🔴 Offline'}</p>
    </div>)
}

// Parent Component
const BasicPropsExample = () => {
  return (
    <div style={{ padding: '20px' }}>
      <h2>Example 1: Basic Props</h2>

      <UserCardname="John Doe"age={28}email="john@example.com"isOnline={true}/>

      <UserCardname="Jane Smith"age={32}email="jane@example.com"isOnline={false}/>

      <UserCardname="Bob Johnson"age={25}email="bob@example.com"isOnline={true}/>
    </div>)
}

export default BasicPropsExample
```

**Update `main.jsx`:**

jsx

```
import { createRoot } from 'react-dom/client'
import BasicPropsExample from './BasicPropsExample.jsx'

createRoot(document.getElementById('root')).render(<BasicPropsExample />)
```

---

## **Example 2: Function Props (Callbacks)**

**Create `FunctionPropsExample.jsx`:**

jsx

```
import React, { useState } from 'react'

// Child Component
const Button = ({ onClick, children, variant = 'primary', size = 'medium' }) => {
  const styles = {
    primary: { backgroundColor: '#007bff', color: 'white' },
    secondary: { backgroundColor: '#6c757d', color: 'white' },
    danger: { backgroundColor: '#dc3545', color: 'white' }
  }

  const sizes = {
    small: { padding: '5px 10px', fontSize: '12px' },
    medium: { padding: '10px 20px', fontSize: '14px' },
    large: { padding: '15px 30px', fontSize: '16px' }
  }

  return (
    <button
      onClick={onClick}style={{
        border: 'none',
        borderRadius: '5px',
        cursor: 'pointer',
        margin: '5px',
        ...styles[variant],
        ...sizes[size]
      }}>
      {children}
    </button>)
}

// Parent Component
const FunctionPropsExample = () => {
  const [count, setCount] = useState(0)
  const [message, setMessage] = useState('')

  const handleIncrement = () => {
    setCount(count + 1)
    setMessage('Increased!')
  }

  const handleDecrement = () => {
    setCount(count - 1)
    setMessage('Decreased!')
  }

  const handleReset = () => {
    setCount(0)
    setMessage('Reset!')
  }

  const showAlert = (text) => {
    alert(text)
  }

  return (
    <div style={{ padding: '20px' }}>
      <h2>Example 2: Function Props (Callbacks)</h2>

      <div style={{ marginBottom: '20px' }}>
        <h3>Counter: {count}</h3>
        <p>{message}</p>
      </div>

      <div>
        <Button onClick={handleIncrement} variant="primary">
          Increment +
        </Button>

        <Button onClick={handleDecrement} variant="secondary">
          Decrement -
        </Button>

        <Button onClick={handleReset} variant="danger" size="small">
          Reset
        </Button>

        <ButtononClick={() => showAlert('Hello from button!')}variant="primary"size="large">
          Show Alert
        </Button>
      </div>

      <div style={{ marginTop: '30px', padding: '15px', backgroundColor: '#f8f9fa' }}>
        <h4>Key Points:</h4>
        <ul>
          <li>✅ Pass functions as props for child-to-parent communication</li>
          <li>✅ Child components can trigger parent functions</li>
          <li>✅ Use for events like clicks, form submissions, etc.</li>
        </ul>
      </div>
    </div>)
}

export default FunctionPropsExample
```

---

## **Example 3: Object & Array Props**

**Create `ObjectArrayPropsExample.jsx`:**

jsx

```
import React from 'react'

// Child Component for single product
const ProductCard = ({ product }) => {
  return (
    <div style={{
      border: '1px solid #ddd',
      borderRadius: '8px',
      padding: '15px',
      margin: '10px',
      textAlign: 'center',
      boxShadow: '0 2px 4px rgba(0,0,0,0.1)'
    }}>
      <img
        src={product.image}alt={product.name}style={{ width: '100px', height: '100px', objectFit: 'cover' }}/>
      <h3>{product.name}</h3>
      <p>{product.description}</p>
      <p style={{
        color: product.inStock ? 'green' : 'red',
        fontWeight: 'bold'
      }}>
        ${product.price} - {product.inStock ? 'In Stock' : 'Out of Stock'}
      </p>
      <button
        disabled={!product.inStock}style={{
          padding: '8px 16px',
          backgroundColor: product.inStock ? '#28a745' : '#6c757d',
          color: 'white',
          border: 'none',
          borderRadius: '4px',
          cursor: product.inStock ? 'pointer' : 'not-allowed'
        }}>
        {product.inStock ? 'Add to Cart' : 'Out of Stock'}
      </button>
    </div>)
}

// Child Component for product list
const ProductList = ({ products, category }) => {
  return (
    <div style={{ marginBottom: '30px' }}>
      <h3>{category} ({products.length} items)</h3>
      <div style={{ display: 'flex', flexWrap: 'wrap' }}>
        {products.map(product => (
          <ProductCard key={product.id} product={product} />))}
      </div>
    </div>)
}

// Parent Component
const ObjectArrayPropsExample = () => {
  const electronics = [
    {
      id: 1,
      name: "Wireless Headphones",
      description: "Noise cancelling wireless headphones",
      price: 199.99,
      inStock: true,
      image: "https://via.placeholder.com/100"
    },
    {
      id: 2,
      name: "Smartphone",
      description: "Latest model smartphone",
      price: 899.99,
      inStock: true,
      image: "https://via.placeholder.com/100"
    },
    {
      id: 3,
      name: "Gaming Laptop",
      description: "High-performance gaming laptop",
      price: 1499.99,
      inStock: false,
      image: "https://via.placeholder.com/100"
    }
  ]

  const books = [
    {
      id: 4,
      name: "React Guide",
      description: "Complete React development guide",
      price: 29.99,
      inStock: true,
      image: "https://via.placeholder.com/100"
    },
    {
      id: 5,
      name: "JavaScript Basics",
      description: "Learn JavaScript from scratch",
      price: 24.99,
      inStock: true,
      image: "https://via.placeholder.com/100"
    }
  ]

  return (
    <div style={{ padding: '20px' }}>
      <h2>Example 3: Object & Array Props</h2>

      <ProductList products={electronics} category="Electronics" />
      <ProductList products={books} category="Books" />

      <div style={{ marginTop: '30px', padding: '15px', backgroundColor: '#f8f9fa' }}>
        <h4>Key Points:</h4>
        <ul>
          <li>✅ Pass objects and arrays as props for complex data</li>
          <li>✅ Use map() to render lists of components</li>
          <li>✅ Each child in a list needs a unique key prop</li>
          <li>✅ Destructure objects in child components for clean code</li>
        </ul>
      </div>
    </div>)
}

export default ObjectArrayPropsExample
```

---

## **Example 4: Children Prop & Composition**

**Create `ChildrenPropsExample.jsx`:**

jsx

```
import React from 'react'

// Layout Components using children prop
const Container = ({ children, backgroundColor = 'white' }) => {
  return (
    <div style={{
      padding: '20px',
      margin: '10px',
      border: '1px solid #ccc',
      borderRadius: '8px',
      backgroundColor: backgroundColor
    }}>
      {children}
    </div>)
}

const Header = ({ children, level = 1 }) => {
  const HeaderTag = `h${level}`return <HeaderTag style={{ color: '#333' }}>{children}</HeaderTag>}

const Button = ({ children, onClick, type = 'button' }) => {
  return (
    <button
      type={type}onClick={onClick}style={{
        padding: '10px 20px',
        backgroundColor: '#007bff',
        color: 'white',
        border: 'none',
        borderRadius: '5px',
        cursor: 'pointer',
        margin: '5px'
      }}>
      {children}
    </button>)
}

// Specialized components using composition
const Card = ({ title, children, footer }) => {
  return (
    <Container backgroundColor="#f8f9fa">
      {title && <Header level={3}>{title}</Header>}
      <div style={{ margin: '15px 0' }}>
        {children}
      </div>
      {footer && (
        <div style={{
          borderTop: '1px solid #ddd',
          paddingTop: '10px',
          marginTop: '10px'
        }}>
          {footer}
        </div>)}
    </Container>)
}

// Parent Component
const ChildrenPropsExample = () => {
  const handleClick = (message) => {
    alert(message)
  }

  return (
    <div style={{ padding: '20px' }}>
      <h2>Example 4: Children Prop & Composition</h2>

      {/* Basic children usage */}
      <Container backgroundColor="#e3f2fd">
        <Header>Welcome to Our App</Header>
        <p>This content is passed as children prop</p>
        <Button onClick={() => handleClick('Hello from basic button!')}>
          Click Me
        </Button>
      </Container>

      {/* Card composition */}
      <Cardtitle="User Profile"footer={<small>Last updated: Today</small>}>
        <p>Name: John Doe</p>
        <p>Email: john@example.com</p>
        <p>Role: Administrator</p>
        <Button onClick={() => handleClick('Profile saved!')}>
          Save Profile
        </Button>
      </Card>

      <Card title="Settings">
        <p>Configure your application settings here:</p>
        <div>
          <Button onClick={() => handleClick('Notifications updated!')}>
            Notifications
          </Button>
          <Button onClick={() => handleClick('Privacy settings saved!')}>
            Privacy
          </Button>
        </div>
      </Card>

      {/* Complex children with multiple elements */}
      <Container>
        <Header level={2}>Advanced Example</Header>
        <div style={{ display: 'flex', gap: '10px', flexWrap: 'wrap' }}>
          <Button onClick={() => handleClick('Action 1')}>
            🚀 Action 1
          </Button>
          <Button onClick={() => handleClick('Action 2')}>
            ⚡ Action 2
          </Button>
          <Button onClick={() => handleClick('Action 3')}>
            🔧 Action 3
          </Button>
        </div>
      </Container>

      <div style={{ marginTop: '30px', padding: '15px', backgroundColor: '#f8f9fa' }}>
        <h4>Key Points:</h4>
        <ul>
          <li>✅ <code>children</code> prop allows component composition</li>
          <li>✅ Pass JSX elements between opening and closing tags</li>
          <li>✅ Build reusable layout components</li>
          <li>✅ Create component hierarchies and specialized components</li>
        </ul>
      </div>
    </div>)
}

export default ChildrenPropsExample
```

---

## **Example 5: Advanced Props (Default Props, PropTypes, Spread)**

**Create `AdvancedPropsExample.jsx`:**

jsx

```
import React from 'react'

// Component with default props
const UserProfile = ({
  name = 'Anonymous',
  age = 0,
  email = 'No email provided',
  isVerified = false,
  hobbies = [],
  ...rest
}) => {
  return (
    <div
      {...rest}style={{
        border: '1px solid #ccc',
        padding: '20px',
        margin: '10px',
        borderRadius: '8px',
        backgroundColor: isVerified ? '#e8f5e8' : '#f5f5f5',
        ...rest.style
      }}>
      <div style={{ display: 'flex', alignItems: 'center', gap: '10px' }}>
        <h3>{name}</h3>
        {isVerified && <span style={{ color: 'green' }}>✓ Verified</span>}
      </div>

      <p><strong>Age:</strong> {age}</p>
      <p><strong>Email:</strong> {email}</p>

      {hobbies.length > 0 && (
        <div>
          <strong>Hobbies:</strong>
          <ul>
            {hobbies.map((hobby, index) => (
              <li key={index}>{hobby}</li>))}
          </ul>
        </div>)}

      {hobbies.length === 0 && (
        <p style={{ color: '#666', fontStyle: 'italic' }}>No hobbies listed</p>)}
    </div>)
}

// Component with prop spreading
const FancyButton = ({ variant = 'primary', size = 'medium', ...buttonProps }) => {
  const baseStyle = {
    border: 'none',
    borderRadius: '6px',
    cursor: 'pointer',
    fontWeight: 'bold',
    transition: 'all 0.2s',
    margin: '5px'
  }

  const variants = {
    primary: { backgroundColor: '#007bff', color: 'white' },
    secondary: { backgroundColor: '#6c757d', color: 'white' },
    success: { backgroundColor: '#28a745', color: 'white' },
    danger: { backgroundColor: '#dc3545', color: 'white' }
  }

  const sizes = {
    small: { padding: '6px 12px', fontSize: '12px' },
    medium: { padding: '10px 20px', fontSize: '14px' },
    large: { padding: '14px 28px', fontSize: '16px' }
  }

  return (
    <button
      {...buttonProps}style={{
        ...baseStyle,
        ...variants[variant],
        ...sizes[size],
        ...buttonProps.style
      }}/>)
}

// Parent Component
const AdvancedPropsExample = () => {
  const userData = {
    name: "Sarah Johnson",
    age: 29,
    email: "sarah@example.com",
    isVerified: true,
    hobbies: ["Reading", "Hiking", "Photography"]
  }

  const partialUserData = {
    name: "Mike Smith",
    email: "mike@example.com"
    // age and isVerified will use defaults
  }

  return (
    <div style={{ padding: '20px' }}>
      <h2>Example 5: Advanced Props Techniques</h2>

      <div style={{ marginBottom: '30px' }}>
        <h3>Default Props Example</h3>

        {/* Full props provided */}
        <UserProfilename="Alice Brown"age={25}email="alice@example.com"isVerified={true}hobbies={["Swimming", "Coding"]}/>

        {/* Using spread operator with object */}
        <UserProfile {...userData} />

        {/* Partial props - defaults will be used */}
        <UserProfile {...partialUserData} />

        {/* Minimum props - all defaults */}
        <UserProfile />

        {/* Additional props passed through */}
        <UserProfilename="Tom Wilson"age={35}style={{ border: '2px solid blue', backgroundColor: '#e6f3ff' }}data-testid="user-profile-1"/>
      </div>

      <div style={{ marginBottom: '30px' }}>
        <h3>Prop Spreading Example</h3>

        <FancyButton variant="primary">
          Primary Button
        </FancyButton>

        <FancyButton variant="success" size="large">
          Success Button
        </FancyButton>

        <FancyButton variant="danger" size="small">
          Danger Button
        </FancyButton>

        {/* Button with additional props */}
        <FancyButtonvariant="secondary"onClick={() => alert('Button clicked!')}disabled={false}title="Hover tooltip"style={{ transform: 'scale(1.1)' }}>
          Custom Button
        </FancyButton>
      </div>

      <div style={{ marginTop: '30px', padding: '15px', backgroundColor: '#f8f9fa' }}>
        <h4>Advanced Props Techniques:</h4>
        <ul>
          <li>✅ <strong>Default Props:</strong> Provide fallback values</li>
          <li>✅ <strong>Prop Spreading:</strong> Pass multiple props easily with <code>...</code></li>
          <li>✅ <strong>Rest Props:</strong> Capture remaining props with <code>...rest</code></li>
          <li>✅ <strong>Conditional Rendering:</strong> Show/hide based on prop values</li>
          <li>✅ <strong>Prop Destructuring:</strong> Clean syntax for accessing props</li>
        </ul>
      </div>
    </div>)
}

export default AdvancedPropsExample
```

---

## **Navigation App**

**Create `App.jsx` for navigation:**

jsx

```
import React, { useState } from 'react'
import BasicPropsExample from './BasicPropsExample'
import FunctionPropsExample from './FunctionPropsExample'
import ObjectArrayPropsExample from './ObjectArrayPropsExample'
import ChildrenPropsExample from './ChildrenPropsExample'
import AdvancedPropsExample from './AdvancedPropsExample'

const examples = [
  { name: '1. Basic Props', component: BasicPropsExample },
  { name: '2. Function Props', component: FunctionPropsExample },
  { name: '3. Object & Array Props', component: ObjectArrayPropsExample },
  { name: '4. Children Props', component: ChildrenPropsExample },
  { name: '5. Advanced Props', component: AdvancedPropsExample }
]

const App = () => {
  const [currentExample, setCurrentExample] = useState(0)
  const CurrentComponent = examples[currentExample].component

  return (
    <div style={{ display: 'flex', height: '100vh' }}>
      {/* Sidebar */}
      <div style={{
        width: '250px',
        backgroundColor: '#f8f9fa',
        borderRight: '1px solid #dee2e6',
        overflow: 'auto',
        padding: '20px'
      }}>
        <h3>React Props Examples</h3>
        {examples.map((example, index) => (
          <button
            key={example.name}onClick={() => setCurrentExample(index)}style={{
              width: '100%',
              textAlign: 'left',
              padding: '10px',
              margin: '5px 0',
              backgroundColor: currentExample === index ? '#007bff' : 'transparent',
              color: currentExample === index ? 'white' : 'black',
              border: '1px solid #dee2e6',
              borderRadius: '4px',
              cursor: 'pointer'
            }}>
            {example.name}
          </button>))}

        <div style={{ marginTop: '30px', padding: '15px', backgroundColor: '#e9ecef', borderRadius: '5px' }}>
          <h4>Props Summary:</h4>
          <ul style={{ fontSize: '14px', paddingLeft: '20px' }}>
            <li>📦 Pass data to components</li>
            <li>🔄 One-way data flow</li>
            <li>🎯 Read-only</li>
            <li>🔧 Any data type</li>
            <li>🧩 Component composition</li>
          </ul>
        </div>
      </div>

      {/* Main Content */}
      <div style={{ flex: 1, overflow: 'auto' }}>
        <CurrentComponent />
      </div>
    </div>)
}

export default App
```

**Update `main.jsx`:**

jsx

```
import { createRoot } from 'react-dom/client'
import App from './App.jsx'

createRoot(document.getElementById('root')).render(<App />)
```

---

## **✅ Phase 4 Complete!**

### **🎯 What You've Learned:**

**5 Essential Props Patterns:**

1. **Basic Props** - Strings, numbers, booleans
2. **Function Props** - Callbacks for child-to-parent communication
3. **Object & Array Props** - Complex data structures
4. **Children Props** - Component composition and layout
5. **Advanced Props** - Default values, spreading, destructuring

### **🚀 Key Benefits:**

- ✅ **Reusable components** - Make components flexible with props
- ✅ **Data flow control** - Parent components control child data
- ✅ **Clean architecture** - Separate data and presentation
- ✅ **Type safety** - Catch errors with proper prop handling
- ✅ **Maintainable code** - Easy to understand and modify

### **💡 Pro Tips:**

- Use **destructuring** for cleaner prop access
- Set **default values** for optional props
- Use **prop spreading** (...props) for wrapper components
- Always include **key prop** in lists
- Use **children prop** for layout components

**Run `npm run dev` and explore each example to master React props!**

## 🧩 Phase 5: Essential React Hooks Mastery

---

## **Step 1: Create Hooks Project**

bash

```
mkdir ReactHooks
cd ReactHooks
npm create vite@latest .
# Select: React → JavaScript
npm install
npm run dev
```

---

## **Hook 1: useState - State Management**

### **📚 Explanation**

Manages component state with getter and setter functions. Triggers re-renders when state changes.

### **🛠 Syntax**

jsx

```
const [state, setState] = useState(initialValue)
```

### **💡 Example**

**Create `UseStateExample.jsx`:**

jsx

```
import React, { useState } from 'react'

const UseStateExample = () => {
  const [count, setCount] = useState(0)
  const [name, setName] = useState('')

  return (
    <div style={{ padding: '20px' }}>
      <h2>useState Hook</h2>

      <div style={{ marginBottom: '20px' }}>
        <h3>Counter: {count}</h3>
        <button onClick={() => setCount(count + 1)}>+</button>
        <button onClick={() => setCount(count - 1)}>-</button>
        <button onClick={() => setCount(0)}>Reset</button>
      </div>

      <div>
        <h3>Name: {name || 'Not entered'}</h3>
        <input
          value={name}onChange={(e) => setName(e.target.value)}placeholder="Enter name"/>
      </div>
    </div>)
}

export default UseStateExample
```

**Update `main.jsx`:**

jsx

```
import { createRoot } from 'react-dom/client'
import UseStateExample from './UseStateExample.jsx'

createRoot(document.getElementById('root')).render(<UseStateExample />)
```

---

## **Hook 2: useEffect - Side Effects**

### **📚 Explanation**

Handles side effects like API calls, subscriptions, timers. Runs after render completes.

### **🛠 Syntax**

jsx

```
useEffect(() => {
  // effect code
  return () => { /* cleanup */ }
}, [dependencies])
```

### **💡 Example**

**Create `UseEffectExample.jsx`:**

jsx

```
import React, { useState, useEffect } from 'react'

const UseEffectExample = () => {
  const [count, setCount] = useState(0)
  const [data, setData] = useState(null)

  // Run on every render
  useEffect(() => {
    document.title = `Count: ${count}`})

  // Run once on mount
  useEffect(() => {
    fetch('https://jsonplaceholder.typicode.com/todos/1')
      .then(response => response.json())
      .then(json => setData(json))
  }, [])

  // Run when count changes
  useEffect(() => {
    if (count > 5) {
      alert('Count is high!')
    }
  }, [count])

  return (
    <div style={{ padding: '20px' }}>
      <h2>useEffect Hook</h2>
      <p>Count: {count}</p>
      <button onClick={() => setCount(count + 1)}>Increment</button>

      <div style={{ marginTop: '20px' }}>
        <h3>API Data:</h3>
        <pre>{data ? JSON.stringify(data, null, 2) : 'Loading...'}</pre>
      </div>
    </div>)
}

export default UseEffectExample
```

---

## **Hook 3: useContext - Global State**

### **📚 Explanation**

Access context values without prop drilling. Shares data across component tree.

### **🛠 Syntax**

jsx

```
const value = useContext(MyContext)
```

### **💡 Example**

**Create `UseContextExample.jsx`:**

jsx

```
import React, { createContext, useContext, useState } from 'react'

const ThemeContext = createContext()

const ThemedButton = () => {
  const { theme, toggleTheme } = useContext(ThemeContext)

  return (
    <button
      onClick={toggleTheme}style={{
        backgroundColor: theme === 'light' ? '#fff' : '#333',
        color: theme === 'light' ? '#000' : '#fff',
        padding: '10px 20px'
      }}>
      Current: {theme}
    </button>)
}

const UseContextExample = () => {
  const [theme, setTheme] = useState('light')

  const toggleTheme = () => {
    setTheme(prev => prev === 'light' ? 'dark' : 'light')
  }

  return (
    <ThemeContext.Provider value={{ theme, toggleTheme }}>
      <div style={{
        padding: '20px',
        backgroundColor: theme === 'light' ? '#f5f5f5' : '#222',
        minHeight: '200px'
      }}>
        <h2>useContext Hook</h2>
        <ThemedButton />
        <p>No prop drilling needed!</p>
      </div>
    </ThemeContext.Provider>)
}

export default UseContextExample
```

---

## **Hook 4: useReducer - Complex State**

### **📚 Explanation**

Manages complex state logic with reducers. Better for multiple related state values.

### **🛠 Syntax**

jsx

```
const [state, dispatch] = useReducer(reducer, initialState)
```

### **💡 Example**

**Create `UseReducerExample.jsx`:**

jsx

```
import React, { useReducer } from 'react'

const counterReducer = (state, action) => {
  switch (action.type) {
    case 'INCREMENT':
      return { count: state.count + 1 }
    case 'DECREMENT':
      return { count: state.count - 1 }
    case 'RESET':
      return { count: 0 }
    default:
      return state
  }
}

const UseReducerExample = () => {
  const [state, dispatch] = useReducer(counterReducer, { count: 0 })

  return (
    <div style={{ padding: '20px' }}>
      <h2>useReducer Hook</h2>
      <h3>Count: {state.count}</h3>

      <button onClick={() => dispatch({ type: 'INCREMENT' })}>
        Increment
      </button>
      <button onClick={() => dispatch({ type: 'DECREMENT' })}>
        Decrement
      </button>
      <button onClick={() => dispatch({ type: 'RESET' })}>
        Reset
      </button>
    </div>)
}

export default UseReducerExample
```

---

## **Hook 5: useMemo - Expensive Calculations**

### **📚 Explanation**

Memoizes expensive calculations. Only recalculates when dependencies change.

### **🛠 Syntax**

jsx

```
const memoizedValue = useMemo(() => computeExpensiveValue(a, b), [a, b])
```

### **💡 Example**

**Create `UseMemoExample.jsx`:**

jsx

```
import React, { useState, useMemo } from 'react'

const UseMemoExample = () => {
  const [number, setNumber] = useState(1)
  const [dark, setDark] = useState(false)

  const expensiveCalculation = (num) => {
    console.log('Calculating...')
    for (let i = 0; i < 1000000000; i++) {}
    return num * 2
  }

  const doubleNumber = useMemo(() => {
    return expensiveCalculation(number)
  }, [number])

  const themeStyles = {
    backgroundColor: dark ? 'black' : 'white',
    color: dark ? 'white' : 'black',
    padding: '20px',
    margin: '10px 0'
  }

  return (
    <div style={{ padding: '20px' }}>
      <h2>useMemo Hook</h2>

      <input
        type="number"value={number}onChange={e => setNumber(parseInt(e.target.value))}/>

      <button onClick={() => setDark(prev => !prev)}>
        Toggle Theme
      </button>

      <div style={themeStyles}>
        Result: {doubleNumber}
      </div>
    </div>)
}

export default UseMemoExample
```

---

## **Hook 6: useRef - DOM References**

### **📚 Explanation**

Creates mutable references that don't trigger re-renders. Access DOM elements directly.

### **🛠 Syntax**

jsx

```
const ref = useRef(initialValue)
// Access: ref.current
```

### **💡 Example**

**Create `UseRefExample.jsx`:**

jsx

```
import React, { useRef, useEffect, useState } from 'react'

const UseRefExample = () => {
  const inputRef = useRef()
  const countRef = useRef(0)
  const [count, setCount] = useState(0)

  useEffect(() => {
    inputRef.current.focus()
  }, [])

  const handleFocus = () => {
    inputRef.current.focus()
    inputRef.current.select()
  }

  return (
    <div style={{ padding: '20px' }}>
      <h2>useRef Hook</h2>

      <input ref={inputRef} placeholder="Auto-focused" />
      <button onClick={handleFocus}>Focus Input</button>

      <div style={{ marginTop: '20px' }}>
        <p>State Count: {count} (re-renders)</p>
        <p>Ref Count: {countRef.current} (no re-render)</p>

        <button onClick={() => setCount(count + 1)}>
          Update State
        </button>
        <button onClick={() => countRef.current += 1}>
          Update Ref (check console)
        </button>
      </div>
    </div>)
}

export default UseRefExample
```

---

## **Hook 7: useCallback - Memoized Functions**

### **📚 Explanation**

Memoizes functions to prevent unnecessary re-renders of child components.

### **🛠 Syntax**

jsx

```
const memoizedCallback = useCallback(() => { doSomething(a, b) }, [a, b])
```

### **💡 Example**

**Create `UseCallbackExample.jsx`:**

jsx

```
import React, { useState, useCallback, memo } from 'react'

const Child = memo(({ onClick, name }) => {
  console.log('Child rendered')
  return <button onClick={onClick}>{name}</button>})

const UseCallbackExample = () => {
  const [count, setCount] = useState(0)
  const [value, setValue] = useState('')

  const increment = useCallback(() => {
    setCount(c => c + 1)
  }, [])

  const decrement = useCallback(() => {
    setCount(c => c - 1)
  }, [])

  return (
    <div style={{ padding: '20px' }}>
      <h2>useCallback Hook</h2>
      <p>Count: {count}</p>

      <Child onClick={increment} name="Increment" />
      <Child onClick={decrement} name="Decrement" />

      <input
        value={value}onChange={(e) => setValue(e.target.value)}placeholder="Type to test re-renders"/>

      <p>Check console for re-renders</p>
    </div>)
}

export default UseCallbackExample
```

---

## **Hook 8: useTransition - Non-blocking Updates**

### **📚 Explanation**

Marks state updates as non-blocking transitions to keep UI responsive.

### **🛠 Syntax**

jsx

```
const [isPending, startTransition] = useTransition()
```

### **💡 Example**

**Create `UseTransitionExample.jsx`:**

jsx

```
import React, { useState, useTransition } from 'react'

const UseTransitionExample = () => {
  const [query, setQuery] = useState('')
  const [filter, setFilter] = useState('')
  const [isPending, startTransition] = useTransition()

  const items = Array.from({ length: 10000 }, (_, i) => `Item ${i}`)

  const filteredItems = items.filter(item =>
    item.toLowerCase().includes(filter.toLowerCase())
  )

  const handleSearch = (e) => {
    const value = e.target.value
    setQuery(value) // Urgent update

    startTransition(() => {
      setFilter(value) // Non-urgent transition
    })
  }

  return (
    <div style={{ padding: '20px' }}>
      <h2>useTransition Hook</h2>

      <input
        value={query}onChange={handleSearch}placeholder="Search..."style={{
          border: isPending ? '2px solid orange' : '2px solid blue'
        }}/>

      <p>Status: {isPending ? '⏳ Updating...' : '✅ Ready'}</p>

      <div style={{ height: '300px', overflow: 'auto' }}>
        {filteredItems.slice(0, 100).map((item, i) => (
          <div key={i}>{item}</div>))}
      </div>
    </div>)
}

export default UseTransitionExample
```

---

## **Hook 9: useId - Unique IDs**

### **📚 Explanation**

Generates unique IDs that are stable across server and client rendering.

### **🛠 Syntax**

jsx

```
const id = useId()
```

### **💡 Example**

**Create `UseIdExample.jsx`:**

jsx

```jsx
import React, { useId } from 'react'

const UseIdExample = () => {
  const nameId = useId()
  const emailId = useId()
  const checkboxId = useId()

  return (
    <div style={{ padding: '20px' }}>
      <h2>useId Hook</h2>

      <form style={{ maxWidth: '300px' }}>
        <div style={{ marginBottom: '15px' }}>
          <label htmlFor={nameId}>Name:</label>
          <input id={nameId} type="text" />
        </div>

        <div style={{ marginBottom: '15px' }}>
          <label htmlFor={emailId}>Email:</label>
          <input id={emailId} type="email" />
        </div>

        <div>
          <input id={checkboxId} type="checkbox" />
          <label htmlFor={checkboxId}>Subscribe</label>
        </div>
      </form>

      <div style={{ marginTop: '20px', background: '#f5f5f5', padding: '10px' }}>
        <p>Generated IDs:</p>
        <ul>
          <li>Name: {nameId}</li>
          <li>Email: {emailId}</li>
          <li>Checkbox: {checkboxId}</li>
        </ul>
      </div>
    </div>)
}

export default UseIdExample
```

---

## **Navigation App**

**Create `App.jsx` for navigation:**

jsx

```jsx
import React, { useState } from 'react'
import UseStateExample from './UseStateExample'
import UseEffectExample from './UseEffectExample'
import UseContextExample from './UseContextExample'
import UseReducerExample from './UseReducerExample'
import UseMemoExample from './UseMemoExample'
import UseRefExample from './UseRefExample'
import UseCallbackExample from './UseCallbackExample'
import UseTransitionExample from './UseTransitionExample'
import UseIdExample from './UseIdExample'

const hooks = [
  { name: '1. useState', component: UseStateExample },
  { name: '2. useEffect', component: UseEffectExample },
  { name: '3. useContext', component: UseContextExample },
  { name: '4. useReducer', component: UseReducerExample },
  { name: '5. useMemo', component: UseMemoExample },
  { name: '6. useRef', component: UseRefExample },
  { name: '7. useCallback', component: UseCallbackExample },
  { name: '8. useTransition', component: UseTransitionExample },
  { name: '9. useId', component: UseIdExample }
]

const App = () => {
  const [currentHook, setCurrentHook] = useState(0)
  const CurrentComponent = hooks[currentHook].component

  return (
    <div style={{ display: 'flex', height: '100vh' }}>
      {/* Sidebar */}
      <div style={{
        width: '250px',
        backgroundColor: '#f8f9fa',
        borderRight: '1px solid #dee2e6',
        overflow: 'auto',
        padding: '20px'
      }}>
        <h3>React Hooks</h3>
        {hooks.map((hook, index) => (
          <button
            key={hook.name}onClick={() => setCurrentHook(index)}style={{
              width: '100%',
              textAlign: 'left',
              padding: '10px',
              margin: '5px 0',
              backgroundColor: currentHook === index ? '#007bff' : 'transparent',
              color: currentHook === index ? 'white' : 'black',
              border: '1px solid #dee2e6',
              borderRadius: '4px',
              cursor: 'pointer'
            }}>
            {hook.name}
          </button>))}
      </div>

      {/* Main Content */}
      <div style={{ flex: 1, overflow: 'auto' }}>
        <CurrentComponent />
      </div>
    </div>)
}

export default App
```

**Update `main.jsx`:**

jsx

```
import { createRoot } from 'react-dom/client'
import App from './App.jsx'

createRoot(document.getElementById('root')).render(<App />)
```

---

## **✅ Phase 5 Complete!**

**You now have 9 essential React hooks with:**

- 📚 **Clear explanations** of each hook's purpose
- 🛠 **Simple syntax** examples
- 💡 **Practical, interactive examples**
- 🔄 **Easy navigation** between hooks

**To use:**

1. Run `npm run dev`
2. Click any hook in the sidebar to see it in action
3. Experiment with the interactive examples
4. Understand when and why to use each hook
