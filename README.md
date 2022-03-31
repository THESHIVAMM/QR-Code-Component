# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)

## Overview

### Screenshot

(./screenshot.png)

### Links

- Solution URL: [Add solution URL here](https://github.com/THESHIVAMM/QR-Code-Component)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Mobile-first workflow

### What I learned

I majorly used Bootstrap to create the Card component and then position it and make its border rounded.

To create card, I used the following code :

"HTML"

<div
      class="card text-center align-self-center position-absolute top-50 start-50 translate-middle rounded-3"
      style="width: 18rem"
    >
      <div class="imgi p-2">
        <img
          class="img-thumbnail border border-white rounded-3"
          src="./images/image-qr-code.png"
          alt="Card image cap"
        />
      </div>
      <div class="card-body flex-grow-1 pt-1 pb-5">
        <h5 class="card-title fw-bolder mt-0">
          Improve your front-end skills by building projects
        </h5>
        <p class="card-text flex-grow-1 fw-lighter" style="font-size: 15px">
          Scan the QR code to visit Frontend Mentor and take your coding skills
          to the next level
        </p>
      </div>
</div>
Here, the Bootstrap classes used with "card" bootstrap class are mainly for positioning the card in the center.

"CSS"
.card[style*="width: 18rem"] {
border-radius: 1rem !important;
}

This css code is used to make the border rounded to 1rem explicitly.

To make the QR Code section, I used following code :

```html
<div class="imgi p-2">
  <img
    class="img-thumbnail border border-white rounded-3"
    src="./images/image-qr-code.png"
    alt="Card image cap"
  />
</div>
```

I created a div to make its border thicker, used p-2 class for that. Then in img tag,used respective classes for white border and rounded corner and proper border width.

```css
.img-thumbnail {
  border-radius: 1rem !important;
}
}
```

This uses is used to overwrite the implicit border radius.

Then the text section is made from following piece of code:

"HTML"

<div class="card-body flex-grow-1 pt-1 pb-5">
  <h5 class="card-title fw-bolder mt-0">
    Improve your front-end skills by building projects
  </h5>
  <p class="card-text flex-grow-1 fw-lighter" style="font-size: 15px">
    Scan the QR code to visit Frontend Mentor and take your coding skills
    to the next level
  </p>
</div>
