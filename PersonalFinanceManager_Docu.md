# PERSONAL FINANCE MANAGER 
Group Name: GROUP_PersonalFinanceManager

Project Title: Personal Finance Manager

Group Members:

•Chang, Noesa Mae E.

•Coniaro, Joanna Mae M. 

•Lagrimas, Shane Eisley

•Tiozon, Mary Joy

## Introduction
   In today’s fast-paced world, managing personal finances has become more crucial than ever. 
A Personal Finance Manager (PFM) serves as an essential tool for individuals seeking to take control of their financial health. This innovative software or application helps users track their income, expenses, savings, and investments, providing a comprehensive overview of their financial situation. By offering features such as budgeting tools, expense tracking, and financial goal setting, a PFM empowers users to make informed decisions, optimize their spending habits, and plan for a secure financial future. Whether you are looking to save for a major purchase, pay off debt, or simply gain a clearer understanding of your financial landscape, a Personal Finance Manager can be your trusted companion on the journey to financial well-being.

## Project Features and Characteristics

### BUDGETING: Centralized Financial Tracking
• Income & Expenses: You may automatically track your income and expenses by entering your bank account information and credit card information into finance manager apps or internet tools. Without the need for manual updates, this real-time data tracking provides a clear perspective of your financial status.

• Categories: With the help of these tools, you can precisely track where your money is going by categorizing your transactions (such as food, rent, and entertainment). If necessary, you can usually establish your own unique categories in apps.
Setting a Budget

• Budget Creation: Each category can have a budget that you determine depending on your income and financial objectives. The app promotes better money management by assisting you in setting reasonable sp ending caps in several areas.

#### Visual Insights:
• Graphs & Charts: These apps usually give you a visual depiction of your spending habits, such as charts that plot your expenditure over time in different categories. This facilitates the identification of patterns, such as excessive spending on entertainment or eating out.

#### Goal Setting & Saving
• Savings Goals: You can set up specific financial goals, like saving for an emergency fund, a vacation, or a big purchase. The app will track your progress and give you insights into how much more you need to save or how you can adjust your spending to meet your goals faster.
Debt Management
• Debt Tracking: You can monitor your credit card balances, loans, and other bills with the aid of several finance apps. They can help you stay on track with debt payback by suggesting the best payment plans, such as the debt snowball or avalanche approach.

### REPORTS: 
• Health Reports: Numerous tools produce comprehensive reports that provide you with a thorough overview of your financial situation at any given time, such as spending summaries and cash flow statements.

• Record Transactions: Ensure that every transaction (both income and expense) is logged into the app. If your app is linked to your bank accounts or credit cards, transactions will be updated automatically. If not, manually input the data.

• Categorize Expenses: Assign each transaction to the appropriate category (e.g., groceries, rent, utilities, etc.). This will help you see where your money goes daily.
Check Budget vs. Actual Spending: Review your weekly spending in comparison to the budget you’ve set for each category. Are you under or over your planned spending? Adjust your habits if necessary.

• Analyze Categories: See which categories you’re overspending in and consider areas where you can cut back. This could reveal trends such as overspending on non-essential items.
Note Income Fluctuations: If you have irregular income, log and analyze any changes weekly to understand cash flow better.

### SEARCH: 
Access Anywhere Browser-based tools or mobile apps let you access your financial information from anywhere, making budgeting easy whether you're at home or on the go.

### SECURITY: 
• Logout or Timeout: After reviewing your data, you can manually log out or rely on the app's auto-logout feature for security.
Data protection: To guarantee the safety of your financial data, the majority of finance apps use bank-level encryption and other security features.

### USER LOGGING: 
Once logged in, you’ll likely be taken to a dashboard. This is the main hub where you can see a snapshot of your financial situation:

• Account Balances: View balances from linked bank accounts, credit cards, and investment accounts.
•Income vs. Expenses: Get a quick summary of your total income and total expenses for the current month.
Budget Overview: See how much you’ve spent in each budget category and how much you have remaining.

