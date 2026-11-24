# BU-DineSync
## Product Requirements Document (PRD)

**Product:** BU-DineSync – Babcock University Digital Meal Verification System  
**Document:** Product Requirements Document  
**Done by:** The Team

### Project Team Members

| S/N | Full Name | Matric Number | Responsibility |
|---:|---|---|---|
| 1 | Paul Mimshach Osemudiamem | 25/2279 | Team Member |
| 2 | Chukwu Godwin Chukwuyelum | 25/2348 | Team Member |
| 3 | Okeke Stephen Ifechukwu | 25/2061 | Team Member |
| 4 | Akinola Tijesunimi Adams | 25/0121 | Team Member |
| 5 | Chidiebere Daniel | 25/0349 | Team Lead |

---

## 1. Product Overview

BU-DineSync is a proposed digital meal-verification system for Babcock University. It is intended to make the process of confirming a student's meal eligibility more reliable and convenient.

Babcock University currently uses student identification cards for meal verification for returning students. Students who do not yet have their university ID cards or have not completed the relevant verification process may use physical meal tickets. The proposed system will provide an authorised digital method of verifying meal eligibility while keeping the university's existing meal entitlements and approval process under the control of the appropriate university offices.

BU-DineSync is a proposed solution. It is not an existing Babcock University service, and its implementation would require approval and cooperation from the relevant university departments.

## 2. Problem Statement

The current meal-verification process can create difficulties for some students:

- Physical meal tickets used by some students can be misplaced or lost.
- Some returning students experience problems when their ID cards are scanned for meal verification.
- When an ID-card verification problem occurs, the affected student may have to leave the cafeteria and visit an office some distance away to have the card checked, updated or reactivated.
- The student may be unable to collect a meal until the issue has been resolved.

Students have already paid for their applicable semester meal plan. The issue described here is not necessarily that a student's meal balance has run out or that another payment is due. It is a verification or card-service issue that may prevent an eligible student from being recognised by the cafeteria verification process.

**Problem to solve:** How might Babcock University provide an authorised, dependable alternative for confirming meal eligibility when a physical ticket or student ID card is unavailable or cannot be verified?

## 3. Current Process and Observed Challenges

Based on the process described for this assessment:

1. Returning students generally present their university ID cards at the cafeteria.
2. The card is scanned using the cafeteria's verification machine.
3. The machine displays the student's details and indicates whether meal eligibility is approved.
4. Some students who encounter ID-card verification problems are directed to an office for assistance with the card.
5. Students who do not yet have an ID card or have not completed the relevant verification process may use physical meal tickets.

### 3.1 Known observations

The following points were provided from the observed Babcock University process:

- Returning students use their ID cards for meal verification.
- Some students experience ID-card verification problems.
- Affected students may need to visit an office away from the cafeteria to resolve the issue.
- Some students use physical meal tickets, which may be lost.

### 3.2 Evidence limitations

No survey percentages, interview quotations, average waiting times, or measured incident frequencies are included in this document because verified figures were not supplied for this version. These should only be added after they have been collected and checked. The observations above describe the process reported for this assessment and should be validated with cafeteria staff and the relevant university office before implementation.

## 4. Product Vision

To provide Babcock University students and authorised cafeteria staff with a simple, reliable and secure way to confirm meal eligibility, reducing avoidable disruption when an ID card or physical meal ticket cannot be used.

## 5. Goals and Objectives

BU-DineSync aims to:

1. Provide an authorised digital method of checking a student's meal eligibility.
2. Reduce reliance on physical meal tickets where the university approves a digital alternative.
3. Provide an alternative verification route for eligible students whose ID cards cannot be read.
4. Help authorised cafeteria staff confirm eligibility without making decisions based only on a student's verbal claim.
5. Record successful and unsuccessful verification attempts for accountability and support.
6. Protect student information and prevent duplicate or unauthorised meal collection.

### 5.1 Out of scope

The first version is not intended to:

- Change the university's meal-plan fees or payment arrangements.
- Give students additional meal entitlements.
- Allow students to bypass the university's meal eligibility rules.
- Replace the university's student information system or official ID-card system.
- Manage cafeteria menus, food inventory, food preparation or food reservations.
- Guarantee that every card issue can be resolved without the responsible university office.

## 6. Target Users

### 6.1 Students

Students with an approved meal plan who need to verify their eligibility before collecting a meal. This includes returning students using ID cards and students authorised to use an alternative verification method.

### 6.2 Cafeteria verification staff

Authorised staff who need to confirm whether a student is eligible to collect a meal and record the verification result.

### 6.3 University administrators

Authorised personnel responsible for student records, meal-plan eligibility, ID-card services and access permissions. Their involvement is required to approve the system and determine which official data source can be used.

## 7. Stakeholders

| Stakeholder | Interest or responsibility |
|---|---|
| Babcock University students | Need a clear and dependable way to prove meal eligibility. |
| Cafeteria staff | Need to verify eligibility accurately before serving a meal. |
| Relevant student-affairs or meal-plan office | Owns or administers the applicable meal eligibility process. |
| ID-card/ICT support personnel | May be responsible for student-card services and approved system integration. |
| University management | Provides approval, oversight and policy direction. |

