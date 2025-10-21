## Requirement Analysis in Software Development.

This repository captures the requirement analysis for an Airbnb-like application. It defines scope, goals, and constraints; consolidates functional and non-functional requirements; and provides user stories and acceptance criteria to align stakeholders. The materials here guide architecture, UX, implementation planning, and testing, serving as the single source of truth for delivery.

### What is Requirement Analysis?

Requirement Analysis is the disciplined process of discovering, clarifying, documenting, and validating what a system must do and the constraints under which it must operate. It converts stakeholder needs into clear, testable, and prioritized requirements that guide all downstream work.
Why it matters in the SDLC (Software Development Life Cycle):
- The Requirement Analysis phase is crucial as it lays the foundation for all subsequent stages of the SDLC. It ensures that the development team understands what the stakeholders need, which helps in delivering a product that meets user expectations.
- By clearly defining requirements, the risk of scope creep is minimized, allowing for better project management and resource allocation.
- It facilitates effective communication among stakeholders, developers, and testers, ensuring everyone is aligned on project goals and deliverables.
- Proper requirement analysis leads to higher quality software, as it reduces the likelihood of defects and rework during later stages of development.
- It supports compliance with regulatory and industry standards by ensuring that all necessary requirements are captured and addressed.
- Ultimately, thorough requirement analysis contributes to the overall success of the project, enhancing user satisfaction and business value.
- Planning: sets scope boundaries, identifies assumptions and risks, and enables estimation and roadmap planning.
- Design: informs architecture and UX with quality attributes (performance, security, availability, usability, compliance).
- Implementation: populates the backlog with well-formed user stories and acceptance criteria, reducing ambiguity and rework.
- Testing: supplies traceable, testable requirements for test planning and coverage; supports a requirements traceability matrix.
- Deployment and operations: NFRs drive capacity planning, monitoring, SLAs, and operational constraints.
- Maintenance and evolution: structured change control and impact analysis minimize regression and scope drift.

### Why is Requirement Analysis Important?

Requirement Analysis is critical in the SDLC for several key reasons:

1. **Reduces Development Costs and Rework**: Identifying and correcting requirements errors early is exponentially cheaper than fixing defects discovered during testing or post-deployment. Clear requirements minimize misunderstandings that lead to costly rework and wasted development effort.

2. **Ensures Stakeholder Alignment and Satisfaction**: Thorough requirement analysis establishes a shared understanding among all stakeholders—business owners, users, developers, and testers. This alignment ensures the final product meets actual user needs and business objectives, leading to higher satisfaction and adoption rates.

3. **Provides a Foundation for Quality and Testing**: Well-defined requirements serve as the basis for test cases, acceptance criteria, and quality metrics. They enable comprehensive test coverage, support validation activities, and provide objective criteria for determining when the system is ready for release.

Core activities:
- Elicitation: interviews, workshops, observation, surveys, document analysis, prototyping.
- Analysis and modeling: user stories/use cases, workflows, domain models, data/state diagrams.
- Specification: SRS/BRD or product backlog with acceptance criteria and definitions of done.
- Validation and verification: reviews, walkthroughs, prototypes, and stakeholder sign-off.
- Management: prioritization, baselining, versioning, and end-to-end traceability.

Typical deliverables: glossary, personas, user stories, acceptance criteria, functional and non-functional requirements, and a traceability matrix.

### Key Activities in Requirement Analysis

**Requirement Gathering**
- Collecting high-level business needs, constraints, and objectives from stakeholders and existing documentation
- Identifying sources of requirements including business stakeholders, end users, regulatory bodies, and legacy systems
- Assembling background materials such as business cases, market research, competitor analysis, and existing system documentation
- Establishing the project context, scope boundaries, and initial assumptions

**Requirement Elicitation**
- Conducting structured interviews and workshops with stakeholders to uncover detailed needs and expectations
- Facilitating brainstorming sessions and focus groups to generate ideas and identify pain points
- Observing users in their work environment to understand actual workflows and unspoken requirements
- Using questionnaires and surveys to gather input from large or distributed user groups
- Analyzing existing documentation, processes, and systems to extract implicit requirements
- Creating prototypes and mockups to help stakeholders articulate and refine their needs

