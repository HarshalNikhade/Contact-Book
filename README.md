# 📒 Contact Book Management System (Python + MySQL)

A simple command-line **Contact Book Application** built in Python with MySQL as the database backend. This tool allows users to add, view, search, and delete contacts efficiently.

---

## 🚀 Features

* ✅ Add new contacts (Name, Phone, Email)
* 📋 View all saved contacts
* 🔍 Search a contact by name
* ❌ Delete a contact
* 💾 Data is stored persistently in a MySQL database

---

## 🛠️ Technologies Used

* **Python 3.x**
* **MySQL**
* `pymysql` library for Python-MySQL integration

---

## 🗃️ Database Schema

Make sure you have a MySQL database named `contact_book` and a table named `contacts` with the following schema:

```sql
CREATE DATABASE contact_book;

USE contact_book;

CREATE TABLE contacts (
    name VARCHAR(100),
    phone VARCHAR(15),
    email VARCHAR(100)
);
```

---

## 📦 Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/contact-book-python.git
   cd contact-book-python
   ```

2. **Install required library:**

   ```bash
   pip install pymysql
   ```

3. **Update MySQL credentials** in the `get_connection()` function:

   ```python
   host="localhost"
   user="root"
   password="YourPasswordHere"
   database="contact_book"
   ```

4. **Run the script:**

   ```bash
   python contact_book.py
   ```

---

## 🧪 How It Works

### ✅ Add Contact

Prompts the user for name, phone, and email and inserts the data into the database.

### 📋 Display Contacts

Fetches and displays all contact records.

### 🔍 Search Contact

Searches for a contact by name and returns the first match if found.

### ❌ Delete Contact

Deletes a contact based on the name entered by the user.

---

## 🔐 Note

Ensure your MySQL server is running, and the credentials you use in `get_connection()` are correct. It's advised **not to hard-code passwords** for production use — consider using environment variables or config files.

---

## 📬 Contact

**Developer**: Harshal Nikhade
📫 Feel free to reach out for any suggestions or collaborations!
