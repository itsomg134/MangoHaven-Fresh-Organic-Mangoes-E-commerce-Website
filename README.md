# MangoHaven — Fresh Organic Mangoes E‑commerce Website

<img width="1881" height="2202" alt="image" src="https://github.com/user-attachments/assets/d74d5736-8d9c-4104-814c-097b62783534" />

> A beautifully crafted, fully responsive mango selling website with a dynamic shopping cart, local storage persistence, and a delightful user experience. Built with vanilla HTML, CSS, and JavaScript.

---

##  Features

-  **Product Catalog** — Display premium mango varieties with images, descriptions, and prices.
-  **Interactive Shopping Cart** — Add/remove items, update quantities, and see real-time total.
-  **Persistent Cart** — Cart data saved in `localStorage` so items remain after page refresh.
-  **Fully Responsive** — Optimized for mobile, tablet, and desktop screens.
-  **Toast Notifications** — User-friendly feedback when items are added or removed.
-  **Modern UI** — Clean, warm color scheme with smooth hover animations.
-  **Accessible** — Semantic HTML and keyboard-friendly interactions (ESC to close cart).

---

## Tech Stack

- **HTML5** — Semantic markup, accessible structure.
- **CSS3** — Flexbox, Grid, custom properties, responsive design.
- **JavaScript (ES6)** — Vanilla JS (no frameworks), DOM manipulation, localStorage API.
- **Font Awesome 6** — Icons for cart, mango logo, and buttons.
- **Google Fonts** — 'Inter' font family for modern typography.

---

##  Screenshots

| Homepage | Shopping Cart Sidebar |
|----------|------------------------|
| ![Homepage screenshot](https://via.placeholder.com/400x250?text=Hero+Section) | ![Cart Sidebar](https://via.placeholder.com/400x250?text=Shopping+Cart) |

*(Replace placeholder links with actual screenshots from your deployment)*

---

## Getting Started

Follow these instructions to get a copy of the project up and running on your local machine.

### Prerequisites

- Any modern web browser (Chrome, Firefox, Safari, Edge)
- A code editor (VS Code, Sublime, etc.) – optional, for customization
- Live Server extension (optional but recommended)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/mangohaven.git
   ```

2. **Navigate to project folder**
   ```bash
   cd mangohaven
   ```

3. **Open the `index.html` file**
   - Double-click `index.html` OR
   - Use Live Server in VS Code (Right-click → "Open with Live Server")

4. **Start shopping!**

> No build steps, no dependencies — just pure HTML/CSS/JS.

---

## Project Structure

```
mangohaven/
├── index.html          # Main HTML file (includes embedded CSS & JS)
├── README.md           # Project documentation (this file)
└── assets/             # (Optional) Folder for local images
    └── (place images here if you prefer local hosting)
```

> **Note:** The current version uses Unsplash placeholder images via URLs. For production, consider downloading and hosting images locally.

---

## How It Works

### Product Data
Products are stored as a JavaScript array of objects, each containing:
- `id`, `name`, `description`, `price`, `image URL`, `unit`

### Cart Logic
- `cart` array holds items with `id`, `name`, `price`, `quantity`.
- Functions: `addToCart()`, `updateQuantity()`, `removeItemFromCart()`
- `localStorage` syncs cart automatically after each modification.

### UI Updates
- `renderProducts()` — Dynamically generates product cards from the product array.
- `renderCartUI()` — Renders cart items and updates total price.
- `updateCartCount()` — Updates the cart badge number.

### Toast Notifications
- Temporary messages appear at the bottom center for 2 seconds.

---

## Customization

### Add More Products

Edit the `products` array inside the `<script>` tag in `index.html`:

```javascript
const products = [
    // ... existing products
    {
        id: 7,
        name: "Your New Mango",
        desc: "Amazing flavor, organic",
        price: 999,
        img: "your-image-url.jpg",
        unit: "dozen (6 pcs)"
    }
];
```

### Change Colors

Modify the CSS variables in the `<style>` section:

```css
:root {
    --primary: #e67e22;    /* mango orange */
    --secondary: #f39c12;  /* warm yellow */
    --dark: #2c1a0e;       /* earthy brown */
}
```

### Adjust Pricing or Currency

- The site uses Indian Rupee (₹). To change to another currency, replace `₹` symbols in the HTML/JS (search for `₹`).

---

##  Responsive Breakpoints

- **Desktop:** > 1024px — full grid (3–4 columns)
- **Tablet:** 768px – 1024px — 2–3 columns
- **Mobile:** < 768px — single column, smaller typography

---

## Contributing

Contributions are welcome! If you have ideas for improvements:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-idea`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-idea`)
5. Open a Pull Request

Please ensure your code follows the existing style and is well-commented where necessary.

---

## Known Issues & Future Improvements

### Current Limitations
- Images are loaded from Unsplash URLs; may break if the URLs change.
- No backend integration — cart is client-side only (good for demo/static sites).
- Checkout is simulated with an alert dialog.

### Planned Enhancements
- [ ] Add user authentication (login/register)
- [ ] Integrate a real payment gateway (Razorpay, Stripe)
- [ ] Add product search & filtering by price/variety
- [ ] Implement order history with localStorage
- [ ] Add a "Featured" section and customer reviews
- [ ] PWA support for offline access
- [ ] Dark mode toggle

---

##  License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

You are free to use, modify, and distribute this code for personal or commercial purposes with attribution.

---

## Acknowledgments

- **Images:** [Unsplash](https://unsplash.com/) for beautiful mango photography
- **Icons:** [Font Awesome](https://fontawesome.com/) (Free CDN)
- **Fonts:** [Google Fonts](https://fonts.google.com/) (Inter font)
- **Inspiration:** Local fruit vendors and the love for sweet, juicy mangoes! 🥭

---

## 📬 Contact

**Developer:** Your Name  
**Email:** your.email@example.com  
**GitHub:** [@your-username](https://github.com/your-username)  
**Project Link:** [https://github.com/your-username/mangohaven](https://github.com/your-username/mangohaven)

Feel free to reach out for questions, collaborations, or just to share your love for mangoes!
