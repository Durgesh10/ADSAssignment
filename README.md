**Introduction:**

This Test Automation Framework is created using Java + Selenium Web Driver + TestNG + Maven. Which can be used across different web based applications. With this framework in place, whenever we need to automate a web based application, we would not need to start from scratch, but use the application independent keyword components to the extent possible and create application specific components for the specific needs.

**Screenshot:**

Most of the time we think to Capture Screenshot in WebDriver when some kind of error or exception surfaces while practicing testing, to resolve the same the framework has a method.
getScreenshot() is used to indicates driver to capture a screenshot and store it in //screenshot/packageName directory.

**Reporting:**

The framework produce index.html report. It resides in the same 'target\surefire-reports' folder. This reports gives the link to all the different component of the TestNG reports like Groups & Reporter Output. On clicking these will display detailed descriptions of execution.
You can find emailable-report.html from target\surefire-reports to email the test reports. As this is a html report you can open it with browser.

**Key Design Elements:**

1. Architecture Layers include Tests, Framework, Selenium Page Objects and Browser.
2. Page Object Pattern - clear seperation of pages versus test cases and represtative of the application.
3. All page classes contructors are called via a Single Generic type of page.
4. Test cases do not include hard coded data, variables or the need to perform instatiation of any object type.
5. Data Generators
6. Base Class which can be extended to handle Initializations before Test Suites are executed.
