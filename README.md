# Korpa+

Korpa+ is a web grocery store designed for cooking enthusiasts who want to find everything they need for preparing healthy and high-quality meals in one place.

The application allows users to browse recipes, automatically add ingredients to their shopping cart, and manage their orders quickly and efficiently.


## Features

### Recipes
- Browse and search recipes
- Filter recipes by different criteria
- Detailed recipe view with instructions and ingredient lists

### Shopping Cart
- Automatic cart creation for each user
- Add ingredients to the cart directly from a recipe
- Modify quantities or remove items from the cart

### Orders and Payments
- Generate orders with user information
- Online payment using **Stripe integration**
- Discount coupons using the **Kuponify API**

### Statistics
- Display statistics about the most frequently added ingredients
- Data visualization using **Chart.js**


## Tech Stack

**Backend**
- Laravel 10

**Frontend**
- React

**Database**
- MySQL

**Other Tools**
- Stripe API (payments)
- Kuponify API (discount coupons)
- Chart.js (data visualization)


## Installation and Setup

Follow these steps to run the application locally.

### 1. Clone the repository

```bash
git clone https://github.com/milenadjeric/Online-Grocery-Store-with-Recipes.git
```

### 2. Navigate to the project folder

```bash
cd korpa-plus
```

### 3. Install dependencies

```bash
composer install
npm install
```

### 4. Environment configuration

Create a .env file by copying the example file:
```bash
cp .env.example .env
```
Update the following parameters in the .env file.

#### Database configuration
```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=database_name
DB_USERNAME=username
DB_PASSWORD=password
```

#### Stripe API keys
```
STRIPE_SECRET=your_secret_key
STRIPE_PUBLIC=your_public_key
```

#### Kuponify API token
```
KUPONIFY_API_TOKEN=your_token
```

### 5. Run database migrations and seed data

```bash
php artisan migrate --seed
```

### 6. Start the application

```bash
php artisan serve
npm run dev
```

The application should now be available at:
http://localhost:8000

## Author
Milena Djeric













