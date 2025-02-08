# Frontend-machine-coding-Round-questions

Here are the best Reactjs machine coding round questions for freshers and experienced professionals who wants to master ReactJs skills. You can try to solve it first on your own without seeing the solution. Remember that by just copying my solution won't let you learn Reactjs. You need to use your brain and google everything to solve the below questions.

## 1. Build a simple counter app that has increment, decrement and reset functionality.


```import { useState, useEffect } from "react";
export default function App() {
  const [count, setCount] = useState(0);

  function incrementCounter() {
    setCount(count + 1);
  }
  function resetCounter() {
    setCount(0);
  }
  function deccrementCounter() {
    setCount(count - 1);
  }

  return (
    <div>
      <p>{count}</p>
      <div>
        <button onClick={incrementCounter}>Increment</button>
        <button onClick={resetCounter}>Reset</button>
        <button onClick={deccrementCounter}>Decrement</button>
      </div>
    </div>
  );
}
```
