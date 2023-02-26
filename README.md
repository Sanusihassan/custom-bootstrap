<p align="center">
  <a href="https://getbootstrap.com/">
    <img src="https://getbootstrap.com/docs/5.2/assets/brand/bootstrap-logo-shadow.png" alt="Bootstrap logo" width="200" height="165">
  </a>
</p>

<h3 align="center">Custom Bootstrap</h3>

<p align="center">
Sleek, intuitive, and powerful front-end framework for faster and easier web development.
</p>

## Installation

1. install cssmolecule

```bash
npm install cssmolecule
```

2. install custom-bootstrap

```bash
npm install custom-bs
```

### Usage

- in your `main.jsx` or `main.tsx` or `main.js` file import the following:

```js
import "cssmolecule";
import "custom-bs";
// your sass entry point
import "./scss/main.scss";
```

Alternatively you can also import the files in your sass.

```scss
@import "cssmolecule/main.scss";
@import "custom-bs/scss/bootstrap.scss";
```

- use it like this

```scss
// include what you want you want from the framework
// for utilities
@include api;
// reboot/normalize
@include reboot;
// forms
@include forms;
// buttons
@include buttons;
.form {
  // you can use extend, apply or class
  @include extend("form-inline py-3");
  // your custom styles

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
