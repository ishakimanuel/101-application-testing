# **Application Testing 101 Guide & Example (React Base)**

This repo is created to give you a basic understanding why you should implement unit testing in your [React](https://reactjs.org/) application, by giving you some basic concepts and practical example by using [jest](https://jestjs.io/docs/) and [testing-library](https://testing-library.com/).


### **What is testing ?**
A process to ensure that our application functionality is running as our expected. **(bug free)**

### **Why do we testing ?**

- Building confidence in our code
- Code documentations of applications flow
- Bugs and regression prevention

### **Potential drawbacks**

- Writing tests is time consuming and difficult.
- If done incorrectly, it can bring false positives. Your tests pass, but your app doesn’t functioning as intended.
- Or false negatives. Your tests fail but your app is functioning as intended.

### Levels **of testing**
#### **Unit test (single unit testing)**
Ensures that each part of the code delivers the expected result
- **Function**
    Logic testing of our single function (give output then expect the result)
- **Snapshoot**
    A snapshot test makes sure that the user interface (UI) of a web application does not change unexpectedly. It captures the code of a component at a moment in time, so that we can compare the component in one state with any other possible state it might take. Rules for snashot is using for UI that not often changes and not complex
- **Component**
    Expect component to render / doing something base on our expectation 

#### **Integration Test (Behavior testing)**
 Integration testing is performed to test individual components to check how they function together. In other words, it is performed to test the modules which are working fine individually and do not show bugs when integrated.

#### **End To End Test (All flow testing)**
Testing method that involves testing an application’s workflow from beginning to end. 

### **Implementation**

#### **TDD (Test Driven Development)**
TDD is software development approuch where unit test and testing is define first before the actual code implementation, and as we start code, we are focusing to solve the test case until our test is passed

- **Leads to better application design**
 By writting test case first, we already know what code should we write and have a good reason about our code.

- **Code simplify and time saving** **(less code)**
Reduce uneeded code because we are focusing on solving test case rather than bug's causing from our code and it's saving time because no need to manual testing, and write our test case after coding, because our testing is complete with the code in the same time.  

    | NO TDD | TDD |
    | ------ | ------ |
    | Code ⇒ manual test ⇒ error ⇒ fix ⇒ manual test ⇒ fix ⇒ done ⇒ unit test | Test Case ⇒ error ⇒ fix ⇒ error ⇒ fix ⇒ done  |
   
      
### What should we test ?
- **Test Render / Result**
Test what you expect from the component or function to render or return.
If you are rendering a custom `Button` component and you pass a `color` prop with a value of `red` you should test that. This will also give you confidence that your component meet the design requirements.

- **Test Interaction**
For example if you expect something to happen when you click or hover over a button test 
            
### **Last Step:** **Best Practices**
- [https://github.com/goldbergyoni/javascript-testing-best-practices](https://github.com/goldbergyoni/javascript-testing-best-practices#section-1-the-test-anatomy-1)
- [https://kentcdodds.com/blog/testing-implementation-details/](https://kentcdodds.com/blog/testing-implementation-details/)
- [https://kentcdodds.com/blog/common-mistakes-with-react-testing-library](https://kentcdodds.com/blog/common-mistakes-with-react-testing-library)
