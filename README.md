# CampusConnect – A Java OOP Based Academic Profile System

**CampusConnect** is a lightweight console-based application designed using **Core Java** and **Object-Oriented Programming (OOP)** principles. It models a real-world academic environment by managing student profiles based on their level of study: Bachelor’s, Master’s, and PhD.

## 🚀 Features

- Object-Oriented design using **abstraction**, **inheritance**, **interfaces**, and **polymorphism**
- Individual handling for:
  - **Bachelor students** (with project work)
  - **Master students** (with conference participation)
  - **PhD students** (with conferences + published articles)
- Modular code for easy extension and testing
- Accurate total score calculation based on unique student types

## 📦 Code Structure

- `Student` *(abstract class)*: Common fields like `id`, `midterm`, `final`, and score calculation base
- Interfaces:
  - `ProjectScoreBehaviour`
  - `ConferenceScoreBehaviour`
  - `ArticleScoreBehaviour`
- Inheriting classes:
  - `BachelorStudent`
  - `MasterStudent`
  - `PhDStudent`
- `CampusConnectApp`: The entry point that simulates creation and scoring of different student types

## 🧪 Sample Output

```plaintext
[CampusConnect Academic Report]

🎓 Bachelor Student
ID: 1025727
Midterm: 70.0 | Final: 80.0 | Project: 20.0
Total Score: 96.0

🎓 Master Student
ID: 5683429
Midterm: 90.0 | Final: 80.0 | Conferences: 2 (10.0 pts)
Total Score: 94.0

🎓 PhD Student
ID: 8976541
Midterm: 80.0 | Final: 70.0 | Conferences: 6 (30.0 pts) | Articles: 3 (24.0 pts)
Total Score: 98.0
