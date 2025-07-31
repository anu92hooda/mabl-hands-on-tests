# 🔬 mabl-hands-on-tests
End-to-end Mabl test flows with real-world scenarios, including test reports and detailed learning notes.


## ⚙️ Test Design & Workflow

1. 🗂️ **Test Plan Setup**
   - Created a new **Ad hoc test plan** in Mabl.
   - Tagged test cases for easy filtering (e.g., `smoke`, `Add user`).

2. 🌐 **Environment & Branching**
   - Tests executed in a dedicated **QA environment**.
   - Used a separate **QA branch** for test development.

3. 🧪 **Test Case Variables**
   - Used dynamic variables like `{{userName}}`, `{{password}}`, and `{{app.url}}` to drive reusability.

4. 🔁 **Data-Driven Testing**
   - Inputs were parameterized to test different data sets efficiently.

5. 🧠 **Conditional Logic**
   - Implemented **if-else** statements to make decisions based on application state (e.g., presence of emergency contact).

6. ☁️ **Execution Layers**
   - All tests were first validated **locally**.
   - Followed by execution in **Mabl Cloud** to generate reports and logs.