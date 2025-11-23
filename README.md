# OOPS-Mini-Project
A C++ OOP-based simulation of a virtual human whose emotions and physical states change dynamically with user actions. Features inheritance, polymorphism, abstraction, encapsulation, and real-time stat updates.
# 🌟 Virtual Human With Emotions — OOP Mini Project (C++)

This project is a console-based simulation that models a **virtual human whose emotions and physical states change dynamically** based on user-selected activities. It demonstrates full implementation of **Object-Oriented Programming (OOP)** concepts in C++.

## 🎯 Project Overview

The system allows the user to choose a human type — **Student** or **Employee** — and then control their daily activities such as eating, sleeping, working, relaxing, or socializing. Each action updates emotional and physical metrics including:
- Energy  
- Hunger  
- Happiness  
- Stress  
- Social life  
- Health  

The simulation uses **inheritance**, **polymorphism**, **encapsulation**, and **abstraction**, making it a complete OOP-based project.
## 🧠 Key OOP Concepts Used
### **1. Abstraction**
The `Human` base class defines common behaviors, and `work()` is declared as a pure virtual function.
### **2. Inheritance**
- `Student` → inherits from `Human`  
- `Employee` → inherits from `Human`
### **3. Polymorphism**
`work()` and `showStatus()` are overridden in derived classes to provide role-specific behavior.
### **4. Encapsulation**
All state variables (energy, hunger, stress, etc.) are private, updated through methods like `updateStats()`.

## 🏗️ System Architecture

### **Base Class: Human**
**Attributes:**
- name  
- energy  
- hunger  
- happiness  
- social  
- health  
- stress  

**Methods:**
- eat()  
- sleep()  
- relax()  
- socialize()  
- updateStats()  
- showStatus()  
- work() *(abstract)*  

### **Derived Class: Student**
Additional attribute:
- knowledge  
Overrides:
- work()  
- showStatus()  

### **Derived Class: Employee**
Additional attribute:
- salary  
Overrides:
- work()  
- showStatus()  

## 🔄 System Workflow
The program follows a simulation loop:
1. User enters name  
2. User selects character type (Student / Employee)  
3. Base stats are initialized  
4. Menu appears:  
   - Eat  
   - Sleep  
   - Relax  
   - Socialize  
   - Work  
   - Show Status  
   - Exit  
5. System updates stats dynamically  
6. Time progresses; days change  
7. Loop continues until exit  

A UML workflow diagram for this process is included in the `/diagrams` directory.

## 🛠️ Implementation Details
**Language:** C++  
**Key features from the project report:**
- Virtual functions  
- Dynamic memory allocation (`Human* person = new ...`)  
- Input validation (`cin.clear` / `cin.ignore`)  
- Utility functions:  
  - `clamp()`  
  - `drawBar()`  
  - `formatTime()`  
  - `getTimeOfDay()`  

## 🧪 Results & Discussion
- Emotional and physical states update realistically  
- Students grow in **knowledge**, employees increase **salary**  
- Bar-style UI improves readability  
- Time-of-day simulation enhances realism  
- Input validation prevents errors
  
## 🚀 Future Enhancements
- Build a GUI or convert into a web app  
- Add more roles (Doctor, Gamer, Athlete)  
- Achievements, leveling system, inventory  
- AI-based emotion prediction  
- Sound effects or animations
  
## 🎓 Learning Outcomes
- Build complete OOP architecture  
- Use inheritance & polymorphism effectively  
- Manage multiple dynamic attributes  
- Create time-based simulations  
- Structure large C++ programs cleanly  
- Model real-world systems using OOP  

## 📚 References
- B. Stroustrup — *The C++ Programming Language*  
- R. Lafore — *Object-Oriented Programming in C++*  
- GeeksforGeeks — C++ OOP Concepts  

