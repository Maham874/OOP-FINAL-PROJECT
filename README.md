### BY MAHAM MUSTAFA __ 25K-0764
# PROJECT TITLE: FUNDWISE SCHOLARSHIP MANAGEMENT SYSTEM
## Project Description

FundWise is a console-based Scholarship Management System developed in C++. It is designed to help manage student applicants and distribute financial aid based on academic performance (CGPA) and financial need (income).

The system supports two type of users:

* Admin → Manages applicants and scholarship distribution
* Applicant → Views profile and pays installments

The system uses Object Oriented Programming (OOP) concepts along with file handling to store and review data.

---

##  Group Members

* Maham Mustafa (25k-0764)
* Fatima Javed (25k-0594)
* Osailah Atif (25k-0789)

---

## USE CASES
## Admin Use Cases
### 1. Add Applicant
Admin enters applicant details such as ID, name, age, CGPA, income, field, username, and password.
The system checks whether the CGPA is valid (between 0 and 4). If valid, a new applicant is created and stored in the system with status “Pending.”

### 2. Update Applicant Information
Admin enters the applicant ID and updates CGPA and income.
The system searches for the applicant, updates the data, and recalculates the eligibility score.

### 3. Delete Applicant
Admin provides an applicant ID to remove.
The system finds the applicant, deletes the record, and removes it from the list permanently.

### 4. Search Applicants
Admin can search applicants based on CGPA, income, status, or eligibility score.
The system checks all stored applicants and displays those that match the given condition.

### 5. Disburse Scholarship Funds
Admin enters applicant ID and scholarship amount.
The system assigns funds to the applicant and updates the status to “Approved.”

### 6. View Eligible Applicants
Admin checks applicants with high eligibility scores.
The system displays applicants whose score is greater than 80.

## Applicant Use Cases
### 1. Applicant Login
Applicant enters username and password.
The system verifies credentials and grants access to the dashboard if correct.
### 2. View Profile
Applicant selects the option to view profile.
The system displays personal, academic, and financial details including status and score.
### 3. Check Scholarship Status
Applicant views their current status.
The system shows whether the status is Pending, Approved, or Completed.
### 4. Pay Installment
Applicant chooses to pay an installment.
The system increases the installment count. After 4 installments, the status becomes “Completed.”
### 5. Track Funds 
Applicant can see the total scholarship amount received.
The system displays the assigned funds.
### 6. Logout
Applicant exits the dashboard.
The system ends the session and returns to the main menu.

## How to Compile The Project
1. Open **Visual Studio**
2. Create a new **Empty C++ Project**
3.  Add the following files:
`
main.cpp, System.cpp, System.h, Applicant.cpp, Applicant.h, Admin.cpp, Admin.h and User.cpp
`
4. Make sure all files are placed under the same project folder
5. Press `Ctrl + Shift + B` to build the solution
---

## How to Run The Project
**1.** After successful compilation, run the project using:
`
Ctrl + 5
`

**2.**  A console window will appear showing the main menu.

**3.**  On the first run:
* No data will exist initially
* The system starts fresh

**4.** After adding applicant records and closing the program:
  * A file named ```applicants.txt``` will automatically be created in the project folder
  * All data will be stored in this file

**5.** On future executions:
  * The system will automatically load data from ```applicants.txt```
  * Previously saved records will be restored
---

## How to Use The System

### 1. Start The Program
* Run the executable file
* The main menu will appear

### 2. Login Selection
You will be asked to choose user type:
* **Admin Login**
*  **Applicant Login**
### 3. Admin Workflow
If logged in as Admin:
* Enter username: `admin`
* Enter password: `123`

 Then access admin dashboard:
  - Add new applicants
  - Update applicant records
  - Delete applicants
  - Search applicants using filters
  - View eligible candidates ( score > 80)
  - Disburse scholarship funds
### 4. Applicant Workflow
If logged in as applicant:
* Enter registered username and password
Then access applicant dashboard:
- View personal profile
- Check scholarship status
- Pay installments
- Track scholarship funds
- Logout from system
### 5. System Navigation
* Use numeric menu options (1,2,3...)
* Follow on-screen instructions carefully
* Invalid inputs will be rejected with error messages
---

## Assumptions And Limitations
* CGPA must be between 0.0 and 4.0 and the system will reject any value outside this range
* Each applicant is allowed exactly 4 installment payments and after the 4th payment the status is automatically set to Completed
* Admin login credentials are fixed at username admin and password 123 and cannot be changed from within the program
* The system runs entirely in the console and there is no graphical interface
* All data is stored in a plain text file called applicants.txt which is created automatically on the first save
* Passwords are stored as plain text and there is no encryption applied

## File Structure

* `User`  → Base class for all users
* `Admin` → Handles administrative operations
* `Applicant` → Manages student data and scholarship logic
* `System` → Core controller of the program
* `main.cpp` → Entry point of application

---
