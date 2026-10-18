# 3. Literature Review

## 3.1 Introduction

This literature review examines existing approaches and technologies related to PortfolioGenie, an AI-powered platform for building developer portfolios.

The review focuses on three main areas: online developer portfolios, GitHub integration, and AI-assisted content generation. These areas provide the technical and conceptual foundation for the proposed system.

The purpose of this review is to identify useful existing practices, evaluate their relevance to the project, and determine opportunities for improvement.

## 3.2 Related Work

### 3.2.1 Online Developer Portfolios

Online developer portfolios allow developers to present their technical skills, projects, education, and professional background through a shareable website.

A portfolio can help developers organize their work and provide recruiters or potential clients with examples of their abilities. However, creating a portfolio from scratch may require frontend development knowledge, design skills, and time.

PortfolioGenie aims to simplify this process by providing guided portfolio creation, reusable templates, and a live preview.

**Relevance to PortfolioGenie:**

- Simplifies the portfolio creation process.
- Provides consistent layouts and reusable templates.
- Helps users organize project and profile information.
- Allows users to review their portfolios before sharing them.

### 3.2.2 GitHub Integration

GitHub provides a REST API that enables applications to retrieve supported repository information. This information may include repository names, descriptions, URLs, and other available metadata, depending on the endpoint and permissions.

Integrating GitHub into PortfolioGenie can reduce the effort required to enter project information manually.

However, repository metadata alone does not guarantee that a project description accurately represents the developer's contribution or the quality of the work. Therefore, imported information should be reviewed by the user before being included in a portfolio.

**Relevance to PortfolioGenie:**

- Reduces repetitive manual data entry.
- Helps users identify projects to include.
- Provides repository links and available metadata.
- Allows users to review imported information before saving it.

**Technical Reference:** GitHub REST API documentation.

https://docs.github.com/en/rest/repos/repos

### 3.2.3 AI-Assisted Content Generation

AI-powered language models can assist users in drafting, rewriting, and improving written content. In PortfolioGenie, AI can help generate an About Me draft, improve project descriptions, and suggest clearer wording.

The quality of AI-generated content depends on the quality of the input information and the instructions provided in the prompt. Generated content may also contain inaccurate or unsupported claims.

For this reason, PortfolioGenie should use relevant user-provided information, provide clear prompts, and allow users to review and edit the generated output.

**Relevance to PortfolioGenie:**

- Helps users who struggle with professional writing.
- Improves the clarity and readability of project descriptions.
- Supports personalized content generation.
- Reduces the effort required to prepare portfolio text.

**Technical References:**

OpenAI, Prompt Engineering Guide:

https://developers.openai.com/api/docs/guides/prompt-engineering

OpenAI Help Center, Prompt Engineering Best Practices:

https://help.openai.com/en/articles/10032626-prompt-engineering-best-practices-for-chatgpt

## 3.3 Comparative Analysis

The following table compares common portfolio creation approaches with the proposed PortfolioGenie solution. It represents a conceptual comparison and should not be treated as the result of a formal usability study.

| Criterion | Manual Portfolio Development | Template-Based Portfolio Builder | Proposed PortfolioGenie |
|---|---|---|---|
| Ease of Creation | Requires technical and design effort | Generally easier | Guided creation process |
| Design Customization | High, depending on user skills | Depends on available templates | Template-based customization |
| Content Assistance | Written manually | Often written manually | AI-assisted drafting and improvement |
| GitHub Integration | Must be implemented or configured separately | Depends on the platform | Planned repository import |
| Live Preview | Must be developed or configured | Commonly available | Included in the proposed workflow |
| User Control | High | Depends on the platform | Users review and edit generated content |
| Technical Flexibility | Depends on the implementation | Depends on the platform | Depends on the implemented features |

## 3.4 Research Gap and Project Opportunity

The reviewed technologies provide useful capabilities, but PortfolioGenie aims to combine several of them in one guided workflow.

The project focuses on reducing the effort required to organize portfolio information, write professional content, and present development projects.

The main opportunities identified are:

1. **Simplified Creation:** Guide users through a structured, multi-step portfolio-building process.
2. **AI-Assisted Writing:** Generate editable content based on information supplied by the user.
3. **GitHub Integration:** Allow users to select relevant repository information rather than entering everything manually.
4. **User Control:** Require users to review imported and AI-generated content before accepting it.
5. **Responsive Design:** Make portfolios accessible across different screen sizes.
6. **Maintainable Architecture:** Use reusable components and a clear application structure to support future improvements.

