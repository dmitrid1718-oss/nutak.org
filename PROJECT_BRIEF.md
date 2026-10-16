# NuTak — canonical project brief

Saved October 16, 2026. Owner: Dmitri / Useless Instruments.
Repository: https://github.com/dmitrid1718-oss/nutak.org
Intended domain: nutak.org. Domain ownership/configuration not verified in this session.

## Product

A funny but useful AI interview rehearsal tool. It prepares people for a real job interview, using researched company and role information. It must help users answer better, not simply entertain them. Confidence, warmth and dry humor; avoid a stern examiner or an AI trying to sound clever.

User flow: nickname -> company -> position -> optional pasted resume -> readiness -> verified $1 payment -> interview. No account is intended. First name or nickname is sufficient. The resume can omit name and contact details; focus on experience, skills and education. Resume input is optional.

English / Russian is required throughout: landing page, setup, interview, notes, notices and payment information. Russian humor should be written naturally, not translated literally. Do not imply employers offer Russian-language interviews.

## Interviewers

User approved 15 distinct interviewers/configurations, one per company, all with Russian names and including men and women. These are shared-model configurations, not 15 separately trained models or subscriptions. Anya, Mila and Vera were the first agreed names; user approved the full name list. Company assignments below are provisional implementation choices, not separately approved assignments.

| Company | Interviewer | Working character |
| --- | --- | --- |
| Amazon | Anya / Аня | Dry humor, raised eyebrow, asks for specifics |
| Google | Mila / Мила | Warm, friendly, incisive follow-ups |
| Microsoft | Vera / Вера | Composed, unexpected follow-ups |
| Meta | Ivan / Иван | Direct questions |
| Apple | Irina / Ирина | Detail-oriented |
| NVIDIA | Pavel / Павел | Patient technical debugger |
| Netflix | Nina / Нина | Candid colleague |
| OpenAI | Boris / Борис | Curious skeptic |
| Anthropic | Olga / Ольга | Thoughtful challenger |
| Adobe | Katya / Катя | Creative critic |
| Salesforce | Sasha / Саша | Easy conversation, sharp listening |
| Oracle | Viktor / Виктор | Practical examiner |
| Tesla | Dmitri / Дмитрий | Resourceful engineer |
| Google DeepMind | Nikolai / Николай | Quiet researcher |
| IBM | Mikhail / Михаил | Experienced listener |

Character visual direction discussed: fitted jacket, glasses, looking over the frames; humor is mandatory. Current page uses a red chair illustration and typographic character cards; character portraits are not yet created.

Separate difficulty and humor controls. Humor targets interview absurdities, not accents, identity, nervousness or background. The assessment criteria should remain consistent across personalities.

## Money

User decision: $1 to start one interview. This supersedes earlier free-session, $2-session, and optional-contribution ideas.

Detailed feedback by email is an optional additional paid product; price is not decided. Collect email only when the user orders that report. PayPal may separately require payer information. Payment processing, fees, tax handling, refunds and delivery expectations must be settled before launch.

Use PayPal. Verify payment on the server before granting access or delivering reports; a success redirect alone is not proof. Handle duplicate notifications and retries without duplicate charges or duplicate paid entitlements. Email delivery needs an authorized transactional email provider.

AI cost estimates discussed are unmeasured and model-dependent. Budget testing first; set session limits and spending cutoffs. Avoid promising a fixed margin at $1 before measuring API usage and PayPal fees.

## Interview records and assessment

Owner requested every interview be assessed and saved in a company folder, using nickname plus a unique internal interview number. Proposed structure: company / position / interview ID. Names may repeat; a nickname must never serve as an authentication secret.

Store transcript, interview ID, nickname, company, position, timestamps, language, interviewer configuration/version and assessment. Keep provider/model and rubric versions so results can be understood later. Keep user records private; never commit transcripts, resumes, emails or payment data to this public repository.

Assessment should evaluate answers with transcript evidence, not a person's worth or hiring probability. Distinguish missing evidence from demonstrated weakness. Include specific improvements and a chance to retry.

A retention duration, deletion method, access controls and lawful launch notices remain undecided. Full resumes should not be stored by default; transcript storage may still contain personal information. Explain actual handling before live use. These are requirements for a later service, not features of this preview.

## Research

Use research/company-interview-research.md as the first evidence baseline. It includes official sources and explicit limitations. Do not call all 15 tracks researched: IBM is not covered, Apple lacks verified interview process details, and Google/Meta need more verification.

Match company, position, level and stage where possible without burdening the first screen. Company culture is not proof of a hiring rubric. Generated questions are simulations. No affiliation or endorsement, no leaked-question claims, no guarantee of employment. Recheck company sources before enabling each live track.

## Validation direction

Owner knows two potential testers. Build and test one complete interviewer first, starting with Anya/Amazon, before implementing 15 live configurations. Ask testers what they would answer differently in a real interview afterward. Check usefulness, humor, English/Russian quality, latency and actual cost.

## Current implementation

index.html is a self-contained bilingual static page with 15 character profiles, company selector, nickname/position validation, optional resume, independent humor/difficulty controls, and a scripted preview dialog. No external assets or dependencies. No network calls, analytics, cookies, application storage, payment or email collection.

The page clearly labels itself as in development. It does not simulate a completed payment or pretend scripted content is a live AI response. Form values remain only in page memory; browser form restoration is outside the app's control.

## Outstanding setup and work

- User has not yet chosen secure creation/reuse of an OpenAI API key. No local key was found. Required credential decision remains pending; no key was created or used.
- No API-backed code is implemented.
- PayPal merchant setup/link and automatic verification are pending.
- Private database/storage, retention/deletion policy, and transactional email service are pending.
- Website hosting is not configured by this change. A Vercel repository-filtered project lookup returned no matching project.
- Domain configuration not verified.
- First research pass is saved; further company/role research remains.
- Live interview length, feedback price, and user-visible assessment details remain to be decided.

## Working preferences

Keep the experience simple. Nickname only, no required account. Make it funny and useful. User said to challenge weak assumptions. Save source, locations and decisions so future work can continue from one canonical repository.
