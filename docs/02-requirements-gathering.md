# 2. Requirements Gathering

## 2.1 Introduction

Requirements gathering is the process of identifying and documenting the needs, expectations, and constraints of the people who will use or interact with PortfolioGenie.

The purpose of this section is to define the system's stakeholders, user stories, use cases, functional requirements, and non-functional requirements. These requirements will guide the design, implementation, and testing phases.

## 2.2 Stakeholder Analysis

A stakeholder is an individual or organization that can influence the project or be affected by its outcome.

| Stakeholder | Role | Main Needs and Expectations |
|---|---|---|
| Junior Developers | Primary users | Create professional portfolios quickly and easily |
| University Students | Primary users | Showcase academic projects, skills, and education |
| Recent Graduates | Primary users | Present qualifications and projects to potential employers |
| Freelancers | Secondary users | Display services, skills, and previous work |
| Recruiters and Employers | Portfolio visitors | Review candidates' skills and projects efficiently |
| Development Team | Project implementers | Build, integrate, test, and maintain the system |
| Project Supervisor | Academic evaluator | Review progress, requirements, and project quality |
| GitHub | External service provider | Provide authorized access to repository information |
| AI API Provider | External service provider | Process requests for AI-assisted content generation |

## 2.3 User Stories

User stories describe the system's features from the perspective of its users.

| ID | User Story | Priority |
|---|---|---|
| US-01 | As a user, I want to create an account and sign in so that I can access my portfolio data securely. | High |
| US-02 | As a user, I want to add and edit my personal information so that visitors can learn about me. | High |
| US-03 | As a user, I want to add, edit, and delete projects so that I can keep my portfolio updated. | High |
| US-04 | As a user, I want to add my technical skills and education so that visitors can understand my background. | High |
| US-05 | As a user, I want to select a portfolio template so that I can choose a suitable presentation style. | High |
| US-06 | As a user, I want to preview my portfolio before publishing it so that I can check its appearance. | High |
| US-07 | As a user, I want to save my portfolio and return to it later so that I do not lose my work. | High |
| US-08 | As a user, I want AI to help improve my project descriptions so that they are clearer and more professional. | Medium |
| US-09 | As a user, I want AI to help draft an About Me section based on my information so that I can introduce myself effectively. | Medium |
| US-10 | As a user, I want to import selected public GitHub repositories so that I can add my coding projects more efficiently. | Medium |
| US-11 | As a user, I want to review and edit AI-generated or imported content so that I remain in control of my portfolio. | High |
| US-12 | As a user, I want to share a public portfolio link so that others can view my work, if publishing is supported. | Medium |

Priorities should be confirmed with the supervisor and adjusted according to the final project scope.

## 2.4 Use Cases

### UC-01: Create and Manage a Portfolio

**Primary Actor:** Portfolio Owner

**Preconditions:**
- The user has access to the application.
- Authentication is completed if required by the system.

**Main Flow:**
1. The user opens the portfolio builder.
2. The system displays the portfolio creation interface.
3. The user enters personal information, skills, education, and project details.
4. The system validates the entered information.
5. The user selects a template.
6. The system displays a portfolio preview.
7. The user saves the portfolio.
8. The system confirms that the information has been saved.

**Alternative Flow:**
- If required information is missing, the system identifies the incomplete fields.
- If saving fails, the system displays an appropriate error message.

**Postconditions:**
- The portfolio data is saved successfully, or the user receives a clear error message.

### UC-02: Generate AI-Assisted Content

**Primary Actor:** Portfolio Owner

**Preconditions:**
- The AI feature is available.
- The user has provided sufficient information for the requested content.

**Main Flow:**
1. The user opens an AI-assisted content feature.
2. The user selects the content type, such as an About Me section or project description.
3. The system prepares a prompt using the relevant user-provided information.
4. The AI service generates a draft.
5. The system displays the generated content.
6. The user reviews and edits the draft.
7. The user accepts or rejects the suggested content.

**Alternative Flow:**
- If the AI service fails or times out, the system informs the user.
- If the input is insufficient, the system requests additional information.
- The user can continue editing the content manually.

**Postconditions:**
- The user decides whether to use the generated content.

### UC-03: Import GitHub Projects

**Primary Actor:** Portfolio Owner

**Preconditions:**
- GitHub integration is configured.
- The required authorization or access method is available.

**Main Flow:**
1. The user opens the GitHub import feature.
2. The system requests the required GitHub account information or authorization.
3. The system retrieves available repository information.
4. The user reviews the retrieved repositories.
5. The user selects the repositories to import.
6. The system maps supported repository details to portfolio project fields.
7. The user reviews and edits the imported information.
8. The system saves the selected projects.

**Alternative Flow:**
- If access is denied, the system explains that authorization is required.
- If no repositories are available, the system allows manual project entry.
- If the API request fails, the system displays an error message.

**Postconditions:**
- Selected repository information is added to the portfolio after user review.

### UC-04: Preview and Publish a Portfolio

**Primary Actor:** Portfolio Owner

**Preconditions:**
- The user has created a portfolio.
- The selected template is available.

**Main Flow:**
1. The user opens the preview.
2. The system renders the portfolio using the selected template.
3. The user checks the content and layout.
4. The user makes any required changes.
5. The user publishes or shares the portfolio if this feature is implemented.
6. The system provides the resulting public URL.

