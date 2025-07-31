# 🔬 mabl-hands-on-tests
End-to-end Mabl test flows with real-world scenarios, Including test steps, test reports and learning notes.  
Used this for testing: [OrangeHRM Demo Application](https://opensource-demo.orangehrmlive.com/) 

### 🧩 Testing types 
- **Web**: End-to-end UI flows such as login, navigation, and form submission.
- **Web + API (Hybrid)**: API values captured and reused in UI validations  
  *(e.g., Fetching email from API and validating in logged-in UI state)*.
- **API**: API endpoint testing including status code validation, response body checks,  
  and variable extraction for downstream tests.


## ⚙️ Test Design & Workflow

1. 🗂️ **Test Plan Setup**
   - Created a new **Ad hoc test plan** in Mabl.
   - Tagged test cases for easy filtering (e.g., `smoke`, `Add user`, `API validation`).

2. 🌐 **Environment & Branching**
   - Tests executed in a dedicated **QA environment**.
   - Used a separate **QA branch** for test development.

3. 🧪  **Test Case Variables**
   - Used dynamic variables like `{{userName}}`, `{{password}}`, and `{{app.url}}` for reusability.
   - **Captured variables dynamically from API responses** and reused them in UI flows for validation  
     *(e.g., Fetch email from API → use in login form → assert in dashboard)*.

4. 🔁 **Data-Driven Testing**
   - Inputs were parameterized to test different data sets efficiently.

5. 🧠 **Conditional Logic**
   - Implemented **if-else** statements to make decisions based on application state (e.g., presence of emergency contact).

6. ☁️ **Execution Layers**
   - All tests were first validated **locally**.
   - Followed by execution in **Mabl Cloud** to generate reports and logs.
