# SnappFood-Like Console Application Named UTfood

This project implements a simplified console-based version of a food delivery system similar to SnappFood. It includes features for user registration, login, account management, restaurant and food menu management, and discount codes. The system supports three user roles: admin, customer, and restaurant.

## Features

### Admin
- Register and login to the system.
- Add and remove restaurants.
- Set and assign discount codes to specific users.
- View restaurant listings and filter them by type.
- View all discount codes and their respective owners.

### Customer
- Register and login/logout.
- Charge account balance.
- View restaurants and filter by type.
- Use discount codes.

### Restaurant
- Register and login/logout.
- Add and remove food items from the menu.
- Charge account balance.
- View menu and manage food items.

## Structure

- `Admin`: Manages restaurants and discount distribution.
- `Customer`: Represents end-users who order food.
- `Restaurant`: Hosts food items, manages its own menu.
- `Food`: Represents food items with name, category, price, and cost.
- `Discount`: Discount codes assigned to customers.
- `Snappfood`: The main controller class, handles commands and UI logic.

## Compilation and Execution

This project is implemented in standard C++ and can be compiled using g++ or any C++ compiler.

```bash
g++ -o snappfood main.cpp
./snappfood
```

## Sample Commands

```text
register user123 Pass123
login user123 Pass123
enter customer menu
charge account 500
logout
```

## Notes

- Passwords must include uppercase, lowercase, and a number and be at least 5 characters long.
- All usernames and passwords must follow a valid format with only alphanumeric characters and underscores.
- Discounts can only be set by the admin to registered customers.