**Alternative Flow:**
- If required fields are incomplete, the system prompts the user to complete them.
- If publication fails, the system explains the failure and allows the user to retry.

**Postconditions:**
- The portfolio is ready for review or is published successfully, depending on the available functionality.

## 2.5 Functional Requirements

Functional requirements describe what the system must do.

| ID | Requirement | Priority |
|---|---|---|
| FR-01 | The system shall provide account registration and authentication if included in the approved scope. | High |
| FR-02 | The system shall allow users to create a portfolio. | High |
| FR-03 | The system shall allow users to enter and update personal information. | High |
| FR-04 | The system shall allow users to add, edit, and delete projects. | High |
| FR-05 | The system shall allow users to manage technical skills and education. | High |
| FR-06 | The system shall provide a guided, multi-step portfolio creation process. | High |
| FR-07 | The system shall validate required fields and display understandable validation messages. | High |
| FR-08 | The system shall allow users to select from the available portfolio templates. | High |
| FR-09 | The system shall provide a preview of the portfolio before publication. | High |
| FR-10 | The system shall save portfolio data and retrieve it for later editing. | High |
| FR-11 | The system shall generate AI-assisted text for supported content fields. | Medium |
| FR-12 | The system shall allow users to review and edit AI-generated content. | High |
| FR-13 | The system shall retrieve supported public GitHub repository information through the configured integration. | Medium |
| FR-14 | The system shall allow users to review and select repository information before importing it. | Medium |
| FR-15 | The system shall display clear error messages when an external service is unavailable. | High |
| FR-16 | The system shall provide a public portfolio URL if portfolio publishing is implemented. | Medium |
| FR-17 | The system shall restrict access to portfolio editing according to the application's authorization rules. | High |
| FR-18 | The system shall allow users to update their portfolio after saving or publishing it. | High |

## 2.6 Non-Functional Requirements

Non-functional requirements describe the expected quality, performance, and constraints of the system.

### 2.6.1 Performance

| ID | Requirement |
|---|---|
| NFR-01 | Common application pages should load within three seconds under the agreed test conditions. |
| NFR-02 | Saving or retrieving portfolio data should normally complete within two seconds under the agreed test conditions, excluding external service delays. |
| NFR-03 | The interface should remain responsive while AI or GitHub requests are being processed. |
| NFR-04 | The system should display loading indicators for operations that take noticeable time. |

### 2.6.2 Security and Privacy

| ID | Requirement |
|---|---|
| NFR-05 | The system shall protect user data against unauthorized access. |
| NFR-06 | Authentication and authorization shall be implemented appropriately if user accounts are supported. |
| NFR-07 | API keys and other secrets shall not be exposed in public frontend code. |
| NFR-08 | The system shall validate and sanitize user inputs where appropriate. |
| NFR-09 | The system shall request only the external service permissions required for its functionality. |
| NFR-10 | Users shall be informed about the information they choose to publish publicly. |

### 2.6.3 Usability and Accessibility

| ID | Requirement |
|---|---|
| NFR-11 | The interface shall use clear labels and understandable navigation. |
| NFR-12 | The portfolio builder shall provide understandable validation and error messages. |
| NFR-13 | The interface shall support keyboard navigation for essential interactions. |
| NFR-14 | Text and interface elements shall aim to meet WCAG 2.2 AA accessibility guidelines where applicable. |
| NFR-15 | Users shall be able to review and edit AI-generated content before accepting it. |

### 2.6.4 Reliability

| ID | Requirement |
|---|---|
| NFR-16 | The system shall handle API failures without unexpectedly crashing the entire application. |
| NFR-17 | The system shall provide clear feedback when saving or importing information fails. |
| NFR-18 | The system shall preserve saved portfolio information according to the implemented storage design. |
| NFR-19 | The system shall handle missing or incomplete project information gracefully. |

### 2.6.5 Maintainability and Scalability

| ID | Requirement |
|---|---|
| NFR-20 | The source code shall follow consistent naming conventions and project structure. |
| NFR-21 | Reusable components shall be used where appropriate. |
| NFR-22 | Frontend, backend, and external service integration responsibilities should be separated clearly. |
| NFR-23 | Changes to one feature should minimize unnecessary changes to unrelated features. |

### 2.6.6 Compatibility

| ID | Requirement |
|---|---|
| NFR-24 | The application shall support current versions of the agreed target browsers. |
| NFR-25 | The interface shall adapt to desktop, tablet, and mobile screen sizes. |
| NFR-26 | The system shall display a usable interface across the screen sizes included in the testing plan. |

## 2.7 Acceptance Criteria

The requirements will be considered accepted when:

1. Each approved requirement has a unique identifier.
2. Each requirement is clear, testable, and relevant to the project scope.
3. The main user workflows have been reviewed by the team.
4. Functional requirements are mapped to suitable test cases.
5. Non-functional requirements have measurable verification methods where possible.
6. The supervisor has reviewed the requirements where required.

## 2.8 Requirements Validation

The team will validate requirements through:

- Team reviews and discussions.
- Supervisor feedback.
- Wireframe and prototype reviews.
- User story and use case walkthroughs.
- Requirement-to-test-case mapping.
- Updating the requirements when the approved scope changes.

The requirements should be revised throughout development to reflect agreed changes and the final implemented functionality.