The exact department names, system owners and approval responsibilities must be confirmed with the university.

## 8. Proposed Solution

BU-DineSync proposes a secure digital verification service linked to an authorised source of student meal eligibility. A student would present an approved digital identifier, such as a university-approved QR code or another method selected by the university. An authorised cafeteria staff member would scan or enter the identifier using a staff-facing verification interface.

The system would check the identifier against the approved eligibility record and display a simple result, such as:

- **Eligible:** the student is currently authorised to collect the applicable meal.
- **Already redeemed:** the relevant meal entitlement has already been recorded as used, where the university's rules support this check.
- **Not verified:** the system cannot confirm eligibility; the student should be referred through the approved support process.

The system must not create or change meal entitlements by itself. The authoritative university record remains the source of truth. The exact identifier, data connection and redemption rules must be approved by Babcock University before development.

## 9. Main User Flow

1. The student opens the university-approved digital pass or presents the approved digital identifier.
2. Cafeteria staff open the authorised BU-DineSync verification interface.
3. Staff scan the student's identifier or enter it using the approved method.
4. BU-DineSync checks the identifier against the authorised eligibility source.
5. The interface displays the verification result and only the minimum information staff need.
6. If the student is eligible, staff confirm the meal collection and the system records the redemption according to university policy.
7. If the student cannot be verified, the interface explains that eligibility could not be confirmed and directs staff or the student to the approved support channel. It must not automatically grant a meal.

## 10. Minimum Viable Product (MVP)

The MVP should focus on the smallest set of functions needed to test digital meal verification safely.

### Included in the MVP

- Secure sign-in for authorised cafeteria staff.
- Student identifier scanning or lookup using a university-approved method.
- Eligibility check against an authorised data source or a controlled test dataset approved for the prototype.
- Clear eligible, already-redeemed and unable-to-verify results, where applicable to the approved meal rules.
- A record of verification and redemption events.
- Basic administrative ability to manage authorised staff access.
- A clear fallback instruction for cases that require the responsible university office.

### Not included in the MVP

- Processing school-fee or meal-plan payments.
- Editing official student records.
- Changing meal-plan entitlement rules.
- Menu ordering, food inventory and food reservation features.
- Facial recognition or other biometric identification.
- Integration with live Babcock University systems before written approval and access are provided.

## 11. User Stories

| ID | User story | Priority |
|---|---|---|
| US-01 | As a student with an approved meal plan, I want an approved digital identifier so that I can present an alternative when the university permits it. | Must have |
| US-02 | As a cafeteria staff member, I want to scan or look up a student's identifier so that I can confirm meal eligibility. | Must have |
| US-03 | As a cafeteria staff member, I want a clear verification result so that I know whether the student can proceed under the university's rules. | Must have |
| US-04 | As a student whose identifier cannot be verified, I want clear guidance on the next step so that I know how to resolve the issue. | Must have |
| US-05 | As an authorised administrator, I want to control staff access so that only approved personnel can use the verification interface. | Must have |
| US-06 | As an authorised administrator, I want verification and redemption records so that issues can be reviewed and investigated. | Should have |
| US-07 | As a student, I want my personal information protected so that only the minimum necessary details are shown during verification. | Must have |

## 12. Functional Requirements

| ID | Requirement | Priority |
|---|---|---|
| FR-01 | The system shall allow authorised cafeteria staff to sign in securely. | Must have |
| FR-02 | The system shall accept a student identifier through the university-approved scanning or lookup method. | Must have |
| FR-03 | The system shall check the identifier against an authorised meal-eligibility source. | Must have |
| FR-04 | The system shall display a clear result indicating whether eligibility was confirmed. | Must have |
| FR-05 | The system shall not grant eligibility where the authorised source cannot confirm it. | Must have |
| FR-06 | Where required by university policy, the system shall prevent the same meal entitlement from being redeemed more than once. | Must have |
| FR-07 | The system shall record verification outcomes and meal-redemption events for authorised review. | Should have |
| FR-08 | The system shall provide an approved support instruction when verification fails. | Must have |
| FR-09 | The system shall allow an authorised administrator to enable or disable staff accounts. | Should have |
| FR-10 | The system shall limit the student information displayed to staff to what is necessary for verification. | Must have |

## 13. Non-Functional Requirements

### Security and privacy

- Only authorised staff should be able to access staff functions.
- Student information must be protected in storage and during transmission.
- Access to records should be limited according to staff roles.
- Verification and administrative actions should be logged.
- The product must follow the university's privacy, data-handling and information-security requirements.

### Reliability

- The system should return a clear result when the approved eligibility service is available.
- If the eligibility service or network is unavailable, the system must show that verification is unavailable rather than incorrectly approving a student.
- A documented manual fallback process should be agreed with the university.

### Usability

- The verification screen should be simple enough for cafeteria staff to use with minimal training.
- Results should be clearly distinguishable and use plain language.
- The student-facing process should require as few steps as practical.

### Performance

- Under normal operating conditions, a verification request should return a result quickly enough to be practical during meal service. A specific response-time target should be set after testing with cafeteria staff and the approved infrastructure.

