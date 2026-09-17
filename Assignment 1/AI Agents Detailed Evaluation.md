# Comparative Evaluation: AI Agents for a Browser-Only Word to PDF Converter

## Assignment Goal

The same task was given to multiple AI app-building and coding agents:

> Build a minimal Word (`.docx`) to PDF converter. A user should upload a Word file and receive a PDF. Conversion must happen entirely inside the browser. The document must not be uploaded to a backend or conversion server. The interface should clearly communicate privacy and remain simple and responsive.

## Live Outputs

| Agent / Platform | Live Output | Observed Score |
|---|---|---:|
| Emergent | https://pdf-maker-274.preview.emergentagent.com/ | 76/100 |
| Lovable | https://local-doc-pdf.lovable.app/ | 91/100 |
| Replit Agent | https://private-word-to-pdf--laplot8.replit.app/ | 75/100 |
| Bolt | https://client-side-word-to-dmue.bolt.host/ | 86/100 |
| Vercel-hosted build | https://word-to-pdf-zeta.vercel.app/ | 93/100 |
| Zite | https://opgyzvetxq.zite.so/ | 76/100 |
| Base44 | https://local-pdf-flow.base44.app/ | 84/100 |
| OpenCode | https://word-to-pdf-yesb-eight.vercel.app/ | 90/100 |
| Google Antigravity | https://word-to-pdf-converter-gray.vercel.app/ | 93/100 |

## Additional Vercel Project Links

- `https://vercel.com/lap-lot-s-team/word-to-pdf-converter` - inspected as a project dashboard. It showed **No Production Deployment** during the review, so it is not treated as a separate runnable output.
- `https://vercel.com/lap-lot-s-team/word-to-pdf-yesb` - project dashboard associated with the OpenCode deployment; the public `word-to-pdf-yesb-eight.vercel.app` URL is used for output evaluation.

## Evaluation Method

The outputs were reviewed on 17 September 2026 using the same criteria: task fit, UI/UX clarity, privacy communication, visible feature completeness, and deployment/polish. Each category is scored out of 10 and the overall score is the category average converted to 100.

Important: this is an **output evaluation**, not a laboratory proof of security. A page can state that conversion is local, but proving that no file bytes are transmitted requires source-code review or browser network tracing. Scores therefore reflect the public implementation and how clearly it satisfies and communicates the assignment.

## Per-Agent Evaluation

### Emergent - 76/100

**Agent properties:** Agentic prompt-to-production platform for full-stack web/mobile apps, with preview, testing, deployment and integrations.

**Observed output:** Live link resolved through an Emergent iframe/preview surface. The use of a preview URL makes it look more like a development result than a final production deployment.

**Strongest feature:** Fast end-to-end app generation with a working hosted preview.

**Main limitation:** Deployment maturity is weaker than the dedicated production URLs in this comparison, and privacy-specific interface text was not fully extractable during inspection.

### Lovable - 91/100

**Agent properties:** Conversational app and website builder with live iteration, visual editing, publishing and managed hosting.

**Observed output:** The page clearly states that conversion happens in the browser, files never leave the device, and DOCX files up to 25 MB are accepted. The upload action is immediately understandable.

**Strongest feature:** Excellent privacy communication combined with a very clear drag-and-drop upload flow.

**Main limitation:** The visible interface is intentionally minimal, so advanced document controls are not part of the public surface.

### Replit Agent - 75/100

**Agent properties:** General software creation agent that can generate code, install dependencies, run applications and deploy them from the same environment.

**Observed output:** The deployed page is reachable and titled "Word to PDF". Compared with the strongest outputs, less requirement-specific information was visible to the text inspection layer.

**Strongest feature:** Strong developer environment and straightforward path from generated code to a live app.

**Main limitation:** The public-facing output communicates fewer privacy and task details on the surface available to inspection.

### Bolt - 86/100

**Agent properties:** Prompt-driven web app builder focused on fast code generation, live preview, responsive interfaces and rapid publishing.

**Observed output:** The live page title explicitly describes a "Private Browser-Based Converter", which closely matches the assignment requirement for client-side conversion.

