# AI-Assisted Client Operations App

## Context

The Sales team has created a static HTML prototype for a Client Operations Portal. The prototype has two screens:

1. Client Database - the main landing page for customer, subscription, agreement, and billing information.
2. Agreement Intake - a new customer intake flow for uploading or entering a signed client agreement.

Sales wants this turned into a functional internal application. They also want a safe workflow where Sales can request app changes through a chat-based agent, preview those changes in UAT, and promote approved changes to production.

Use the provided `prototype/client-operations-portal.html` as your starting point. You may keep the UI, refactor it, split it into routes, replace it with a framework, or improve it as you see fit. Preserve the basic product intent.

## Deliverable

Upload a private 5-8 minute demo video to YouTube, Dailymotion, or the video hosting service of your choice, and send us the link.

No repository, README, deployment URL, or written document is required. In the video, show what you built and briefly explain key tradeoffs.

## What to Build

### 1. Functional Client Database

Create a working version of the Client Database page.

At minimum, users should be able to:

- View client records.
- Search or filter clients.
- Navigate to the new customer intake flow.
- See meaningful client status and subscription information.

### 2. Functional New Customer Intake

Create a working intake flow based on the Agreement Intake page.

At minimum, users should be able to:

- Start a new customer intake.
- Upload or simulate uploading an agreement.
- Review extracted customer or agreement fields.
- Confirm the record.
- Add the new customer to the Client Database.

You may simulate document extraction. For example, a fake upload can produce extracted fields such as client name, country, feed type, agreement date, account owner, contract value, and status.

### 3. Sales Change-Request Agent Workflow

Build or simulate a workflow where a Sales user can request changes through a chat interface.

The chat interface may be Teams, Slack, Telegram, WhatsApp, Google Chat, Discord, or a simulated in-app chat.

Example Sales request:

> Add an Account Owner column to the Client Database and let me filter by owner.

The workflow should show:

- Sales submitting a request in chat.
- The agent clarifying or summarizing the requirement.
- A proposed change being created.
- The proposed change appearing in a UAT or staging view.
- Sales approving or rejecting the UAT change.
- An approved change being promoted to production.

### 4. UAT to Production Flow

Demonstrate a clear separation between requested, staged, approved, and live changes.

At minimum, show:

- UAT or staging preview.
- Approval action.
- Production promotion action.
- Basic audit trail showing who requested the change, what changed, when it happened, and approval status.

### 5. Bonus: Rollback

Show how Sales or an admin could roll back a bad production change.

This can be a real implementation or a credible simulation, but the demo should make the rollback behavior clear.

## Guidance

You may use any stack, framework, database, LLM, hosting provider, or chat platform.

You may simulate external systems such as CRM, billing, Teams, Slack, WhatsApp, deployment tooling, or LLM calls. Simulations are acceptable as long as the workflow is clear and believable.

Focus on product judgment, safe automation, and an end-to-end working flow. We care more about how you think through the system than about pixel-perfect UI polish.

## Timebox

Suggested timebox: 4-6 hours.

Please do not spend more than 8 hours.

## Evaluation Criteria

We will evaluate the demo on:

- Product judgment: Does the workflow make sense for non-technical Sales users?
- Functional execution: Does the app work beyond the static HTML?
- AI and agent design: Is the agent practical, safe, and auditable?
- UAT and production workflow: Is there a clear path from request to staged preview to production?
- Simplicity: Is the solution appropriately scoped for a take-home?
- Demo quality: Can you explain tradeoffs clearly?
- Bonus: Is rollback supported or convincingly designed?

## Suggested Demo Structure

1. Start on the Client Database page.
2. Show search, filtering, or client record behavior.
3. Click Intake New Customer.
4. Simulate agreement upload or manual intake.
5. Confirm the extracted data and add a customer to the database.
6. Open the Sales change-request chat.
7. Request a UI or data change.
8. Show the change in UAT.
9. Approve and promote the change to production.
10. Bonus: roll back the change.
