### Project Structure

```bash
Project
 ↳ Epic 1..*
  ↳ Feature 1..*
   ↳ User Story 1..*
    ↳ Acceptance Criteria 1..*

Project
 ↳ Epic 1..*
  ↳ Feature 1..*
   ↳ Gherkin Story 1..*
    ↳ Gherkin Test 1..*

Project
 ↳ Module 1..*
  ↳ Service 1..*
   ↳ Library 1..*
    ↳ Class 1..*

Project
 ↳ Job 1..*
  ↳ Phase 1..*
   ↳ Task 1..*
    ↳ Library 1..*
    ↳ Class 1..*
``` 

Each user story with acceptance criteria is defined using Gherkin format (GWT).

### _(TODO) Markdown Embed Code From File (GitHub Action)_

### Sequence Diagram for class creation flow

![AADSDSDAS](./diagrams/classCreateFlow.md)

### Flowchart Service as Request Handler

![](./images/serviceRequestHandler-1.svg)

### Flowchart Service as Event Handler (Event Stream)

![](./images/serviceEventHandler-1.svg)

### Roles (TODO)
- admin
- project admin (PA)
- production manager (PM)
...