**Strongest feature:** Strong requirement alignment and fast, focused frontend output.

**Main limitation:** The page content was JavaScript-heavy and not fully extractable, so deeper feature verification from the public surface was limited.

### Vercel-hosted build - 93/100

**Agent properties:** The generating agent was not specified in the provided information. Vercel is the deployment platform, so this row evaluates the output rather than attributing capabilities to an unknown agent.

**Observed output:** The output is branded "DocVault" and clearly states: no uploads, no servers and no tracking. It also shows DOCX support up to 30 MB and repeats that documents never leave the device.

**Strongest feature:** The clearest combination of privacy messaging, file-limit guidance and polished product-style presentation.

**Main limitation:** Agent-level properties cannot be evaluated fairly because the builder/agent name was not provided.

### Zite - 76/100

**Agent properties:** AI builder oriented toward business apps, databases, forms, workflows, websites and operational automation.

**Observed output:** The deployment is reachable as "Word to PDF | Zite". Zite is capable of broader business systems, but this task is a small single-purpose browser utility.

**Strongest feature:** Rapid deployment inside a platform that can later expand into workflows or business processes.

**Main limitation:** For this narrow client-side converter task, the platform is broader than necessary and the output exposes fewer task-specific details in text inspection.

### Base44 - 84/100

**Agent properties:** No-code AI builder with built-in backend, auth, storage, workflows, responsive design, testing and publishing.

**Observed output:** The page title explicitly identifies a private browser-based converter, showing good alignment with the requested architecture.

**Strongest feature:** Good prompt-to-app completeness with clear privacy-oriented positioning.

**Main limitation:** Base44 includes many full-stack capabilities that are unnecessary for a deliberately local-only conversion tool.

### OpenCode - 90/100

**Agent properties:** Open-source coding agent with build and read-only plan modes, provider flexibility and strong developer control through a terminal/client-server workflow.

**Observed output:** The deployed page title is "Word to PDF Converter | Private & Local", directly matching the local-processing requirement and presenting the result as a complete utility.

**Strongest feature:** Strong developer control with a clean output that keeps the privacy requirement prominent.

**Main limitation:** Unlike hosted no-code builders, deployment and project management remain more developer-driven.

### Google Antigravity - 93/100

**Agent properties:** Multi-step coding agent with reasoning, tools, browser control, artifacts and parallel agent workflows for end-to-end software tasks.

**Observed output:** The public page title is "Word to PDF | 100% Private In-Browser Converter", which is highly aligned with the assignment wording and clearly communicates the intended privacy model.

**Strongest feature:** Very strong requirement interpretation, privacy framing and polished deployment-oriented output.

**Main limitation:** The public page alone cannot prove that no file data is ever transmitted; that requires source or network-level verification.

## Overall Findings

The strongest observed outputs were the Vercel-hosted DocVault build and the Google Antigravity build, both because they communicated the local/private requirement extremely clearly and presented a polished production-style result. Lovable also performed very strongly because the page explicitly stated local browser conversion and gave a clear 25 MB DOCX limit. OpenCode combined strong privacy framing with high developer control.

Emergent, Replit, Zite and Base44 are capable broader app-building platforms, but this assignment is intentionally narrow. For such a small browser-only utility, extra full-stack features do not automatically improve the result. The most successful outputs stayed focused on one action: choose a DOCX file, convert locally, and make the privacy promise obvious.

## Deliverables

This evaluation package contains:

- `AI_Agent_Word_to_PDF_Evaluation_README.md`
- `AI_Agent_Word_to_PDF_Detailed_Evaluation.docx`
- `AI_Agent_Word_to_PDF_Detailed_Evaluation.pdf`
- `AI_Agent_Word_to_PDF_Assignment_Short.docx`
- `AI_Agent_Word_to_PDF_Assignment_Short.pdf`

## Sources Reviewed

Live application URLs are listed above. Platform capability descriptions were cross-checked against current official pages/documentation for Emergent, Lovable, Replit, Bolt, Zite, Base44, OpenCode and Google Antigravity. Review date: 17 September 2026.
