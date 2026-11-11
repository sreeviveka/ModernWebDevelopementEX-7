# Exp 7 – React Lab Exercise: Frame-Based Layout Using React Components

## NAME:V.S.SREE VIVEKA  
## REG NO: 2305001031 

## Aim
To develop a frame-based webpage layout using React components such as Header, Sidebar, Content, and Footer.

## Objectives
- To understand component-based architecture in React.
- To create reusable React components.
- To arrange components to build a webpage layout.
- To apply CSS for styling different sections.

## Program

### Step 1: Header.jsx
```jsx
function Header() {
  return (
    <header className="header">
      <h1>Student Management System</h1>
    </header>
  );
}

export default Header;
```

### Step 2: Sidebar.jsx
```jsx
function Sidebar() {
  return (
    <aside className="sidebar">
      <h3>Menu</h3>

      <ul>
        <li>Home</li>
        <li>Students</li>
        <li>Courses</li>
        <li>Contact</li>
      </ul>
    </aside>
  );
}

export default Sidebar;
```

### Step 3: Content.jsx
```jsx
function Content() {
  return (
    <main className="content">
      <h2>Welcome to My Student Portal</h2>

      <h3>Student Name: SREE VIVEKA</h3>

      <p>
        This is my personal student dashboard.
      </p>

      <p>
        This page is designed using React components
        to display student details and application information.
      </p>
    </main>
  );
}

export default Content;
```

### Step 4: Footer.jsx
```jsx
function Footer() {
  return (
    <footer className="footer">
      <p>© 2026 Student Management System</p>
    </footer>
  );
}

export default Footer;
```

### Step 5: App.jsx
```jsx
import Header from "./components/Header";
import Sidebar from "./components/Sidebar";
import Content from "./components/Content";
import Footer from "./components/Footer";
import "./App.css";

function App() {
  return (
    <div className="app">
      <Header />

      <div className="main">
        <Sidebar />
        <Content />
      </div>

      <Footer />
    </div>
  );
}

export default App;
```

### Step 6: App.css
```css
* {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: Arial, sans-serif;
}

.app {
  min-height: 100vh;
}

.header {
  background-color: #1976d2;
  color: white;
  padding: 20px;
  text-align: center;
}

.main {
  display: flex;
  min-height: 400px;
}

.sidebar {
  width: 220px;
  background-color: #eeeeee;
  padding: 20px;
}

.sidebar ul {
  list-style: none;
  padding: 0;
}

.sidebar li {
  padding: 12px;
  margin-bottom: 5px;
  cursor: pointer;
}

.content {
  flex: 1;
  padding: 30px;
}

.content h2 {
  color: #1976d2;
}

.footer {
  background-color: #333333;
  color: white;
  text-align: center;
  padding: 15px;
}
```

## Output

### Frame-Based React Layout
<img width="1072" height="523" alt="image" src="https://github.com/user-attachments/assets/d63f3234-4e45-47ac-80e2-079b7f545fbb" />


## Result
Thus, a frame-based webpage layout was successfully created using React components and CSS.
