# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug involving the `useEffect` hook and its dependency array.  The code in `bug.js` shows an infinite loop due to a missing dependency in the `useEffect` hook. The corrected code is available in `bugSolution.js`.

**Problem:** The original code incorrectly omits `count` from the dependency array.  This results in the effect rerunning on every render, causing an infinite loop. 

**Solution:** The corrected code includes `count` in the dependency array. Now, the effect only reruns when `count` changes.