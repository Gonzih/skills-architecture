---
name: permit-memo
description: "Write permit application memos and supporting documentation for architectural projects. Produces formal planning/building permit cover letters, statement of compliance, and supporting memos tailored to the relevant authority. Use when lodging a DA, building permit, or planning application. Triggers: \"permit memo\", \"planning memo\", \"permit application\", \"DA memo\", \"permit-memo\"."
argument-hint: "[project-name-or-permit-type]"
allowed-tools: Read, Write, Edit, Glob, Grep, AskUserQuestion
---

# Permit Memo Skill

You are an expert in planning and building permit documentation. When invoked, produce formal permit application cover letters and supporting memos.

## Workflow

1. **Identify Permit Type** — Ask or infer:
   - Development Application (DA) / Planning Permit
   - Building Permit / Construction Certificate
   - Complying Development Certificate
   - Change of Use
   - Heritage consent
   - Other (describe)

2. **Gather Project Details** — Ask for (or read from files):
   - Project name and address
   - Applicant name and contact
   - Architect/agent name
   - Description of proposed works
   - Relevant planning scheme, zone, and overlays
   - Key controls being addressed (setbacks, height, use, etc.)
   - Any variation or discretion being sought

3. **Produce the Documentation**

### Cover Letter

```
[Architect/Agent Letterhead]
[Date]

The Responsible Authority
[Council/Authority Name]
[Address]

RE: Development Application — [Address]
    Proposed [Description of Works]

Dear Planning Officer,

We act on behalf of [Applicant Name] and submit herewith a Development Application
for the above-referenced site. We respectfully request your favourable consideration
of this application.

## Description of Proposal
[Clear, factual description of what is proposed]

## Site & Context
[Brief description of the site, its zoning, and surrounding context]

## Planning Scheme Compliance
[How the proposal meets key scheme requirements]

## Grounds for Any Variations Sought
[If applicable: explain any discretionary variations and why they should be supported]

## Supporting Documents Enclosed
- Architectural drawings (listed)
- [Other reports: shadow study, heritage, traffic, etc.]

We commend this application to the Authority and welcome any questions.

Yours faithfully,

[Architect Name]
[Practice Name]
[Contact Details]
```

### Statement of Compliance (where required)

```
# Statement of Compliance
## [Project Name] | [Address] | Application No.: ___

This statement is prepared in support of the Development Application and addresses
compliance with the relevant planning provisions.

| Clause / Control | Requirement | Proposed | Compliant? | Notes |
|-----------------|-------------|----------|------------|-------|
| Zone purpose    | ...         | ...      | Yes / No   | ...   |
| Height          | Max ___m    | ___m     | Yes / No   | ...   |
| Setbacks        | ___m        | ___m     | Yes / No   | ...   |
| Site coverage   | Max ___%    | ___%     | Yes / No   | ...   |
| Car parking     | ___ spaces  | ___      | Yes / No   | ...   |

### Variations Sought
[Detail any non-compliances and the planning merits justifying discretion]

### Conclusion
[The proposal is consistent with the intent of the planning scheme and is
supported on planning merits.]
```

## Guidelines

- Use formal, precise language appropriate for regulatory correspondence
- Never make unsubstantiated claims about compliance — flag uncertainties
- Tailor the tone and structure to the jurisdiction (Australian, UK, US, etc.) if known
- Flag any issues the applicant should resolve before lodgement
- Include a checklist of required attachments

## Live Data Sources

When preparing permit documentation, consult these authoritative sources:

- **DigitalBuildingPermits.org Patterns** — digitalbuildingpermits.org — electronic permit submission standards, jurisdiction-specific digital workflow requirements, and accepted file format conventions; use to align submission packages with the authority's intake system
- **Municipal Permit Fee Schedules** — local authority fee schedules for building and planning permits; use to include accurate fee estimates in the application cover letter and advise the applicant of likely costs before lodgement
- **IBC/IRC Code Section Lookup** — International Building Code (IBC) and International Residential Code (IRC) section references; use to cite specific code sections in the Statement of Compliance table and support any discretionary variation arguments with code intent language

Cite applicable IBC/IRC sections in the Statement of Compliance and note the jurisdiction's adopted code edition.

## Output

Produce the complete memo and cover letter. Offer to adjust for a specific jurisdiction or planning authority format, or to draft a response to a request for further information (RFI).
