# Web components cheat sheet

## Bases

### Create component

```javascript
class MyComponent extends HTMLElement {
  constructor() {
    super();
  }
}
```

### Declare component to registry
```javascript
customElements.define('my-component', MyComponent);
```

### Create shadow DOM

```javascript
this.attachShadow({mode: 'open'});
this.shadowRoot // use it to manipulate the shadow DOM
```

### Life cycle
 * connectedCallback
 * disconnectedCallback

## Slot

### slot
Use slot
```html
<slot></slot>
```

### Style
```css
::slotted(h1) {
  /* define styles here for sloted h1*/
}
```
