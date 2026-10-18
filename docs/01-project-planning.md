# 1. Project Planning & Management

## 1.1 Project Proposal

### 1.1.1 Project Overview

**PortfolioGenie** is an AI-powered web application designed to help junior developers, students, and recent graduates create professional online portfolios. The platform simplifies portfolio creation by providing guided forms, customizable templates, live previews, GitHub project import, and AI-assisted content generation.

Users can enter their personal information, technical skills, education, and projects. The system can help improve project descriptions and generate an editable professional biography based on information provided by the user.

### 1.1.2 Problem Statement

Junior developers often struggle to present their technical skills and projects professionally. Creating a portfolio from scratch may require design knowledge, frontend development skills, and considerable time.

In addition, developers may find it difficult to write effective project descriptions, organize their work, and highlight relevant skills.

PortfolioGenie aims to address these challenges by offering a guided portfolio-building experience supported by AI-powered content assistance and GitHub integration.

### 1.1.3 Project Aim

The main aim of PortfolioGenie is to provide an accessible and user-friendly platform that enables junior developers to create, customize, preview, and publish professional portfolios with less effort.

### 1.1.4 Project Objectives

The project objectives are to:

1. Develop an intuitive and responsive user interface.
2. Provide a guided, multi-step portfolio creation process.
3. Allow users to manage personal information, skills, education, and projects.
4. Integrate with the GitHub API to retrieve relevant public repository information.
5. Use AI to assist with writing and improving portfolio content.
6. Provide customizable portfolio templates and a live preview.
7. Allow users to review and edit AI-generated content before using it.
8. Enable users to publish and share their completed portfolios through public links, subject to the implemented publishing functionality.
9. Follow software engineering principles that support maintainability, accessibility, and usability.

### 1.1.5 Project Scope

#### In Scope

- User registration and authentication, if included in the final implementation.
- Creating and editing portfolio profiles.
- Managing skills, education, and project information.
- Importing selected public GitHub repository information.
- AI-assisted generation and improvement of portfolio text.
- Selecting portfolio templates.
- Previewing portfolio content before publication.
- Saving portfolio data.
- Publishing or sharing portfolios through public URLs, if supported by the final system.
- Responsive design for desktop, tablet, and mobile devices.
- Basic validation, error handling, and testing.

#### Out of Scope

- Training a custom AI model from scratch.
- Building a recruitment or job-matching platform.
- Accessing private GitHub repositories without appropriate authorization.
- Developing a dedicated native Android or iOS application.
- Advanced analytics, custom domains, or paid subscription features unless added to the approved project scope.

### 1.1.6 Target Users

The primary target users are:

- Junior developers seeking their first job or internship.
- Computer science and information technology students.
- Recent graduates who need to showcase their projects.
- Freelancers who want to present their skills and previous work.

### 1.1.7 Proposed Technologies

The final technology stack will depend on the team's implementation decisions.

| Component | Proposed Technology |
|---|---|
| Frontend | React |
| Routing | React Router |
| Styling | CSS, Bootstrap, or Tailwind CSS |
| Backend | Node.js and Express.js |
| Database | MongoDB |
| GitHub Integration | GitHub REST API |
| AI Integration | An external AI API |
| UI/UX Design | Figma |
| Version Control | Git and GitHub |
| Testing | Appropriate frontend and backend testing tools |

## 1.2 Project Plan

### 1.2.1 Project Management Approach

The team will follow an iterative development approach. The project will be divided into manageable phases, allowing the team to review progress, identify problems early, and improve the application throughout development.

The team will use GitHub for version control, issue tracking, and collaboration. Tasks will be assigned according to team members' responsibilities and reviewed regularly.

### 1.2.2 Project Timeline

The following schedule is a proposed eight-week plan and should be adjusted according to the actual project deadline.

| Phase | Timeline | Main Deliverables |
|---|---|---|
| Requirements Gathering and Planning | Week 1 | Project proposal and requirements |
| UI/UX Design | Weeks 1–2 | Wireframes and interface design |
| Database and API Planning | Weeks 2–3 | Database structure and API plan |
| Core Development | Weeks 3–5 | Main frontend and backend features |
| AI and GitHub Integration | Weeks 5–6 | AI assistance and repository import |
| System Integration | Week 6–7 | Integrated application |
| Testing and Bug Fixing | Weeks 7–8 | Test results and corrected issues |
| Final Documentation and Presentation | Week 8 | Final report and presentation |

