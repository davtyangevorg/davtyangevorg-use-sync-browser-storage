React JS custom hook for working with Browser storages (localStorage,sessionStorage)

## Installation

```bash
npm install use-sync-browser-storage
```

## Available Hooks

useSyncWithLocalStorage: A hook for syncing with localStorage.
useSyncWithSessionStorage: A hook for syncing with sessionStorage

## Usage

useSyncWithLocalStorage

Example usage:

```jsx
import { useSyncWithLocalStorage } from "use-sync-browser-storage";

function Coutner() {
  const [count, updateCount] = useSyncWithLocalStorage({
    storageKey: "counter",
    initialState: 0,
  });

  return (
    <div>
      <div>{count}</div>
      <button onClick={() => updateCount(count + 1)}>increment </button>
    </div>
  );
}

export default Coutner;
```

## License

This project is licensed under the MIT License.
