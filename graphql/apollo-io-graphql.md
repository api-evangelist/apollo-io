# Apollo.io GraphQL Schema

## Overview

This is a conceptual GraphQL schema for the Apollo.io B2B sales intelligence and engagement platform. Apollo.io does not natively expose a GraphQL endpoint; this schema is derived from the Apollo REST API surface (https://docs.apollo.io/reference) and represents the logical data model as a GraphQL type system. It is intended to support tooling, documentation, code generation, and API governance workflows.

## Domain Model

Apollo.io organizes its API around several core domains:

- **People & Organizations** — the 270M+ contact database and 60M+ company database, searchable and enrichable by title, location, seniority, technology stack, funding stage, and more.
- **CRM** — Contacts, Accounts, Deals, and Pipelines managed within a user's workspace.
- **Sequences** — Multi-step outreach cadences (email, call, task) with subscriber management.
- **Engagement** — Emails, Calls, Tasks, Meetings, and Notes tracking every touchpoint.
- **Workspace** — Users, Labels, Tags, Custom Fields, Lists, and API Key management.
- **Webhooks & Events** — Real-time event delivery for platform automation.

## Schema Source

Schema derived from the Apollo REST API reference documentation at https://docs.apollo.io/reference and the Apollo API documentation at https://apolloio.github.io/apollo-api-docs/.

## Types

The schema defines the following named types (65 total):

### People Domain
- `Contact` — a person record in a user's CRM workspace
- `ContactDetails` — enriched detail record for a contact
- `ContactStatus` — enum of CRM lifecycle stages
- `PersonEmail` — structured email address with confidence and type
- `PersonPhone` — structured phone number with type (work/mobile/direct)
- `PersonTitle` — job title string with normalization metadata
- `PersonSeniority` — enum of seniority levels (C-Suite, VP, Director, Manager, etc.)
- `PersonDepartment` — functional department classification
- `PersonCompany` — company affiliation for a person record
- `PersonLinkedIn` — LinkedIn profile URL and metadata
- `PersonTwitter` — Twitter handle and metadata
- `PersonLocation` — city, state, country, and postal code for a person
- `PersonTechnology` — technology used by a person's organization

### Organization Domain
- `Organization` — a company record in the Apollo database
- `OrganizationDetails` — enriched company detail record
- `OrgDomain` — primary and secondary web domains
- `OrgSize` — headcount range and exact employee count
- `OrgRevenue` — annual revenue range
- `OrgFunding` — total funding, last round, and funding stage
- `OrgFoundedYear` — year the organization was founded
- `OrgIndustry` — industry and sub-industry classification
- `OrgTechnology` — technology stack detected for the organization
- `OrgPhoneNumber` — organization switchboard and direct phone numbers
- `OrgLocation` — headquarters city, state, country, and postal code
- `OrgSocialMedia` — LinkedIn, Twitter, Facebook, and other social URLs

### Sequences Domain
- `Sequence` — a multi-step outreach cadence definition
- `SequenceContact` — a subscriber enrolled in a sequence
- `SequenceStep` — an individual step within a sequence
- `EmailStep` — an email send step within a sequence
- `CallStep` — a call task step within a sequence
- `TaskStep` — a generic task step within a sequence
- `FollowUpStep` — a conditional follow-up step within a sequence

### Engagement Domain
- `EmailMessage` — a sent or received email message
- `Subject` — email subject line with template variable metadata
- `Body` — email body (plain text and HTML) with template metadata
- `Task` — a to-do item assigned to a user and linked to a contact or account
- `TaskType` — enum of task types (call, email, action, LinkedIn)
- `TaskOutcome` — enum of task disposition outcomes
- `Call` — a logged inbound or outbound phone call
- `CallRecord` — call recording URL, duration, and transcript reference
- `EmailThread` — grouped email conversation thread
- `EmailReply` — a reply to a sent sequence email

### CRM Domain
- `Account` — a company record in a user's CRM workspace
- `AccountOwner` — the user assigned as owner of an account
- `Deal` — an opportunity (deal) linked to an account and contact
- `DealStage` — the pipeline stage of a deal
- `DealValue` — monetary value and currency for a deal
- `Pipeline` — a sales pipeline definition
- `PipelineStage` — a stage within a sales pipeline

### Activity Domain
- `Activity` — a generic activity event for a contact or account
- `ActivityType` — enum of activity types
- `Note` — a free-text note attached to a contact, account, or deal
- `Meeting` — a calendar meeting linked to a contact and account

### Taxonomy Domain
- `Label` — a workspace label applied to contacts or sequences
- `Tag` — a user-defined tag for categorizing contacts or accounts

### Search & Filter Domain
- `Filter` — a structured search filter criterion
- `SearchParams` — aggregated parameters for a people or org search
- `SearchResult` — paginated container for search results
- `ContactSearch` — people search result set
- `OrgSearch` — organization search result set

### Enrichment Domain
- `BulkEnrich` — a bulk enrichment job record tracking status and results

### Platform Domain
- `WebhookEvent` — a delivered webhook event payload
- `APIKey` — an API key credential for workspace authentication
- `Token` — an OAuth or session token for API access

## Queries

- `searchContacts(params: SearchParams!): ContactSearch` — search the Apollo person database
- `searchOrganizations(params: SearchParams!): OrgSearch` — search the Apollo org database
- `getContact(id: ID!): Contact` — fetch a CRM contact by ID
- `getAccount(id: ID!): Account` — fetch a CRM account by ID
- `getDeal(id: ID!): Deal` — fetch a deal by ID
- `getSequence(id: ID!): Sequence` — fetch a sequence definition by ID
- `listTasks(userId: ID, contactId: ID): [Task]` — list tasks filtered by user or contact
- `listCalls(contactId: ID): [Call]` — list calls for a contact
- `listMeetings(contactId: ID): [Meeting]` — list meetings for a contact
- `getWebhookEvent(id: ID!): WebhookEvent` — fetch a webhook event by ID

## Mutations

- `createContact(input: ContactInput!): Contact` — create a CRM contact
- `updateContact(id: ID!, input: ContactInput!): Contact` — update a CRM contact
- `deleteContact(id: ID!): Boolean` — delete a CRM contact
- `createAccount(input: AccountInput!): Account` — create a CRM account
- `updateAccount(id: ID!, input: AccountInput!): Account` — update a CRM account
- `createDeal(input: DealInput!): Deal` — create a deal
- `updateDeal(id: ID!, input: DealInput!): Deal` — update a deal
- `enrollContact(sequenceId: ID!, contactId: ID!): SequenceContact` — enroll a contact in a sequence
- `removeContact(sequenceId: ID!, contactId: ID!): Boolean` — remove a contact from a sequence
- `createTask(input: TaskInput!): Task` — create a task
- `completeTask(id: ID!, outcome: TaskOutcome!): Task` — mark a task complete with outcome
- `createNote(input: NoteInput!): Note` — create a note on a contact or account
- `bulkEnrichPeople(inputs: [PersonInput!]!): BulkEnrich` — enrich up to 10 person records
- `bulkEnrichOrganizations(inputs: [OrgInput!]!): BulkEnrich` — enrich up to 10 org records

## File

- Schema file: `apollo-io-schema.graphql`
