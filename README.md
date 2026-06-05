# Apollo.io (apollo-io)

Apollo.io is a sales intelligence and engagement platform combining a 270M+ contact database with email and call sequencing. The Apollo REST API exposes people search & enrichment, organization search & enrichment, contacts, accounts, deals, sequences, email accounts, calls, tasks, meetings, lists, and webhooks.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/apollo-io/refs/heads/main/apis.yml)

## Tags

- Sales Intelligence
- Prospecting
- Engagement
- B2B Data
- Enrichment
- SaaS

## Timestamps

- **Created:** 2026-05-08
- **Modified:** 2026-05-19

## APIs

### Apollo People Search API

Search Apollo's 270M+ person database by title, location, seniority, function, industry, technology stack, and other filters. Returns matching people with optional enrichment fields.

#### Tags

- People
- Search
- Prospecting

#### Properties

- [Documentation](https://docs.apollo.io/)
- [API Reference](https://docs.apollo.io/reference/people-search)
- [OpenAPI](openapi/apollo-io-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/apollo-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/apollo-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Apollo Organization Search API

Search Apollo's organization database by industry, headcount, revenue, technology stack, location, and funding stage.

#### Tags

- Organizations
- Companies
- Search

#### Properties

- [API Reference](https://docs.apollo.io/reference/organization-search)
- [Postman Collection](collections/apollo-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/apollo-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Apollo People Enrichment API

Enrich a known person record by email, LinkedIn URL, name + company, or other identifiers; returns work email, mobile, title, social profiles, and tenure.

#### Tags

- People
- Enrichment

#### Properties

- [API Reference](https://docs.apollo.io/reference/people-enrichment)
- [Postman Collection](collections/apollo-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/apollo-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Apollo Organization Enrichment API

Enrich a known organization by domain or LinkedIn URL; returns headcount, industry, revenue, funding, technologies, and location.

#### Tags

- Organizations
- Enrichment

#### Properties

- [API Reference](https://docs.apollo.io/reference/organization-enrichment)
- [Postman Collection](collections/apollo-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/apollo-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Apollo Bulk People Enrichment API

Enrich up to 10 person records in a single API call to reduce round-trip and credit cost.

#### Tags

- Bulk Enrichment
- People

#### Properties

- [API Reference](https://docs.apollo.io/reference/bulk-people-enrichment)
- [Postman Collection](collections/apollo-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/apollo-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Apollo Bulk Organization Enrichment API

Enrich multiple organizations in a single API call.

#### Tags

- Bulk Enrichment
- Organizations

#### Properties

- [API Reference](https://docs.apollo.io/reference/bulk-organization-enrichment)
- [Postman Collection](collections/apollo-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/apollo-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Apollo Contacts API

Manage contacts in your Apollo CRM workspace — create, update, delete, and bulk-import contacts with custom fields and tags.

#### Tags

- Contacts
- CRM

#### Properties

- [API Reference](https://docs.apollo.io/reference/contacts)
- [Postman Collection](collections/apollo-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/apollo-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Apollo Accounts API

Manage accounts (companies) in your Apollo CRM with stage, ownership, and custom fields.

#### Tags

- Accounts
- CRM

#### Properties

- [API Reference](https://docs.apollo.io/reference/accounts)
- [Postman Collection](collections/apollo-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/apollo-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Apollo Deals API

Manage deals (opportunities) attached to accounts and contacts, including stage, value, probability, and custom fields.

#### Tags

- Deals
- Opportunities
- Pipeline

#### Properties

- [API Reference](https://docs.apollo.io/reference/deals)
- [Postman Collection](collections/apollo-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/apollo-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Apollo Sequences API

Manage outreach sequences (cadences) and add or remove contacts as sequence subscribers; trigger sends and pause/resume schedules.

#### Tags

- Sequences
- Cadences
- Outreach

#### Properties

- [API Reference](https://docs.apollo.io/reference/sequences)
- [Postman Collection](collections/apollo-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/apollo-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Apollo Email Accounts API

Manage connected email accounts (Gmail / Outlook / SMTP) used for outbound sequence sends and inbox sync.

#### Tags

- Email Accounts
- SMTP

#### Properties

- [API Reference](https://docs.apollo.io/reference/email-accounts)
- [Postman Collection](collections/apollo-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/apollo-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Apollo Emails API

Read sent / received email metadata and tracking events (open, click, reply, bounce) for sequence emails.

#### Tags

- Emails
- Tracking

#### Properties

- [API Reference](https://docs.apollo.io/reference/emails)
- [Postman Collection](collections/apollo-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/apollo-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Apollo Calls API

Log inbound and outbound calls with duration, recording URLs, transcripts, and disposition outcomes.

#### Tags

- Calls
- Telephony

#### Properties

- [API Reference](https://docs.apollo.io/reference/calls)
- [Postman Collection](collections/apollo-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/apollo-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Apollo Tasks API

Manage user tasks tied to contacts and accounts.

#### Tags

- Tasks

#### Properties

- [API Reference](https://docs.apollo.io/reference/tasks)
- [Postman Collection](collections/apollo-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/apollo-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Apollo Meetings API

Manage meetings booked via Apollo's Meetings (scheduling) feature and synced from connected calendar accounts.

#### Tags

- Meetings
- Scheduling

#### Properties

- [API Reference](https://docs.apollo.io/reference/meetings)
- [Postman Collection](collections/apollo-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/apollo-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Apollo Custom Fields API

Define and read custom field schemas across people, organizations, contacts, accounts, and deals.

#### Tags

- Custom Fields
- Metadata

#### Properties

- [API Reference](https://docs.apollo.io/reference/custom-fields)
- [Postman Collection](collections/apollo-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/apollo-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Apollo Lists API

Manage saved lists (static and dynamic) for segmenting people and accounts and feeding them into sequences and dialer queues.

#### Tags

- Lists
- Segments

#### Properties

- [API Reference](https://docs.apollo.io/reference/lists)
- [Postman Collection](collections/apollo-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/apollo-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Apollo Tags API

Read, create, and apply tags to contacts and accounts for categorization and filtering.

#### Tags

- Tags

#### Properties

- [API Reference](https://docs.apollo.io/reference/tags)
- [Postman Collection](collections/apollo-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/apollo-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Apollo Users API

Manage users (sales reps, managers) and their roles within the Apollo workspace.

#### Tags

- Users

#### Properties

- [API Reference](https://docs.apollo.io/reference/users)
- [Postman Collection](collections/apollo-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/apollo-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Apollo Analytics API

Pull aggregated activity, sequence performance, dialer, and pipeline analytics for reporting use cases.

#### Tags

- Analytics
- Reporting

#### Properties

- [API Reference](https://docs.apollo.io/reference/analytics)
- [Postman Collection](collections/apollo-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/apollo-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Apollo API Usage API

Read your workspace's API usage and remaining credit balance across hourly, daily, and monthly windows.

#### Tags

- Usage
- Credits

#### Properties

- [API Reference](https://docs.apollo.io/reference/api-usage)
- [Postman Collection](collections/apollo-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/apollo-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Apollo Webhooks API

Subscribe to Apollo events (contact.created, sequence.added, email.opened, call.completed) for downstream automation.

#### Tags

- Webhooks
- Events

#### Properties

- [API Reference](https://docs.apollo.io/reference/webhooks)
- [Postman Collection](collections/apollo-io.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/apollo-io.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/apolloio)
- [Website](https://www.apollo.io/)
- [Documentation](https://docs.apollo.io/)
- [API Reference](https://docs.apollo.io/reference)
- [Pricing](https://www.apollo.io/pricing)
- [Login](https://app.apollo.io/)
- [Status Page](https://status.apollo.io/)
- [Blog](https://www.apollo.io/blog)
- [Support](https://knowledge.apollo.io/)
- [GitHub Organization](https://github.com/apolloio)
- [Privacy Policy](https://www.apollo.io/privacy-policy)
- [Terms of Service](https://www.apollo.io/terms)
- [Authentication](https://docs.apollo.io/reference/authentication)
- [Rate Limits](https://docs.apollo.io/reference/rate-limits)
- [Webhooks](https://docs.apollo.io/reference/webhooks)
- [Plans](plans/apollo-io-plans-pricing.yml)
- [Rate Limits](rate-limits/apollo-io-rate-limits.yml)
- [Fin Ops](finops/apollo-io-finops.yml)
- [Features](undefined)
- [Integrations](https://www.apollo.io/partners)
- [M C P Server](https://github.com/apolloio/apollo-mcp-plugin)
- [L L Ms Txt](https://docs.apollo.io/llms.txt)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
