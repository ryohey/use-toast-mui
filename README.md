# useToast Hook for MUI

Hooks for super easy use of [MUI](https://github.com/mui/material-ui)'s [Snackbar](https://mui.com/material-ui/react-snackbar/).

## Installation

```sh
npm install use-toast-mui
```

## Setup

```js
<ToastProvider>
  <App />
</ToastProvider>
```

## useToast

`useToast` provides a function to display a [Snackbar](https://mui.com/material-ui/react-snackbar/) with [Alert](https://mui.com/material-ui/react-alert/).

```js
const ExampleButton = () => {
  const toast = useToast()
  return <button onClick={() => toast.success("hello!")}>
    push me
  </button>
}
```

## API

### success(message: string)

![image](https://user-images.githubusercontent.com/5355966/186865516-c5068e89-33e9-4762-b156-5e98fe38a83b.png)

### warning(message: string)

![image](https://user-images.githubusercontent.com/5355966/186863630-d8e618c8-85bb-4b14-8e3c-08d0aec9b210.png)

### info(message: string)

![image](https://user-images.githubusercontent.com/5355966/186865273-71fe753a-99b2-4bef-81c2-66d5601339f7.png)

### error(message: string)

![image](https://user-images.githubusercontent.com/5355966/186863529-af25c700-4140-49c9-ae44-f3fc0a816a49.png)

### show(message: string, options: { severity: AlertColor })

`show` accepts the severity as a parameter.

`show("hello", { severity: "info" })` is equivalent to `info("hello")`
