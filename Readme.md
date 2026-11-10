## Step 1: Define the Test Context

| Section                  | Description                                   |
| ------------------------ | --------------------------------------------- |
| Test objective 1         | Verify that users can successfully create valid bookings using rental selection, dates, and guest information. |
| Test objective 2         | Ensure booking information is accurately displayed and updated in the booking list.               |
| In scope                 | Rental selection, check-in/check-out dates, guest count, booking creation, booking viewing, increase/decrease/reset controls                          |
| Out of scope             | Payment processing, user authentication, third-party integrations      |
| Test Basis               | Requirements documents, user stories, UI designs, source code    |
| Assumption/constraint    | Testing must be completed within one week before release.      |


## Step 2: Identify Roles and Responsibilities

|       Role        |	    Responsibilities            |	    When Involved       |   	Communication       |
|-------------------|-----------------------------------|---------------------------|---------------------------|
|    Tester	        | Create and execute test cases, report defects	 | Throughout testing |	Developers and Test Lead    |
|    Developer      | Fix defects and verify fixes      |	During defect resolution|	Testers                 |
|    Product Owner  | Validate requirements and approve release readiness |Beginning and end of testing | Tester and Project Team |


## Step 3: Define the Test Approach

|       Test Area	    |       Test Level/Type     |	Technique	                 |   Manual or Automated	    |       Deliverable     |
|-----------------------|---------------------------|--------------------------------|------------------------------|-----------------------|
|   Booking Form        |	Component Testing       |	Boundary Value Analysis	     |      Automated	            | Automated test scripts|
|   Date Validation	    |   Integration Testing	    |   Equivalence Partitioning	 |      Manual	                |   Test cases          |
|  Guest Count Controls	|   System Testing	        |   Boundary Value Analysis	     |      Manual	                |   Test results        |
|   Booking Creation	|   System Testing	        |   Positive and Negative Testing|	    Manual	                |   Defect reports      |
|   Booking List        |	Acceptance Testing      |	User Scenario Testing	     |      Manual	                | Test completion report|

### Test Levels
- Component Testing
- Integration Testing
- System Testing
- User Acceptance Testing (UAT)

### Test Types
- Functional Testing
- Regression Testing

### Test Deliverables
- Test Cases
- Test Results
- Defect Reports
- Coverage Reports
- Test Completion Report

## Step 4: Identify Test Requirements

### Test Environment
- Staging/test environment matching production configuration

### Browsers/Devices
- Google Chrome
- Microsoft Edge
- Firefox
- Mobile browser testing

### Testing Tools
- Jira or GitHub Issues
- Browser Developer Tools
- Test case documentation

### Test Data
- Valid booking dates
- Invalid booking dates
- Various guest counts
- Multiple rental selections

### Access/Permissions
- Tester account
- Developer access to logs and environment

### People/Training
- Tester familiar with booking requirements
- Developer available for defect fixes


## Step 5: Create a Risk Register

|           Risk	                    |    Type      |	Likelihood     |  Impact	|           Mitigation               |
|---------------------------------------|--------------|-------------------|------------|------------------------------------|
| Users can book with invalid dates	    | Product Risk |    Medium	       |    High	| Prioritize date validation testing |
| Guest count controls produce incorrect values | Product Risk | Medium    |	Medium	|  Execute boundary value tests      |
| Test environment becomes unavailable	| Project Risk |	Low     	   |    High	| Verify environment access before testing |
| Defects are not fixed before release	| Project Risk |    Medium	       |    High	| Daily defect review meetings       |

## Step 6: Define Entry Criteria

|   Type	|           Criterion                         |
|-----------|---------------------------------------------|
| Entry	    |Test environment is available and accessible |
| Entry	    | Current release build has been deployed     |
| Entry	    | Test cases have been reviewed and approved  |    
| Entry	    | Test data has been prepared                 |
| Entry	    | Required testing tools are installed        |

## Step 7: Define Exit Criteria

|   Type	|           Criterion                         |
|-----------|---------------------------------------------|
| Exit	    | 100% of planned test cases executed         |
| Exit	    |No critical or high-severity defects remain open |
| Exit	    | All booking creation tests pass             |    
| Exit	    | Regression testing completed successfully   |
| Exit	    | Product Owner approves release readiness    |


## Step 8: Create a Test Schedule

|       Activity        	|   Responsible Role	  |  Time  |    Dependency                |
|---------------------------|-------------------------|--------|------------------------------|
| Review requirements       |	Tester, Product Owner |	Day 1  | Requirements available       |
| Design test cases	        |   Tester	              | Day 2  | Requirements review completed|
| Prepare environment and data |	Tester, Developer |	Day 3  | Test cases completed         |  
| Execute tests             |	    Tester	          | Day 4-5| Environment ready            |
| Fix defects	            |       Developer	      | Day 5-6| Defects identified           |   
| Regression testing	    |       Tester	          | Day 6  | Defect fixes completed       |
| Final review and sign-off	|       Product Owner	  | Day 7  | Testing completed            |


## Step 9: Define the Communication Plan

|   Information	            |   Audience	|   Method	        | Frequency             |
|---------------------------|---------------|-------------------|-----------------------|
| Test progress	            |  Project Team	| Daily Stand-up    |	Daily               |
| Defect reports            |   Developers  | GitHub Issues/Jira|	As defects are found|
| Testing summary           | Product Owner | Email or Meeting  |	End of testing      |
| Release readiness status	|  Project Team | Status Meeting    |	Final day           |