**Requirement Documentation**
- Recording requirements in a clear, consistent, and structured format (user stories, use cases, or formal specifications)
- Writing detailed descriptions with acceptance criteria, preconditions, postconditions, and business rules
- Creating a comprehensive glossary to define domain terminology and ensure common understanding
- Organizing requirements into logical categories (functional, non-functional, technical, business)
- Maintaining metadata such as priority, source, rationale, and dependencies for each requirement

**Requirement Analysis and Modeling**
- Analyzing requirements for completeness, consistency, feasibility, and testability
- Identifying conflicts, gaps, and ambiguities that need resolution
- Prioritizing requirements based on business value, risk, dependencies, and stakeholder input
- Creating visual models such as use case diagrams, process flows, data models, and state diagrams
- Decomposing high-level requirements into more detailed, implementable specifications
- Assessing technical and operational feasibility of proposed requirements

**Requirement Validation**
- Reviewing requirements with stakeholders to confirm accuracy and alignment with business goals
- Conducting walkthroughs and inspection sessions to identify errors, omissions, and inconsistencies
- Validating requirements against acceptance criteria and quality standards
- Obtaining formal sign-off and approval from key stakeholders
- Ensuring requirements are verifiable, traceable, and measurable
- Establishing a baseline for change control and version management


### Types of Requirements

#### Functional Requirements

Functional Requirements define what the system must do—the specific behaviors, features, and functions that deliver value to users and support business processes. They describe inputs, outputs, data transformations, and user interactions.

**Examples for Airbnb Booking Management:**

- **Property Search and Filtering**: Users must be able to search for properties by location, dates, price range, number of guests, and amenities (WiFi, parking, pet-friendly).
- **Booking Creation**: Guests must be able to select available dates, specify the number of guests, review pricing details, and submit a booking request to the host.
- **Payment Processing**: The system must securely process payments via credit card, debit card, or digital wallets, and send payment confirmations to both guest and host.
- **Booking Management**: Hosts must be able to view, accept, decline, or cancel booking requests, and guests must be able to modify or cancel their reservations according to the cancellation policy.
- **Review and Rating System**: After checkout, guests must be able to leave reviews and ratings for properties, and hosts must be able to respond to reviews and rate guests.
- **Notification System**: The system must send email and in-app notifications for booking confirmations, cancellations, payment receipts, upcoming check-ins, and review reminders.
- **Calendar Synchronization**: Hosts must be able to block dates for unavailability and sync their calendar with external booking platforms to prevent double-bookings.

#### Non-functional Requirements

Non-functional Requirements define how the system performs its functions—the quality attributes, constraints, and operational characteristics that affect user experience, reliability, and maintainability. They cover performance, security, usability, scalability, and compliance.

**Examples for Airbnb Booking Management:**

- **Performance**: The property search page must load results within 2 seconds under normal load conditions, and booking confirmation must be processed within 3 seconds.
- **Scalability**: The system must support up to 100,000 concurrent users during peak booking periods without performance degradation.
- **Availability**: The booking platform must maintain 99.9% uptime, with planned maintenance windows scheduled during off-peak hours and communicated in advance.
- **Security**: All payment transactions must be encrypted using TLS 1.3, personal data must comply with GDPR and CCPA regulations, and user authentication must support multi-factor authentication (MFA).
- **Usability**: The booking workflow must be completable within 5 clicks, the interface must be intuitive for first-time users without requiring training, and the application must be accessible according to WCAG 2.1 Level AA standards.
- **Reliability**: The system must implement automated data backups every 6 hours, maintain data consistency across distributed databases, and recover from failures within 15 minutes (RTO).
- **Compatibility**: The platform must be responsive and function correctly across Chrome, Firefox, Safari, and Edge browsers, and provide native mobile applications for iOS and Android devices.
- **Maintainability**: The codebase must follow established coding standards, include comprehensive unit test coverage (minimum 80%), and support zero-downtime deployments.

### Use Case Diagrams

Use Case Diagrams are visual representations that illustrate the interactions between users (actors) and the system, highlighting the various use cases that define the system's functionality. They provide a high-level overview of the system's requirements and help stakeholders understand how users will interact with the system.

