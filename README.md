# 🌈 Colorful Half-Circle Loader 🎨

A simple animated half-circle loader with a vibrant rainbow gradient effect using pure CSS! Perfect for adding a splash of color to your loading screens.

---

## 🚀 Features

- 🌟 Six colorful rainbow segments revealed one by one
- 🎭 Uses CSS `repeating-radial-gradient` masking for distinct half-circles
- 🔄 Smooth step-based animation with no JavaScript needed
- ⚡ Lightweight and easy to customize

---

## 🎬 [Demo](https://linschmitz.github.io/RainbowLoader/)

---

## 🎯 Usage

### HTML

```html
<div class="loader"></div>
```

### CSS

```css
.loader {
  width: 120px;
  height: 60px;
  border-radius: 200px 200px 0 0;
  -webkit-mask: repeating-radial-gradient(
    farthest-side at bottom,
    #0000 0,
    #000 1px 12%,
    #0000 calc(12% + 1px) 20%
  );
  background: radial-gradient(
      farthest-side at bottom,
      #ff0000 0%,
      /* red */ #ffa500 20%,
      /* orange */ #ffff00 40%,
      /* yellow */ #008000 60%,
      /* green */ #0000ff 80%,
      /* blue */ #4b0082 95%,
      /* indigo */ #0000 100% /* transparent */
    ) bottom/0% 0% no-repeat #ddd;
  animation: l10 2s infinite steps(6);
}

@keyframes l10 {
  100% {
    background-size: 120% 120%;
  }
}
```

---

## 📄 License

This project is licensed under the MIT License.

---
