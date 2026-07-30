# 🌿 Paradise Nursery - e-Plant Shopping

An interactive e-commerce web application for buying plants, built with **React**, **Redux Toolkit**, and **Vite**. Users can browse plant categories, add items to a shopping cart, manage quantities, and view real-time totals.

## 🚀 Features

- **Landing Page** – Welcome screen with "Get Started" button to enter the shop.
- **About Us Section** – Information about the nursery's mission and values.
- **Product Listing** – Browse plants organized by categories:
  - Air Purifying Plants
  - Aromatic Fragrant Plants
  - Insect Repellent Plants
  - Medicinal Plants
  - Low Maintenance Plants
- **Shopping Cart** – Full cart functionality:
  - Add items to cart with "Add to Cart" button (becomes disabled once added).
  - Increment / decrement item quantities.
  - Remove items from the cart.
  - Real-time subtotal per item and total cart amount.
  - Cart icon badge showing total quantity of items.
  - "Continue Shopping" button to return to the product list.
  - "Checkout" button (placeholder for future functionality).
- **State Management** – Powered by Redux Toolkit for predictable state handling.
- **Responsive Design** – Clean, modern UI with CSS styling.

## 📁 Project Structure

```
src/
├── assets/               # Static assets
├── AboutUs.css           # About Us page styles
├── AboutUs.jsx           # About Us component
├── App.css               # Global app styles
├── App.jsx               # Main app component (routing between landing & shop)
├── CartItem.css          # Cart item styles
├── CartItem.jsx          # Cart item component (quantity, remove, totals)
├── CartSlice.jsx         # Redux slice (actions: addItem, removeItem, updateQuantity)
├── index.css             # Base styles
├── main.jsx              # App entry point (Redux Provider setup)
├── ProductList.css       # Product listing styles
├── ProductList.jsx       # Product listing component (grid, add to cart, cart icon)
└── store.js              # Redux store configuration
```

## 🧰 Tech Stack

| Technology       | Purpose                     |
|------------------|-----------------------------|
| **React 18**     | User interface library      |
| **Redux Toolkit**| State management            |
| **React-Redux**  | React bindings for Redux    |
| **Vite**         | Build tool & dev server     |
| **ESLint**       | Code linting                |

## ⚙️ Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/FouadAlfarra/e-plantShopping.git
   cd e-plantShopping
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Run the development server**
   ```bash
   npm run dev
   ```
   Open your browser and navigate to the URL shown in the terminal (usually `http://localhost:5173`).

4. **Build for production**
   ```bash
   npm run build
   ```

5. **Preview the production build**
   ```bash
   npm run preview
   ```

## 🛒 How It Works

### Adding Items to Cart
- Click **"Add to Cart"** on any plant card.
- The button becomes disabled and changes to **"Added to Cart"**.
- The cart icon badge updates to show the total number of items.

### Managing Cart
- Click the **cart icon** in the navbar to open the cart view.
- Use **+** and **-** buttons to adjust quantities.
- Click **Delete** to remove an item entirely.
- The total cost updates automatically per item and overall.

### Continue Shopping
- Click **"Continue Shopping"** to return to the plant listing.

### Checkout
- Click **"Checkout"** (placeholder – currently shows an alert).

## 📦 Redux State

The app uses a single Redux slice (`CartSlice`) with:

- **State**: `{ items: [] }` – array of cart items.
- **Actions**:
  - `addItem({ name, image, cost })` – adds a plant or increments quantity if already in cart.
  - `removeItem(name)` – removes a plant from the cart.
  - `updateQuantity({ name, quantity })` – updates the quantity of a specific plant.

## 🧪 Scripts

| Command              | Description                    |
|----------------------|--------------------------------|
| `npm run dev`        | Start development server       |
| `npm run build`      | Build for production           |
| `npm run preview`    | Preview production build       |
| `npm run lint`       | Run ESLint                     |

## 👤 Author

**Fouad Alfarra** – [GitHub Profile](https://github.com/FouadAlfarra)

## 📄 License

This project is licensed under the MIT License – see the [LICENSE](LICENSE) file for details.