### USER AUTHENTICATION:
• Username/Email & Password: Enter your credentials, such as your email or username and password.
• Two-Factor Authentication (2FA): Many apps offer an additional layer of security with two-factor authentication. You’ll need to verify your login via a text message, email, or authentication app.

### NOTIFICATION: 
• Automatic Alerts: Notifications are frequently sent by finance manager software when you're getting close to or over budget in a particular category. This enables you to monitor your spending and make necessary adjustments.
• Spending Alerts: If you’re approaching your budget limit in any category, many apps will alert you immediately upon login.

## Project Scope
-User friendly:
-Enable users to track their budget and expenses: they can easily track their inserted amount of money inside their account real-time
-Offers budget tips for the users: the system will pop up some offers to the users while exploring the site
-Ensure data security and privacy: QR codes are implemented for more secured account

## Work breakdown Structure

### Level 1: Project Scope
•Personal Finance Manager

### Level 2: Major Deliverables
•User Interface
•Backend System
•Data Management
•Testing and Quality Assurance
•Deployment and Maintenance

### Level 3: Detailed Tasks

## User Interface
•Design user interface (UI) mockups
•Develop UI components
•Implement user interactions and navigation
•Create responsive design for mobile and desktop

## Backend System
•Design database schema
•Develop backend logic and APIs
•Integrate with payment gateways (if applicable)

## Data Management 
•Data validation and cleansing
•Data storage and retrieval
•Data backup and recovery
•Data analytics and reporting

## Testing and Quality Assurance
•Unit Testing
•Integration Testing
•System Testing
•User acceptance testing (UAT)
•Quality assurance processes

## Deployment and Maintenance 
•Deployment planning
•System development
•Post-deployment support
•Ongoing maintenance and updates

