# Hosptial_Appointment_System
C++ program provides an efficient and user-friendly solution for managing appointments through a structured class hierarchy, vector storage, and interactive menu options. The incorporation of date and time classes, along with sorting mechanisms, ensures the integrity and accessibility of appointment data within the application.

**Project Overview**:
- **Objective:** Develop a C++ program for managing appointments with different recurrence patterns (Daily, Monthly, Onetime).
- **Storage:** Utilize a vector to maintain a schedule of appointments.
- **User Interface:** Implement an interactive menu system allowing users to add appointments, check appointments for a specific day, save appointments to a file, load appointments from a file, and exit the program.

**Key Features:**
1. **Dynamic Polymorphism:**
   - Utilize polymorphism through the use of a base class (`Appointment`) and derived classes (`Daily`, `Monthly`, `Onetime`) to represent different types of appointments.

2. **User Input and Output:**
   - Implement user-friendly prompts for entering appointment details, including description, date, and time.
   - Display a menu for users to choose options such as adding appointments, checking appointments for a specific day, saving to a file, loading from a file, and quitting the program.

3. **File Handling:**
   - Implement file I/O functionality to save appointments to a file (`save` method) and load appointments from a file (`load` method).

4. **Date and Time Handling:**
   - Implement date and time handling functionalities to accurately represent and check occurrences for appointments.

5. **Memory Management:**
   - Dynamically allocate memory for appointment objects using `new` to ensure proper memory management.
   - Use a vector of pointers (`vector<Appointment*> schedule`) to store different types of appointments in a unified manner.

6. **Modular Design:**
   - Organize the program into separate header and implementation files (`Appointment.h`, `Daily.h`, `Onetime.h`) to promote modularity and code organization.

**Description:**
- The program provides a flexible appointment scheduling system with different recurrence patterns, catering to daily, monthly, and one-time events.
- Users can interact with the program through a menu, choosing options for adding, checking, saving, loading appointments, or quitting the program.
- The code uses object-oriented principles, leveraging dynamic polymorphism to handle appointments of various types in a unified manner.
- File handling functionalities enable users to persist their appointments to a file and reload them when needed.
- Date and time handling ensures accurate representation and checking of appointments, contributing to the program's reliability.
- Memory management practices, such as dynamic allocation and vector usage, contribute to the program's efficiency and scalability.
- The modular design separates different appointment types into distinct classes, promoting code readability and maintainability.


**Testing Overview:**

- **Unit Testing:**
  - Each class (`Appointment`, `Daily`, `Monthly`, `Onetime`) has undergone comprehensive unit testing to ensure individual functionalities work as intended.
  - Testing involves creating instances of each class, calling methods, and verifying the expected outputs.

- **Integration Testing:**
  - The program has been thoroughly tested to ensure seamless integration between different classes and components.
  - Functions that involve collaboration between classes, such as saving and loading appointments, have been rigorously tested for correct data transfer and consistency.

- **Edge Cases:**
  - Testing includes scenarios where appointments are added, checked, saved, and loaded for different days, months, and years.
  - Handling of boundary cases, such as scheduling appointments on the first and last day of a month, has been validated.

- **User Input Handling:**
  - Robust testing has been conducted to ensure that user input is appropriately processed and validated.
  - Invalid inputs, including non-numeric and out-of-range values, have been tested to confirm that the program handles them gracefully.

- **Memory Leak Detection:**
  - Tools like Valgrind or similar memory analysis tools have been used to verify that dynamic memory allocated using `new` is properly released using `delete` to prevent memory leaks.

- **File I/O Consistency:**
  - File saving and loading functionalities have been tested with various combinations of appointments to guarantee consistency and accuracy.
  - Scenarios such as saving an empty schedule and loading from an empty file have been considered.

- **Menu-Driven Interaction:**
  - The interactive menu system has been extensively tested to ensure users can smoothly navigate through the program and execute desired actions.

**Testing Results:**

- **Unit Testing:**
  - All individual classes and methods have passed their respective unit tests.
  - Methods for reading, printing, saving, and loading appointments have been verified for correctness.

- **Integration Testing:**
  - Integration testing has confirmed that different components work seamlessly together.
  - Collaborative functionalities, such as sorting and displaying appointments, have been verified.

- **Edge Cases:**
  - The program handles edge cases gracefully, ensuring accurate results for appointments scheduled on the first and last day of a month, leap years, etc.

- **User Input Handling:**
  - The program effectively validates user input, preventing invalid data from compromising the system.
  - Users are prompted appropriately for re-entry in case of invalid input.

- **Memory Leak Detection:**
  - Memory analysis tools confirm that dynamically allocated memory is appropriately released, preventing memory leaks.

- **File I/O Consistency:**
  - Saving and loading from files have been validated for consistency and correctness across various scenarios.

- **Menu-Driven Interaction:**
  - The menu system allows users to navigate through the program without issues, with all options performing as expected.

**Conclusion:**
The testing process has successfully validated the robustness and correctness of the program, ensuring that it functions reliably in various scenarios and handles different types of appointments as intended.
