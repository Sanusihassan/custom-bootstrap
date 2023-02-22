<p align="center">
  <a href="https://getbootstrap.com/">
    <img src="https://getbootstrap.com/docs/5.2/assets/brand/bootstrap-logo-shadow.png" alt="Bootstrap logo" width="200" height="165">
  </a>
</p>

<h3 align="center">Custom Bootstrap</h3>

## Usage

1. install cssmolecule

```bash
npm install cssmolecule
```

2. install custom-bootstrap

```bash
npm install custom-bs
```

3. use it your project

- in your `main.jsx` or `main.tsx` or `main.js` file import the following:

```js
import "cssmolecule";
import "custom-bs";
// your sass entry point
import "./scss/main.scss";
```

- use it like this

```scss
.form {
  @include extend("form-inline py-3");
  // your custom styles
  h1 {
    @include extend("text-center text-capitalize");
  }

  input,
  textarea {
    @include extend("form-control my-2 px-4");
  }
  button {
    @include extend("btn btn-primary w-100");
    // customize without using !important
    background-color: red;
  }
}
// to extend a class

.form-2 {
  @include extend("form", ".");
}
```
