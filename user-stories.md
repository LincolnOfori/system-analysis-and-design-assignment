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


## User Story 2: Reschedule Appointment

**As a** patient
**I want to** reschedule my appointment
**So that** I can change my appointment time when necessary.

### Acceptance Criteria

```gherkin
Scenario: Patient reschedules an appointment within 24 hours

Given a patient has a scheduled appointment for "2026-10-15T10:00:00Z"
When the patient requests a reschedule to "2026-10-16T14:00:00Z" less than 24 hours before the original time
Then the system should apply a late-change flag
And emit an "AppointmentRescheduled" event to the Notification Service
And display a confirmation message with updated details to the patient
```

