# OOP-FINAL-PROJECT
## Project Description

FundWise is a C++ based console application designed to manage scholarship applications. It allows administrators to manage applicants and distribute funds, while applicants can track their application status and manage installments.

---

##  Group Members

* Maham Mustafa (25k-0764)
* Fatima Javed (25k-0594)
* Osailah Atif (25k-0789)

---

## Use Cases

1. Admin can add new applicants
2. Admin can update applicant academic details
3. Admin can delete applicants
4. Admin can search applicants based on CGPA, income, or status
5. Admin can disburse scholarship funds
6. Applicant can login and view their profile
7. Applicant can pay installments

---

## How to Compile

Using g++:

```
g++ main.cpp System.cpp Applicant.cpp Admin.cpp User.cpp -o app
```

---

## How to Run

```
./app
```

---

## How to Use

1. Run the program

2. Select Login

3. Choose:

   * Admin Login
     Username: admin
     Password: 123

   * Applicant Login
     Use created credentials

4. Follow menu options

---

## Assumptions / Limitations

* Only one admin (hardcoded)
* Data stored in text file (no database)
* Names cannot contain spaces
* Basic console interface only

---

## File Structure

* User → Base class
* Admin → Admin operations
* Applicant → Student data & logic
* System → Core system controller
* main.cpp → Entry point

---
