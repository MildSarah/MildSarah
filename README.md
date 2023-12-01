- 👋 Hi, I’m @Manali Iyengar
- 👀 I’m interested in QA position
- 🌱 
- 💞
- 📫 

<!---
MildSarah/MildSarah is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->



Automated Testing for E-commerce Website
Part 1: Test Planning
Test Strategy Document:
Objectives of Testing:
The primary objectives are to ensure the functionality, usability, and performance of the e-commerce website. Additionally, we aim to identify and mitigate potential risks that could impact the system.

Scope of Testing:
The testing will cover all key features, including user registration, product search, cart management, checkout process, and order management. It includes functional, usability, and performance testing.

Testing Levels:
Unit Testing
Integration Testing
System Testing
Acceptance Testing
Testing Types:
Functional Testing
Usability Testing
Performance Testing
Entry and Exit Criteria:
Entry Criteria:

Completion of development
Availability of test environment
Test data is prepared
Exit Criteria:

No critical or high-severity defects
All planned tests executed successfully
Approval from stakeholders
Test Environment and Tools:
Test Environment: Staging environment replicating the production setup
Testing Tools: Selenium for functional testing, JMeter for performance testing, and JIRA for test management.
Risk Analysis:
Identify potential risks such as third-party integration issues, performance bottlenecks, and security vulnerabilities. Mitigation strategies should be in place.

Test Plan:
Test Deliverables:
Test Strategy Document
Test Cases
Automated Test Scripts
Test Execution Reports
Test Schedule:
Divide testing into phases and allocate time accordingly. Include time for regression testing and retesting.

Test Resources:
Define roles and responsibilities. Ensure access to necessary hardware, software, and testing tools.

Test Data and Environment Setup:
Describe how test data will be generated or obtained. Specify the process for setting up the test environment.

Test Execution and Reporting:
Define the process for executing tests, capturing results, and reporting defects. Specify the frequency and format of test status reports.

Part 2: Test Case Design
Functional Test Cases:
User Registration:
Verify successful user registration with valid details.
Validate error message for incomplete registration form.
Check if existing users are prevented from using the same email for registration.
Product Search:
Verify the search functionality returns relevant results.
Test search using special characters and verify appropriate handling.
Check if the search results page displays correct product details.
Adding Items to Cart:
Confirm that items can be added to the cart from product pages.
Validate the cart total updates accurately when items are added or removed.
Test adding items to the cart from different product categories.
Checkout Process:
Ensure a user can proceed through the checkout process smoothly.
Validate the application handles address validation correctly.
Confirm the order summary is accurate on the checkout page.
Order Management:
Verify the order history displays all past orders for a user.
Test order cancellation functionality.
Validate the order status updates correctly after payment.
Edge and Boundary Test Cases:
User Registration:
Test registration with the maximum allowed characters in the username.
Verify system behavior when registering with an empty password field.
Test registration with the minimum and maximum allowed length for the password.
Product Search:
Search for a product with the shortest possible search query.
Test search with the maximum allowed characters in the search query.
Verify the system's response to an empty search query.
Part 3: Test Automation
Test Automation Framework:
Selenium WebDriver:
Selenium is chosen for its robust cross-browser compatibility and wide community support. Its ability to integrate with various programming languages allows seamless automation of web applications.

Automated Test Scripts:
User Registration:
python
Copy code
# Automation script for user registration
# Test case: Verify successful user registration with valid details.

# Selenium code to open the registration page, fill in details, and submit
...

# Verification steps
assert "Welcome" in driver.title  # Assuming the title changes after successful registration
Product Search:
python
Copy code
# Automation script for product search
# Test case: Verify the search functionality returns relevant results.

# Selenium code to open the search bar, enter a valid search query, and submit
...

# Verification steps
assert len(search_results) > 0  # Assuming search results are displayed
Adding Items to Cart:
python
Copy code
# Automation script for adding items to cart
# Test case: Confirm that items can be added to the cart from product pages.

# Selenium code to navigate to a product page, add item to cart, and navigate to cart
...

# Verification steps
assert cart_total_updated_correctly()  # Assuming there's a function to check cart total
Test Data Management:
Test data will be managed using CSV files. Scripts will read data from these files to simulate various scenarios.

Submission Requirements:
Documentation: Clearly document assumptions and any deviations from the initial plan.
Instructions: Provide clear setup instructions and guidelines for running automated tests.
Configuration Files: Include necessary configuration files in the repository.
Repository: Submit the solution in a version-controlled repository (GitHub) with a link for review.
README: Include a README file with instructions for running tests and additional relevant comments.
Evaluation Criteria:
Clarity and Completeness: Test planning should be clear, comprehensive, and address all specified points.
Test Case Effectiveness: Functional and edge test cases should cover relevant scenarios.
Automated Test Scripts: Scripts should be well-structured, cover positive and negative scenarios, and provide clear verification steps.
Documentation: The README should be comprehensive, including setup instructions and relevant comments.



