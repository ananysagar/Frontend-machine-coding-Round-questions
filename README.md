# Frontend-machine-coding-Round-questions

Here are the best Reactjs machine coding round questions for freshers and experienced professionals who wants to master ReactJs skills. You can try to solve it first on your own without seeing the solution. Remember that by just copying my solution won't let you learn Reactjs. You need to use your brain and google everything to solve the below questions.

## 1. Build a simple counter app that has increment, descrment and reset functionality.


import { useState, useEffect } from "react";<br/>
export default function App() {<br/>
  const [count, setCount] = useState(0);<br/>

  function incrementCounter() {<br/>
    setCount(count + 1);<br/>
  }<br/>
  function resetCounter() {<br/>
    setCount(0);<br/>
  }<br/>
  function deccrementCounter() {<br/>
    setCount(count - 1);<br/>
  }<br/>

  return (<br/>
    <div><br/>
      <p>{count}</p><br/>
      <div><br/>
        <button onClick={incrementCounter}>Increment</button><br/>
        <button onClick={resetCounter}>Reset</button><br/>
        <button onClick={deccrementCounter}>Decrement</button><br/>
      </div><br/>
    </div><br/>
  );<br/>
}
