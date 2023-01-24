# React router
React Router is standard library for routing in React. It enables the navigation among views of various components in a React Application, allows changing the browser URL, and keeps the UI in sync with the URL.

- Install React Router:
```bash
npm install --save react-router-dom
```

- How to use

In index.tsx, import `BrowserRouter`.
```js
import React from 'react';
import ReactDOM from 'react-dom/client';
import './index.css';
import App from './App';
import { BrowserRouter } from 'react-router-dom';

const root = ReactDOM.createRoot(
  document.getElementById('root') as HTMLElement
);
root.render(
  <React.StrictMode>
    <BrowserRouter>
      <App />
    </BrowserRouter>
  </React.StrictMode>
);
```

In App.tsx, import any components and Route, Routes from react-router-dom.
You can specify multiple `Route` inside `Routes`.
```js
import React, { ReactElement } from 'react';
import './App.css';
import TodosPage from './pages/todos';
import ExamplePage from './pages/examples';
import { Route, Routes } from 'react-router-dom';


const App = (): ReactElement => {
  return (
    <div className="App">
      <Routes>
        <Route path='/' element={<TodosPage />} />
        <Route path='/example' element={<ExamplePage />} />
      </Routes>
    </div>
  );
}

export default App;
```
