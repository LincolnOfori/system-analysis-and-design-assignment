# Patient Care User Stories


## User Story 1: View Medical Record

**As a** patient
**I want to** view my medical record
**So that** I can access my health information when needed.

### Acceptance Criteria

```gherkin
Scenario: Patient views their medical record

Given a patient is registered in the system
And the patient has an existing medical record
When the patient requests to view their medical record
Then the system should display the patient's available medical information
And the system should display the medical record to the authenticated patient
```


## User Story 1: Receive Lab Test Results

**As a** patient
**I want to** view my lab test results
**So that** I can know the outcome of my medical tests.

### Acceptance Criteria

```gherkin id="b9u6qz"
Scenario: Patient views an available lab test result

Given a patient has completed a lab test
And the lab test result is available in the system
When the patient requests to view the result
Then the system should display the patient's lab test result
And display the date of the test
And allow the patient to view the result securely
```


