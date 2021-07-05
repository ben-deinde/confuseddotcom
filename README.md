-----------------------
# confuseddotcom
-----------------------
Test automation exercise for a database of computer names

This project repo was created to use test automation scripts
to check three features of the Computer Database at
http://computer-database.herokuapp.com/

# Tools

- IDE - Microsoft Visual Studio
- Automation API - Selenium WebDriver
- BDD interpreter - Specflow
- Coding language - C#

# User Guide

The repo has the project files
- computerdatabase.feature
- computerdatabase.feature.cs
- computerdatabaseSteps.cs
- SpecRun.Runner 3.9.7
- SpecFlow.MsTest 3.9.8
- SpecFlow 3.9.8
- Selenium.WebDriver 3.141.0
- Selenium.Support 3.141.0
- MSTest.TestFramework 2.2.5

1. Open the confuseddotcom solution in your IDE
2. There are three tests:
- AddANewComputerToTheDatabase
- DeleteAComputerFromTheDatabase
- SearchForAComputerByName
3. To run all 3 tests, click on Run All
4. To run individual test, select the test to run (rightclick) and run selected test

# AddANewComputerToTheDatabase
This script accesses the database frontend URL and clicks the Add Computer button. It inputs into the text fields valid entries and selects an option from the dropdownlist. Then it  clicks the Create Computer button and verifies that the notification on the page confirms successful addition of computer name to database. With this successful confirmation, the script closes the web browser session.

# DeleteAComputerFromTheDatabase
This script accesses the database frontend URL and searches for a listed computer. If the search finds the desired computer, the script selects it for deletion and clicks the Delete button. After the delete action, the script verifies the notification on the page to confirm successful deletion and closes the browser session.

# SearchForAComputerByName
This script opens up a new browser session and accesses the database frontend. It makes entry into the search field and clicks the search button. With the list of computer names revealed, the script verifies this includes the computer searched for. If included, the script closes the browser session.

