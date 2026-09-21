# Patient Care User Stories

## User Story 1: View Medical Record

**As a** patient
**I want to** view my medical record
**So that** I can access my health information when needed.

### Acceptance Criteria

```gherkin
Scenario: Patient views their medical record

Given a patient is registered in the healthcare system
And the patient has an existing medical record
When the patient requests to view their medical record
Then the system should display the patient's available medical information
And the system should only allow the authenticated patient to view the record
```

## User Story 2: Cancel an Appointment

**As a** patient
**I want to** cancel my appointment
**So that** I can free the appointment slot when I am no longer available.

### Acceptance Criteria

```gherkin
Scenario: Patient cancels a scheduled appointment

Given a patient has a scheduled appointment
When the patient selects the appointment and confirms the cancellation
Then the system should cancel the appointment
And update the appointment status to "Cancelled"
And display a confirmation message to the patient
```