### 1.2.3 Milestones

| Milestone | Expected Completion | Success Criteria |
|---|---|---|
| M1: Project Approval | End of Week 1 | Project scope and objectives agreed upon |
| M2: Requirements and Design | End of Week 2 | Requirements and initial designs reviewed |
| M3: Core Application | End of Week 5 | Main portfolio creation features implemented |
| M4: Integrations | End of Week 6 | Planned AI and GitHub features integrated |
| M5: System Testing | End of Week 7 | Critical defects addressed |
| M6: Final Delivery | End of Week 8 | Documentation, demonstration, and final build ready |

### 1.2.4 Task Assignment and Roles

The following roles are proposed and may be adjusted based on the team's skills and workload.

| Team Member | Main Responsibility | Expected Deliverables |
|---|---|---|
| Member 1 | UI/UX Design and Frontend Foundation | Wireframes, design system, shared interface components |
| Member 2 | Portfolio Builder Frontend | Multi-step form, portfolio editor, live preview |
| Member 3 | Backend and Database | API endpoints, database models, data persistence |
| Member 4 | AI and GitHub Integration | AI content assistance and GitHub repository import |
| Member 5 | Templates, System Integration, and Quality Assurance | Portfolio templates, integration support, test cases, bug reports |

All team members are expected to participate in documentation, code reviews, integration, testing, and project presentations.

### 1.2.5 Resources

The project may require the following resources:

- **Human Resources:** Five team members and the project supervisor.
- **Development Tools:** Code editor, browser, Git, and GitHub.
- **Design Tools:** Figma or an equivalent interface-design tool.
- **Technical Resources:** React, backend services, database, GitHub API, and an AI API.
- **Documentation Resources:** Project reports, technical documentation, and relevant academic or official sources.

External APIs may have rate limits, usage restrictions, or costs. The team should review their terms before integration.

## 1.3 Risk Assessment and Mitigation

| Risk | Probability | Impact | Mitigation Strategy |
|---|---|---|---|
| Project delays | Medium | High | Set weekly milestones and review progress |
| GitHub API limitations | Medium | Medium | Handle rate limits and provide clear error messages |
| AI-generated inaccurate content | Medium | High | Allow users to review and edit generated content |
| Integration conflicts | Medium | High | Agree on API contracts and use feature branches |
| Data loss | Low | High | Implement appropriate persistence and backup practices |
| Security vulnerabilities | Medium | High | Validate inputs and protect authentication and API credentials |
| Responsive design issues | Medium | Medium | Test on different screen sizes |
| Team communication problems | Medium | Medium | Hold regular meetings and document decisions |

Probability and impact ratings are initial estimates and should be reviewed as the project progresses.

## 1.4 Key Performance Indicators (KPIs)

The team will use the following indicators to evaluate project progress and quality.

| KPI | Measurement Method | Proposed Target |
|---|---|---|
| Requirement Completion | Percentage of approved requirements implemented | At least 90% of approved in-scope requirements |
| Core Feature Completion | Verification against the agreed feature checklist | All critical features completed |
| Test Pass Rate | Passed tests divided by executed tests | At least 90% before final delivery |
| Critical Defects | Number of unresolved critical defects | Zero known critical defects at release |
| Responsive Compatibility | Results of testing across agreed screen sizes | All agreed screen sizes tested successfully |
| AI Content Editability | Verify users can review and edit generated content | All AI-generated fields in scope are editable |
| GitHub Import Reliability | Successful imports in agreed test scenarios | Target set after baseline testing |
| Documentation Completion | Review of required documentation sections | All required sections completed and reviewed |

These targets are proposed project goals, not measured results. Actual results should be recorded after implementation and testing.

## 1.5 Project Completion Criteria

PortfolioGenie will be considered ready for final submission when:

1. The agreed core requirements have been implemented.
2. The portfolio creation workflow works as intended.
3. The planned AI and GitHub integrations have been tested.
4. Users can review and edit generated content.
5. The interface has been tested on the agreed screen sizes.
6. Critical defects have been addressed.
7. The documentation has been reviewed by the team.
8. The final demonstration and presentation materials are ready.
