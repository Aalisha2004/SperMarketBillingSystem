# 🛒 Supermarket Billing System (C++)

This is a console-based Supermarket Billing System written in **C++**, designed to simulate a basic shopping and inventory system with administrator and buyer functionalities. Products can be added, edited, and deleted by the administrator, and buyers can purchase items and generate receipts.

---

## 📋 Features

### 🔐 Administrator

* **Login Protected** (hardcoded credentials)
* Add new products with price and discount
* Modify existing products
* Delete products
* View all products

### 🧾 Buyer

* View product list
* Place orders
* Generate receipt with:

  * Quantity
  * Price
  * Total amount after applying discount

---

## 🧑‍💻 Admin Login

| Field    | Value                          |
| -------- | ------------------------------ |
| Email    | `aalishapatwekar001@gmail.com` |
| Password | `aalisha123@`                  |

---

## 📁 File Structure

* **`database.txt`**
  Stores product records in the format:
  `pcode pname price discount`

* **`database1.txt`**
  Used as a temporary file for updating and deleting products.

---

## 📌 Functional Overview

### ✅ `menu()`

Displays the main menu with options for **Administrator**, **Buyer**, or **Exit**.

### ✅ `administrator()`

Accessible only after login. Allows:

* `add()` - Add new product
* `edit()` - Edit existing product
* `rem()` - Remove product

### ✅ `buyer()`

Allows buyer to:

* `receipt()` - View products, place orders, and generate receipt

### ✅ `list()`

Lists all available products.

---

## 💻 How to Run

1. Compile the program:

```bash
g++ supermarket.cpp -o supermarket
```

2. Run the executable:

```bash
./supermarket
```

---

## 📝 Sample Product Entry Format

```
101 Apple 50 5
102 Banana 20 0
103 Milk 40 10
```

---

## ⚠️ Notes

* Ensure `database.txt` is in the same directory as the executable.
* File I/O is used for persistent storage.
* Admin credentials are hardcoded — for real applications, use secure authentication.
* Uses `goto` statements for menu navigation (not recommended for modern C++ practices).


---

## 🧑‍💼 Author

**Aalisha Patwekar**
Email: `aalishapatwekar001@gmail.com`


