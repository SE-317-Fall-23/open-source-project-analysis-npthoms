# Assignment Submission

## Project Selected: <Enter project name>

## I. Introduction
- Briefly introduce the purpose of this section, which is to provide a detailed description of two test cases in the selected open-source project.
-I'll be analysing test cases from the javascript program TodoMVC. TodoMVC provides multiple implementations of a to-do list application in various JavaScript frameworks, offering a valuable case study for testing practices.


## II. Test Case 1: [No ToDos]
### A. Description
- This test is designed verify that the program does not load in headers and footers for the page when there are no todos in the list.
### B. Gherkin Syntax (if applicable)
- If you choose to use Gherkin syntax, write the Gherkin scenario for this test case.
### C. Test Steps
- Enumerate the sequence of steps or actions involved in the test case.
1. Assert that there are no items in the list. 
2. Assert that there is no header.
3. Assert that there is no footer.
### D. Code Segments Under Test
- Identify specific code segments or functions that are being tested in this case.

```Java
//              testOps.assertItemCount(0);
//			    testOps.assertMainSectionVisibility(false);
//              testOps.assertFooterVisibility(false)
```
### E. Initial State
- Describe the initial state or conditions of the system or component before executing the test.
- The system is waiting for the initializaton of a new page
### F. Transition
- Explain the actions or events that trigger a change in the system's state.
- The state of the system changes when a page is loaded with and empty list. The change is in the appearance of the page.
### G. Expected State
- The expected state is there should be no list, no header, and no footer.

## III. Test Case 2: [New ToDo]
### A. Description
- Provide a concise overview of the purpose of the second test case.
- This purpose of the test case is to make sure the program is properly adding new "todo" items to the list.
### B. Gherkin Syntax (if applicable)
- If you choose to use Gherkin syntax, write the Gherkin scenario for this test case.
### C. Test Steps
- Enumerate the sequence of steps or actions involved in this test case.
1. Initialization of the browser page.
2. Add item to the list
3. Assert that the item is in the list
4. Add item to the list 
5. Assert that  the item is in the list
### D. Code Segments Under Test
- Identify specific code segments or functions that are being tested in this case.
```Java
// page.enterItem(TODO_ITEM_ONE);
// testOps.assertItems([TODO_ITEM_ONE]);
// page.enterItem(TODO_ITEM_TWO);
// testOps.assertItems([TODO_ITEM_ONE, TODO_ITEM_TWO])Enter code
```
### E. Initial State
- Describe the initial state or conditions of the system or component before executing the test.
- The system initializes a new page.
### F. Transition
- An item is added to the list.
### G. Expected State
- Clearly outline the expected state or outcome after the test steps have been completed.
- The expected outcome is that there is a new item in the todo list. This test case happens twice within the test.

