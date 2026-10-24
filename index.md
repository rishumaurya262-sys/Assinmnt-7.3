# Assignment 7.3 — Responsive Product Listing

## HTML Code (`index.html`)

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Product Listing</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>Our Products</h1>

    <main class="product-container">
        <div class="product-card">
            <img src="https://placehold.co/300x200?text=Headphones" alt="Headphones">
            <h2>Headphones</h2>
            <p class="price">$25.00</p>
            <button>Add to Cart</button>
        </div>

        <div class="product-card">
            <img src="https://placehold.co/300x200?text=Smart+Watch" alt="Smart Watch">
            <h2>Smart Watch</h2>
            <p class="price">$40.00</p>
            <button>Add to Cart</button>
        </div>

        <div class="product-card">
            <img src="https://placehold.co/300x200?text=Keyboard" alt="Keyboard">
            <h2>Keyboard</h2>
            <p class="price">$30.00</p>
            <button>Add to Cart</button>
        </div>

        <div class="product-card">
            <img src="https://placehold.co/300x200?text=Mouse" alt="Mouse">
            <h2>Wireless Mouse</h2>
            <p class="price">$15.00</p>
            <button>Add to Cart</button>
        </div>

        <div class="product-card">
            <img src="https://placehold.co/300x200?text=Speaker" alt="Speaker">
            <h2>Bluetooth Speaker</h2>
            <p class="price">$35.00</p>
            <button>Add to Cart</button>
        </div>

        <div class="product-card">
            <img src="https://placehold.co/300x200?text=Backpack" alt="Backpack">
            <h2>Backpack</h2>
            <p class="price">$28.00</p>
            <button>Add to Cart</button>
        </div>
    </main>
</body>
</html>
```

## CSS Code (`style.css`)

```css
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

body {
    font-family: Arial, sans-serif;
    background-color: #f1f5f9;
    padding: 30px 20px;
}

h1 {
    text-align: center;
    margin-bottom: 30px;
}

.product-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: stretch;
    gap: 20px;
}

.product-card {
    background-color: white;
    border-radius: 10px;
    padding: 15px;
    text-align: center;
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);

    flex-grow: 1;
    flex-shrink: 1;
    flex-basis: 250px;

    max-width: 350px;
}

.product-card img {
    width: 100%;
    height: 180px;
    object-fit: cover;
    border-radius: 6px;
    margin-bottom: 15px;
}

.product-card h2 {
    font-size: 20px;
    margin-bottom: 10px;
}

.price {
    color: #2563eb;
    font-size: 18px;
    font-weight: bold;
    margin-bottom: 15px;
}

button {
    background-color: #2563eb;
    color: white;
    border: none;
    padding: 10px 16px;
    border-radius: 5px;
    cursor: pointer;
}

button:hover {
    background-color: #1d4ed8;
}

@media (max-width: 600px) {
    body {
        padding: 20px 12px;
    }

    .product-card {
        flex-basis: 100%;
        max-width: 100%;
    }
}
```

## Result

A responsive product listing was created using HTML and CSS Flexbox. It contains six product cards, each with an image, name, price, and button. The `display: flex`, `flex-wrap: wrap`, `gap`, `flex-grow`, `flex-shrink`, and `flex-basis` properties are used to control the layout and spacing. The cards wrap onto new lines and adjust to smaller screens.

## Submission

Submit the responsive product listing with the following files:

1. `index.html`
2. `style.css`
3. `Assignment-7.3.md`

Attach screenshots showing the product listing at desktop and mobile screen widths.