#### Benefits of Use Case Diagrams:
- **Clarity**: They simplify complex system functionalities into easily understandable visuals, making it easier for stakeholders to grasp the system's capabilities.
- **Communication**: Use Case Diagrams facilitate discussions among stakeholders, developers, and designers by providing a common language and reference point.
- **Requirement Validation**: They help in validating requirements by ensuring that all necessary interactions are captured and understood.
- **Scope Management**: Use Case Diagrams assist in defining the scope of the project by clearly outlining what the system will and will not do.

#### Guest Use Cases:
1. **Search Properties**: Allows guests to search for available properties based on criteria such as location, dates, and number of guests.
2. **View Property Details**: Enables guests to view detailed information about a specific property, including descriptions, photos, amenities, and reviews.
3. **Create Account/Login**: Allows guests to create a new account or log in to an existing account to access the system's features.
4. **Book Property**: Enables guests to book a property for a specified period.
5. **Make Payment**: Allows guests to make payments for their bookings through the integrated payment gateway.
6. **Manage Bookings**: Enables guests to view, modify, or cancel their existing bookings.
7. **Write Reviews**: Allows guests to write reviews and provide feedback on properties they have stayed in.
8. **Receive Notifications**: Enables guests to receive notifications about booking confirmations, updates, and other relevant information.

### Acceptance Criteria

Acceptance Criteria are specific, measurable conditions that a feature or user story must satisfy to be considered complete and accepted by stakeholders. They serve as a contract between the development team and stakeholders, defining the boundaries of functionality and providing clear pass/fail guidelines for testing and validation.

#### Importance of Acceptance Criteria in Requirement Analysis:

- **Establishes Clear Definition of Done**: Acceptance criteria eliminate ambiguity by precisely defining what "complete" means for each feature, preventing misunderstandings between developers, testers, and stakeholders.
- **Enables Effective Testing**: They provide the foundation for creating test cases and scenarios, ensuring comprehensive test coverage and objective validation of functionality.
- **Facilitates Accurate Estimation**: Well-defined acceptance criteria help development teams better estimate effort and complexity, leading to more reliable sprint planning and delivery commitments.
- **Reduces Rework and Scope Creep**: By establishing boundaries upfront, acceptance criteria prevent feature bloat and minimize costly rework caused by unclear or changing expectations.
- **Supports Stakeholder Alignment**: They ensure all parties share the same understanding of what will be delivered, reducing conflicts and promoting consensus.
- **Enables Early Validation**: Acceptance criteria can be reviewed and approved before development begins, catching issues in requirements before they become expensive defects.

#### Example: Acceptance Criteria for Checkout Feature

**Feature**: Guest Checkout and Payment Processing

**Acceptance Criteria**:

1. **Booking Summary Display**
    - Given a guest is on the checkout page, when the page loads, then the system must display property name, check-in/check-out dates, number of guests, nightly rate, total nights, subtotal, service fee, taxes, and grand total.

2. **Payment Method Selection**
    - Given a guest is ready to pay, when they view payment options, then the system must support credit card, debit card, PayPal, and Apple Pay as payment methods.

3. **Payment Information Validation**
    - Given a guest enters payment details, when they submit the form, then the system must validate card number format, expiration date (not expired), CVV (3-4 digits), and billing address completeness before processing.

4. **Secure Payment Processing**
    - Given valid payment information is submitted, when the payment is processed, then all transaction data must be encrypted using TLS 1.3 and handled via PCI-DSS compliant payment gateway.

5. **Booking Confirmation**
    - Given a successful payment, when the transaction completes, then the system must generate a unique booking confirmation number, send confirmation emails to both guest and host within 30 seconds, and update the property calendar to mark dates as booked.

6. **Payment Failure Handling**
    - Given a payment fails, when the error occurs, then the system must display a clear error message indicating the reason (insufficient funds, invalid card, etc.), retain the entered booking details, and allow the guest to retry with a different payment method without re-entering booking information.

7. **Cancellation Policy Acknowledgment**
    - Given a guest is reviewing their booking, when they reach the payment step, then the system must display the applicable cancellation policy and require explicit acknowledgment (checkbox) before allowing payment submission.

8. **Receipt Generation**
    - Given a completed booking, when payment is confirmed, then the system must generate a downloadable PDF receipt containing booking reference, itemized charges, payment method (last 4 digits only), transaction date, and host contact information.