### Compatibility

- The staff interface should work on devices approved by the university.
- The student identifier method should be selected based on devices and systems the university can support.

## 14. Acceptance Criteria

The MVP can be considered ready for a controlled pilot when:

1. An authorised staff member can sign in successfully.
2. Staff can submit a valid test student identifier.
3. The system returns the correct eligibility result for approved test cases.
4. The system does not approve an unknown or unverified identifier.
5. Where duplicate redemption prevention is required, a second attempt for the same meal entitlement is rejected or flagged.
6. The system records the verification outcome for later authorised review.
7. A staff member can identify the correct support route when verification is unavailable or unsuccessful.
8. Unauthorised users cannot access staff verification functions.
9. Testing confirms that only necessary student details are displayed.

## 15. Success Metrics

The following measures can be used during a pilot. Baseline values and targets should be agreed after the university approves the pilot and initial measurements are collected.

- **Verification success rate:** percentage of valid eligible test attempts correctly verified.
- **Verification time:** time taken from identifier submission to displayed result.
- **Failed verification rate:** percentage of attempts that cannot be confirmed.
- **Duplicate redemption prevention:** number of duplicate attempts correctly flagged or blocked in test cases.
- **Staff usability:** feedback from cafeteria staff after using the prototype.
- **Student experience:** feedback from participating students about clarity and ease of verification.
- **System availability:** proportion of the agreed pilot period during which the verification service is available.

No numerical targets are claimed in this PRD because a measured baseline has not been provided.

## 16. Assumptions and Dependencies

### Assumptions

- Babcock University will determine the official source of meal eligibility.
- The university may approve an additional digital verification route.
- Students using the system will have an identifier approved by the university.
- Cafeteria staff will use the system only for authorised meal-verification purposes.

### Dependencies

- Approval from the relevant university authority.
- Identification of the department responsible for meal-plan eligibility.
- Approval and access to a suitable eligibility data source or API.
- Agreement on meal redemption rules, including whether entitlements are tracked per meal, per day or by another policy.
- Approval of the student identifier and staff devices to be used.
- A defined support and manual fallback process for outages and failed verification.

## 17. Risks and Mitigations

| Risk | Potential effect | Proposed mitigation |
|---|---|---|
| No access to the official eligibility source | The system cannot confirm real student entitlements. | Use an approved test dataset for the prototype and seek formal integration approval before a live pilot. |
| Network or service outage | Students may be unable to complete digital verification. | Display a clear unavailable status and use a university-approved fallback process. |
| Unauthorised access | Student records or meal-verification functions may be misused. | Use staff authentication, role-based access and audit logs. |
| Duplicate meal redemption | A meal entitlement may be used more than once. | Apply the university-approved redemption rules and record each transaction. |
| Student identifier is lost or shared | Another person may attempt to use the identifier. | Use a university-approved identity check and suitable controls such as time-limited or refreshable identifiers, if approved. |
| Incorrect eligibility data | An eligible student may be rejected or an ineligible student approved. | Treat the university's authorised record as the source of truth and provide a clear escalation route. |

## 18. Open Questions for Babcock University

1. Which office owns and maintains the official meal-plan eligibility records?
2. Is there an existing API or approved way to check meal eligibility electronically?
3. Would the university approve a QR code, student portal pass or another digital identifier?
4. Should the digital method support students who have not yet received their ID cards?
5. What exact meal-redemption rules should the system enforce?
6. What information may cafeteria staff see during verification?
7. What should happen when the internet, scanner or eligibility service is unavailable?
8. Which university staff members may create, disable or review system accounts?
9. What privacy, security and retention requirements must the system follow?
10. Which devices and network infrastructure may be used for a pilot?

## 19. Proposed Release Approach

### Phase 1 – Requirements confirmation

Confirm the process with students, cafeteria staff and the responsible university office. Resolve the open questions about eligibility records, identifiers and meal-redemption rules.

### Phase 2 – Prototype

Build a prototype using an approved test dataset. Demonstrate staff sign-in, identifier lookup, eligibility results and verification records without connecting to live student records.

### Phase 3 – Controlled testing

Test valid, invalid, duplicate and unavailable-service scenarios with authorised reviewers. Collect usability feedback and correct identified issues.

### Phase 4 – Approved pilot

Proceed to a limited live pilot only after the university grants the necessary approval, data access, device access and operational support.

## 20. Conclusion

BU-DineSync proposes a more dependable digital route for meal verification at Babcock University. The product is focused on the difficulty students may face when a physical meal ticket is lost or an ID card cannot be verified. By checking eligibility through an authorised university source, giving cafeteria staff clear results and recording verification events, the proposed system could make the process easier to manage while preserving the university's existing meal rules.

The next step is to validate the requirements with the relevant Babcock University stakeholders and obtain approval before any live integration or deployment.

---

## Submission Checklist

- [ ] Add only research figures, dates or interview quotations that were actually collected and verified.
- [ ] Save the file with the exact name `PRD.md`.
- [ ] Upload the file to the correct repository branch as instructed by the lecturer.