## Functional Requirements

        1. User Requirements (what the users wants to be featured in the system)
        -more secured account
        -no limitation of inputting amount of money in the system
        -expense tracker
        -dashboard
        -income management and personal goals
        -user support
        -data managements
   

        2. Use case

        ![image](https://github.com/user-attachments/assets/e8d26b28-0da1-4fa1-95a0-68d3f05de9fc)



## Database Architecture

  1. Data Dictionary
     
      USER_TABLE
     ---------------------------------------------------------
     | FIELD NAME | DESCRIPTION | DATA TYPE | LENGTH | SAMPLE |
     | ---------  |  ---------- | --------- | ------ | ------ |
     | UserID (Primary Key) | Unique identifier for each | VARCHAR  | 50 | A-0001 |  
     | Username | User's chosen name for login. | VARCHAR | 225 | Admin |
     | Password | Encrypted password for security. | VARCHAR | 255 | AD1234 |
     | Email | User's email address. | VARCHAR | 255 | admin@gmail.com | 
     | CreatedDate  | The date and time when the user account was created. | DATETIME |  | 2024-08-30 00:00:00 |
     | LastLogin | The last date and time the user logged in. | DATETIME |   | 2024-08-30 00:00:00 |


      ACCOUNT_TABLE
      ---------------------------------------------------------
     | FIELD NAME | DESCRIPTION | DATA TYPE | LENGTH | SAMPLE |
     | ---------  |  ---------- | --------- | ------ | ------ |
     | AccountID (Primary Key) | Unique identifier for each account. | VARCHAR  | 50 | A-0002 | 
     | UserID (Foreign Key)| Links to the Users table. | VAECHAR | 255 | A-0001  |  
     | AccountName | Name of the financial account (e.g., Savings, Checking). | VARCHAR | 255 | John |
     | Balance |  Current balance of the account. | DECIMAL | 15,2 | 10,000.50 |
     | Currency | Currency code (e.g., USD, EUR). | VARCHAR | 3 | PH |
     | CreatedDate | The date when the account was added. | DATETIME |  | 2024-08-30 00:00:00 |


     TRANSACTIONS_TABLE
     ----------------------------------------------------------
     | FIELD NAME | DESCRIPTION | DATA TYPE | LENGTH | SAMPLE |
     | ---------  |  ---------- | --------- | ------ | ------ |
     | TransactionID (Primary Key)|  Unique identifier for each transaction. | VARCHAR  | 50 | TRAN-0001 | 
     | AccountID (Foreign Key) | Links to the Accounts table. | VARCHAR  | 50 | A-0002 |
     | TransactionDate | The date and time when the transaction occurred. | DATETIME |  | 2024-08-30 00:00:00 |
     | Amount | The amount of money involved in the transaction. | DECIMAL | 15,2 | 10,000.50 |
     | TransactionType | Type of transaction (e.g., Debit, Credit). | VARCHAR | 10  | Debit |
     | CategoryID (Foreign Key)| Links to the Categories table. | VARCHAR | 255 | CATEG-0001  | 
     | Description | Details or notes about the transaction. | VAECHAR | 255 | Balance |


     CATEGORIES_TABLE
     ----------------------------------------------------------
     | FIELD NAME | DESCRIPTION | DATA TYPE | LENGTH | SAMPLE |
     | ---------  |  ---------- | --------- | ------ | ------ |
     | CategoryID (Primary Key) |  Unique identifier for each category. | VARCHAR | 255 | CATEG-0001  |
     | UserID (Foreign Key)| Links to the Users table. | VARCHAR  | 50 | A-0001 |
     | CategoryName | Name of the category (e.g., Groceries, Utilities). | VARCHAR | 255  | Groceries |
     | CategoryType | Type of category (e.g., Income, Expense). | VARCHAR | 255  | Expense |


     BUDGETS_TABLE 
      ----------------------------------------------------------
     | FIELD NAME | DESCRIPTION | DATA TYPE | LENGTH | SAMPLE |
     | ---------  |  ---------- | --------- | ------ | ------ |
     | BudgetID (Primary Key) | Unique identifier for each budget. |  VARCHAR  | 50 | Budg-0001 |
     | UserID (Foreign Key) | Links to the Users table. | VARCHAR  | 50 | A-0001 |
     | CategoryID (Foreign Key) | Links to the Categories table. | VARCHAR | 255 | CATEG-0001  |
     | BudgetAmount | The allocated amount for the budget. | DECIMAL | 15,2 | 10,000.50 |
     | StartDate | The start date for the budget period. | DATETIME |  | 2024-08-30|
     | EndDate | The end date for the budget period. | DATETIME  |  | 2024-08-30|


     GOAL_TABLE
     ----------------------------------------------------------
     | FIELD NAME | DESCRIPTION | DATA TYPE | LENGTH | SAMPLE |
     | ---------  |  ---------- | --------- | ------ | ------ |
     | GoalID (Primary Key) | Unique identifier for each goal. | VARCHAR  | 50 | GOAL-0001 |
     | UserID (Foreign Key)| Links to the Users table. | VARCHAR  | 50 | A-0001 |
     | TargetAmount | The total amount aimed for the goal. | DECIMAL | 15,2 | 10,000.50 |
     | CurrentAmount | The amount already saved or invested towards the goal. | DECIMAL | 15,2 | 10,000.50 |
     | TargetDate | The date by which the goal should be achieved. |  DECIMAL | 15,2 | 10,000.50 |

     
     REPORTS_TABLE
     ----------------------------------------------------------
     | FIELD NAME | DESCRIPTION | DATA TYPE | LENGTH | SAMPLE |
     | ---------  |  ---------- | --------- | ------ | ------ |
     | ReportID (Primary Key) | Unique identifier for each report. | VARCHAR  | 50 | RE-0001 |
     | UserID (Foreign Key)| Links to the Users table. | VARCHAR  | 50 | A-0001 |
     | ReportType | Type of report (e.g., Monthly, Annual). | VARCHAR  | 255 | Monthly |
     | GeneratedDate | The date when the report was generated. | DATETIME |  | 2024-08-30 00:00:00 |
     | ReportData | Serialized data of the report content. | TEXT | 500 | report context |
     
   
  3. ERD
   https://drive.google.com/file/d/1FPX-ZkL_OVnOiXapxt3KsNd4oiah_0EO/view?usp=sharing


     
