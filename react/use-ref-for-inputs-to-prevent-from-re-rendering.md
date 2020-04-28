# `useRef` instead of `useState` hook for input fields

To access a form field on submit use `useRef` hook instead of using `useState`:

```js
const emailInput = useRef();

const submit = () => {
  login({ email: emailInput.current.value });
}

...

<input ref={ emailInput } type="email" />
<button onClick={ submit }>Sign in</button>
```

This won't cause re-rendering on every keystroke which would happen if `useState` hook was used.

[Source](https://www.codebeast.dev/usestate-vs-useref-re-render-or-not/)
