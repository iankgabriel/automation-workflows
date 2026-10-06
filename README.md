# Automation Workflows

Workflow automations I've built across Make, n8n, Zapier, and GoHighLevel. Each folder has the problem it solves, how it works, screenshots, and the exported workflow file where the platform allows it.

I'm Ian Kennedy Gabriel, an AI Automation Specialist at IKG Digital. Before automation, I spent 8 years in video editing and production, and I bring the same habits to every build: break the work into small steps, test the edge cases, and make sure it holds up before it goes live.

**Portfolio site:** [ikgdigital.com](https://www.ikgdigital.com)  
**LinkedIn:** [linkedin.com/in/ian-kennedy-gabriel](https://www.linkedin.com/in/ian-kennedy-gabriel)


## Make

Workflows built in Make, using Routers for branching and the Iterator and Aggregator pair to combine data from more than one source.

| Project | What it does |
|---|---|
| [AI Inbox Triage & Routing](make/ai-inbox-triage) | Reads every incoming message, labels it as Sales, Support, or Spam, then drafts a reply and posts it to the right Slack channel. Spam is filtered out before the reply step, so it never costs anything to process. |
| [Invoice/Document Processing & Validation](make/invoice-document-processing) | Checks each incoming invoice against a Google Sheet of purchase orders, then marks it as approved, flags a price mismatch, or reports a missing PO. |
| [Scheduled Multi-Source Reporting Pipeline](make/scheduled-reporting-pipeline) | Runs every morning, pulls data from two public APIs, combines it into one summary, logs it to a Google Sheet, and posts a short digest in Slack. |

## n8n

Workflows built in n8n, ranging from simple routing to an AI agent that answers questions from its own knowledge base.

| Project | What it does |
|---|---|
| [AI Inbox Triage & Routing](n8n/ai-inbox-triage) | The same labeling and routing idea as my Make version, rebuilt in n8n with a Switch node and its built-in Slack integration. |
| [Invoice/Document Processing & Validation](n8n/invoice-document-processing) | Looks up each invoice in a Google Sheet of purchase orders and sends it down a Valid, Discrepancy, or Missing branch, including the case where no PO exists at all. |
| [AI Research Agent (RAG-grounded)](n8n/ai-research-agent-rag) | An AI agent that searches a small knowledge base before it answers, says so when the answer isn't there, and remembers earlier questions within the same conversation. |

## Zapier

Zaps built with Paths, Filters, and Code by Zapier, solving the same kinds of problems within Zapier's more structured setup.

| Project | What it does |
|---|---|
| [AI Inbox Triage & Routing](zapier/ai-inbox-triage) | Labels each incoming message as Sales, Support, or Spam, then uses Paths to draft a reply and alert the right Slack channel. Spam skips the reply step entirely. |
| [Invoice/Document Processing & Validation](zapier/invoice-document-processing) | Checks each invoice against a Google Sheets record and routes it as approved, mismatched, or missing, using simple logic with no AI involved. |
| [Multi-Path Support Ticket Router](zapier/support-ticket-router) | Filters out obvious noise, scores each remaining ticket for urgency and topic, and sends urgent issues to a different Slack channel than routine ones. |

## GoHighLevel

GoHighLevel builds covering lead follow-up driven by tags, a missed-call reply that changes with the time of day, and a Zapier connection that copies pipeline updates into a spreadsheet.

| Project | What it does |
|---|---|
| [Automated Lead Response](gohighlevel/automated-lead-response) | Follows up with new leads using tags and timed waits, from the first text message all the way to a booked appointment. |
| [Missed Call Text-Back](gohighlevel/missed-call-text-back) | Texts back every missed call within moments, with different wording during and after business hours, and adds the caller to the pipeline as a new opportunity. |
| [Pipeline-to-Sheet Lead Sync](gohighlevel/pipeline-to-sheet-sync) | Watches for pipeline stage changes in GoHighLevel and writes the lead's details into a Google Sheet, so there's always an up-to-date copy outside the CRM. |

## A note on the exported files

Webhook URLs, API keys, sheet IDs, email addresses, and connection IDs have been replaced with placeholders like `YOUR_WEBHOOK_URL`. To run a workflow, import it and connect your own accounts.

## Certifications

- Make Academy: Foundation, Basics, and AI Automation Explorer
- Google AI Professional Certificate

## Contact

Email: ian.kennedy.gabriel@gmail.com  
WhatsApp: +63 927 129 1980
