# VotingSystem
# Voting System

## 📌 Project Description

The **Voting System** is a simple Java console-based application developed to demonstrate the basic concepts of Java programming.

The system allows voters to register, view the available candidates, cast their vote, and view the total voting count.

The project also includes input validation to ensure that voters provide valid details before they are allowed to vote.

---

## 🎯 Features

- Register a new voter
- Validate 4-digit Voter ID
- Validate voter name
- Validate voter age
- Display available candidates
- Verify registered voters before voting
- Allow a voter to cast a vote
- Prevent a voter from voting more than once
- Display the total vote count for each candidate
- Exit the application

---

## 🛠️ Technologies Used

- **Programming Language:** Java
- **Java Version:** Java 17
- **IDE:** Eclipse
- **Data Structure:** ArrayList
- **Input:** Scanner
- **Project Type:** Console-based application

---

## 📂 Project Structure

```text
VotingSystem
│
└── VotingSystem.java
```

The program contains:

- `Voter` class – stores voter details
- `Candidate` class – stores candidate details and vote count
- `registerVoter()` – registers voters
- `displayCandidates()` – displays candidates
- `castVote()` – allows voters to cast their vote
- `displayVotingCount()` – displays vote counts

---

## 🔄 Program Flow

```text
START
   ↓
Display Main Menu
   ↓
Register Voter
   ↓
Validate Voter ID
   ↓
Validate Name
   ↓
Validate Age
   ↓
Voter Registration
   ↓
Display Candidates
   ↓
Cast Vote
   ↓
Check Voter ID
   ↓
Check Already Voted
   ↓
Select Candidate
   ↓
Record Vote
   ↓
Display Voting Count
   ↓
Exit
```

---

## ✅ Input Validation

### Voter ID

The voter ID must contain exactly **4 digits**.

Example:

```text
Valid   : 1234
Invalid : 12
Invalid : 12345
```

If an invalid ID is entered:

```text
Invalid Voter ID! ID must contain exactly 4 digits.
```

### Voter Name

The name can contain only **letters and spaces**.

Example:

```text
Valid   : rakshitha
Valid   : Ravi Kumar
Invalid : rak1
Invalid : Ravi@123
```

If an invalid name is entered:

```text
Invalid name! Name can contain only letters and spaces.
```

### Age

The voter must be **older than 18** according to the validation used in this project.

If the voter enters an invalid age:

```text
You are not eligible to vote.
```

---

## 🗳️ Candidates

The application contains four candidates:

| Candidate ID | Candidate Name |
|---|---|
| 1 | Arun |
| 2 | Priya |
| 3 | Rahul |
| 4 | Sneha |

---

## 💻 Sample Output

### Voter Registration

```text
========== VOTER REGISTRATION ==========

Enter 4-digit Voter ID: 12

Invalid Voter ID! ID must contain exactly 4 digits.
```

The user then enters a valid voter ID:

```text
Enter 4-digit Voter ID: 1234
Enter voter name: rak1

Invalid name! Name can contain only letters and spaces.
```

After entering valid details:

```text
Enter 4-digit Voter ID: 1234
Enter voter name: rakshitha
Enter age: 22

Voter registered successfully!
Voter ID : 1234
Name     : rakshitha
Age      : 22
```

---

### Display Candidates

```text
========== CANDIDATES ==========

Candidate ID : 1
Candidate Name : Arun
-----------------------------

Candidate ID : 2
Candidate Name : Priya
-----------------------------

Candidate ID : 3
Candidate Name : Rahul
-----------------------------

Candidate ID : 4
Candidate Name : Sneha
-----------------------------
```

---

### Invalid Voter

When an unregistered voter ID is entered:

```text
========== CAST VOTE ==========

Enter your Voter ID: 1244

Voter not found! Please register first.
```

---

### Successful Voting

After entering a registered voter ID:

```text
Enter your Voter ID: 1234

========== CANDIDATES ==========

Candidate ID : 1
Candidate Name : Arun
-----------------------------

Candidate ID : 2
Candidate Name : Priya
-----------------------------

Candidate ID : 3
Candidate Name : Rahul
-----------------------------

Candidate ID : 4
Candidate Name : Sneha
-----------------------------

Enter Candidate ID: 1

Vote cast successfully!
You voted for: Arun
```

---

### Voting Count

After casting the vote:

```text
========== VOTING COUNT ==========

Arun : 1 votes
Priya : 0 votes
Rahul : 0 votes
Sneha : 0 votes
```

This shows that **Arun received one vote**, while the other candidates have zero votes.

---

## 🔐 Duplicate Voting Prevention

The system keeps track of whether a voter has already voted.

If the same voter tries to vote again, the system displays:

```text
You have already voted!
```

This prevents the same registered voter from casting multiple votes during the current program execution.

---

## 📚 Java Concepts Used

This project demonstrates several basic Java concepts:

- Classes and Objects
- Constructors
- Encapsulation through class fields
- ArrayList
- Scanner
- Methods
- `if-else` statements
- `switch` statement
- `for` loop
- String validation using Regular Expressions
- Boolean values
- User input
- Basic object-oriented programming

---

## ▶️ How to Run the Project

### Step 1
Open the project in **Eclipse**.

### Step 2
Make sure **Java 17** is configured.

### Step 3
Open:

```text
VotingSystem.java
```

### Step 4
Right-click the Java file.

Select:

```text
Run As → Java Application
```

### Step 5
Enter the required details through the console.

---

## 📝 Project Output Summary

The project successfully demonstrates:

1. Voter registration
2. Voter ID validation
3. Name validation
4. Age validation
5. Candidate display
6. Voter verification
7. Vote casting
8. Duplicate voting prevention
9. Vote counting
10. Program termination

---

## 🚀 Future Enhancements

The project can be further improved by adding:

- Database connectivity using MySQL
- Admin login
- Voter login
- Candidate registration
- Persistent voter records
- Persistent voting results
- Search voter functionality
- Delete/update voter functionality
- GUI using Java Swing or JavaFX
- More advanced security and auditing

---

## 👩‍💻 Conclusion

The **Voting System** is a beginner-friendly Java project that demonstrates how Java can be used to develop a simple voting application.

It provides voter registration, input validation, candidate selection, vote casting, duplicate voting prevention, and vote counting through a console-based interface.
