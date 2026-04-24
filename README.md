# 💇 Salon Appointment Scheduler

This project is part of the **freeCodeCamp Relational Database Certification**.

It is an interactive Bash program that uses **PostgreSQL** to manage salon customers and appointments.

---

## 📌 Project Overview

The application allows users to:

* View available salon services
* Select a service
* Enter their phone number
* Register as a new customer (if needed)
* Book an appointment time
* Receive a confirmation message

---

## 🗂️ Database Structure

### 👤 customers

* `customer_id` (Primary Key)
* `phone` (Unique)
* `name`

### ✂️ services

* `service_id` (Primary Key)
* `name`

### 📅 appointments

* `appointment_id` (Primary Key)
* `customer_id` (Foreign Key → customers)
* `service_id` (Foreign Key → services)
* `time`

---

## ⚙️ Technologies Used

* PostgreSQL
* Bash (Shell Scripting)
* SQL

---

## 🚀 Features

* Interactive terminal-based UI
* Prevents duplicate customers using phone number
* Automatically registers new customers
* Stores appointment records
* Displays confirmation messages

---

## 📁 Files Included

* `salon.sh` → Main Bash script
* `salon.sql` → Database dump file

---

## ▶️ How to Run

1. Start PostgreSQL:

```bash
sudo service postgresql start
```

2. Run the program:

```bash
./salon.sh
```

---

## 🧪 Example Usage

```text
1) cut
2) color
3) trim

Select service: 1
Enter phone: 12345
Enter name: Faizan
Enter time: 10:30

I have put you down for a cut at 10:30, Faizan.
```

---

## 🎓 Certification

Completed as part of the **freeCodeCamp Relational Database Certification**.

---

