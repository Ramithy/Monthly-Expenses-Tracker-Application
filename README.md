# Monthly-Expenses-Tracker-Application
Problem Statement
David, a young professional in a fast-paced city, needs a tool to effectively manage his monthly expenses and savings. He struggles with overspending and keeping track of his finances. This project aims to develop a user-friendly front-end application that helps users like David monitor their monthly income, expenses, and savings, providing insights into their spending habits.

Technical Specifications
Tech Stack
Front-end: Angular
Front-end Port: 8081
Implementation Details
UtilsService
UtilsService: Create a service named UtilsService that implements the sum function. This function will calculate the total monthly income and expenditure.
FormComponent
FormComponent: An Angular component for the input form to add income and expenses.
handleSubmit: Captures form values such as ID, type (income or expense), description, and value (a number).
Resets the form after submission and sets the focus to the description input.
onSubmit should not be called if descriptionInput is null.
Create a variable isButtonDisabled and set its value based on whether the description or value fields are empty. Use this variable to disable the submit button when necessary.
TransactionListComponent
TransactionListComponent: An Angular component to display lists of income and expenditures.
Implements functionality to render these lists correctly.
Provides a way to delete items when needed.
TransactionItemComponent
TransactionItemComponent: An Angular component to display individual income and expenditure items.
Implements functionality to render these items correctly.
Provides a way to delete individual items.
AppComponent
AppComponent: The main Angular component that includes FormComponent and TransactionListComponent within its template.
Sample Output
Create templates and stylesheets to match the provided sample output for adding income and expenses with descriptions and values.
Folder Structure
Follow the below folder structure for the Angular application:

angularapp
src/
app/
utils/
utils.service.ts (UtilsService)
form/
form.component.ts (FormComponent)
form.component.html
form.component.css
transaction-list/
transaction-list.component.ts (TransactionListComponent)
transaction-list.component.html
transaction-list.component.css
transaction-item/
transaction-item.component.ts (TransactionItemComponent)
transaction-item.component.html
transaction-item.component.css
app.component.ts (AppComponent)
app.component.html
app.component.css
index.html
styles.css
Platform Instructions
Step 1
Open the terminal and enter the following command to use Node.js version 14:
nvm use 14
Navigate to the angularapp folder:
cd angularapp
Install Node Modules:
npm install
Step 2
Write the code inside the src folder.
Create the necessary components as outlined in the folder structure.
Step 3
To run the project, use the following command:
npm start