These opportunities describe the project's intended value. Their effectiveness must be evaluated through implementation and testing.

## 3.5 Suggested Improvements

The following improvements are recommended during the design and development of PortfolioGenie.

### 3.5.1 Improve the User Experience

- Use a clear, multi-step portfolio creation process.
- Display progress indicators so users know which steps remain.
- Provide helpful validation messages.
- Include a live preview where practical.
- Allow users to return to previous steps without losing entered information.

### 3.5.2 Improve AI Content Quality

- Use prompts that specify the intended content type, tone, and length.
- Base generated text on information provided by the user.
- Avoid inventing skills, achievements, experience, or project contributions.
- Allow users to edit, regenerate, or reject generated content.
- Handle unavailable AI services gracefully.

### 3.5.3 Improve GitHub Import

- Allow users to review available repositories before importing them.
- Display repository names, links, and supported metadata.
- Allow manual editing of imported project descriptions.
- Handle authorization errors and API rate limits.
- Avoid exposing API credentials in frontend code.

### 3.5.4 Improve Accessibility and Responsiveness

- Use semantic HTML and appropriate form labels.
- Support keyboard navigation for essential functionality.
- Maintain readable text and sufficient color contrast.
- Test layouts on desktop, tablet, and mobile devices.
- Follow relevant WCAG accessibility recommendations.

### 3.5.5 Improve Testing and Maintainability

- Create test cases for core user workflows.
- Test API failures and incomplete user input.
- Use reusable React components where appropriate.
- Follow consistent naming and coding conventions.
- Review code through GitHub pull requests.
- Document setup instructions and configuration requirements.

## 3.6 Feedback and Evaluation

Feedback from the project supervisor and testing participants should be used to improve the system throughout development.

**Important:** The following table is a feedback-recording template. Actual feedback must be collected from the supervisor or testers; it should not be invented.

| Evaluation Area | Feedback to Record | Suggested Action |
|---|---|---|
| Project Scope | Record comments about objectives and scope | Update the project scope if approved |
| User Interface | Record comments about layout and navigation | Refine the design and user flow |
| Functional Requirements | Record missing or unclear features | Update requirements and priorities |
| AI Integration | Record observations about content quality | Improve prompts and validation |
| GitHub Integration | Record issues with repository retrieval | Improve error handling and import flow |
| Testing | Record defects and unsuccessful test cases | Fix issues and repeat testing |
| Documentation | Record comments about clarity and completeness | Revise the relevant sections |

### 3.6.1 Evaluation Methods

PortfolioGenie may be evaluated through:

- Supervisor review.
- Functional testing against approved requirements.
- Usability feedback from representative users.
- Responsive design testing.
- Accessibility checks.
- AI output review for relevance, clarity, and unsupported claims.
- GitHub integration tests covering successful and unsuccessful requests.

The team should record the testing method, results, limitations, and any changes made in response to feedback.

## 3.7 Proposed Final Grading Criteria

The following breakdown is an illustrative proposal only. The official assessment rubric provided by the supervisor or institution must take precedence.

| Assessment Component | Proposed Weight |
|---|---:|
| Documentation | 20% |
| Requirements Analysis and UI/UX Design | 15% |
| Implementation and Core Functionality | 30% |
| Testing and Evaluation | 15% |
| Final Presentation and Demonstration | 10% |
| Team Collaboration and Project Management | 10% |
| **Total** | **100%** |

The final weights should be updated once the official grading criteria are available.

## 3.8 Conclusion

The literature review highlights the relevance of online developer portfolios, GitHub integration, and AI-assisted content generation to the development of PortfolioGenie.

Combining these capabilities within a guided workflow may help junior developers organize their work and prepare professional portfolio content more efficiently.

The project should prioritize usability, accuracy, accessibility, privacy, and user control. The success of the proposed solution will ultimately depend on the quality of its implementation and the results of systematic testing.

## 3.9 References

1. GitHub. (n.d.). *REST API endpoints for repositories*. GitHub Docs. https://docs.github.com/en/rest/repos/repos

2. OpenAI. (n.d.). *Prompt engineering*. OpenAI API Documentation. https://developers.openai.com/api/docs/guides/prompt-engineering

3. OpenAI Help Center. (n.d.). *Prompt engineering best practices for ChatGPT*. https://help.openai.com/en/articles/10032626-prompt-engineering-best-practices-for-chatgpt

**Note:** Review the references before submission and format them according to the citation style required by your institution, such as APA or IEEE.
