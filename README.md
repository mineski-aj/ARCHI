# ARCHI USER GUIDE

**AI-Driven Procurement Manager \& Financial Strategist**
*Operations Department · v4.0 · Claude · Gemini · ChatGPT*

\---

## WHAT IS ARCHI?

Archi is an AI-powered procurement and financial operations assistant for the entire Operations Department. It builds Cost Estimates, closes projects, analyzes vendors, handles compliance requests, and builds operational tools — all while enforcing the department's **36% Gross Profit mandate** on every output.

**Who can use it:** Tribe Leads, Project Managers, and Associates across all four Tribes.
**Chain of command:** Tribe Leads → AJ (Head of Operations) → Nate (General Manager)

> Each session is private. Your project data is not visible to other Tribes unless you share it explicitly within the session.

\---

## HOW TO START

Every time you open a new chat on any AI platform:

**Step 1** — Upload **`Archi\_Global\_Procurement\_Initialization.md`**
*(or paste the full contents of `ARCHI\_System\_Prompt\_v4.md` as your first message)*

**Step 2** — Type: *"Initialize Archi."*

**Step 3** — Introduce yourself before giving any task:

> \*"I'm \[Name], \[role] under \[Tribe Name]. I need help with \[task]."\*

Archi will confirm it is online and ask for exactly what it needs — nothing more.

\---

## WHAT ARCHI CAN DO

\---

### 1 · Build a Cost Estimate or Client Quotation

Provide a raw RFP, production brief, or a list of vendor quotes — even if unorganized.

**Archi needs:**

* Event name and scope
* Exact ingress / event / egress dates and times
* Venue name
* Vendor quotes (raw is fine)
* Client budget ceiling *(if known)*

**Archi will deliver:**
A fully margin-protected CE matrix with Internal COGS, Markup, and Client Quote columns — with the 0.64 divisor applied to every line and hidden costs (venue tap-in fees, overnight meal tiers, trucking surcharges) already injected.

\---

### 2 · Project Closing \& Reconciliation

Cross-check a completed project's approved CE against actual POs and PRs to get final GP% and flag all discrepancies.

**Two access tiers:**

|Tier|What you get|How to access|
|-|-|-|
|**Basic**|Reconciliation output generated directly in chat — CE structure mirrored, status tags, financial summary (Scenario A \& B), export as Excel or CSV|Available to all users — upload CE + PO CSV + PR CSV and ask Archi|
|**Comprehensive Dashboard**|Full interactive tool with drag-and-drop uploads, live filters, and advanced export|Request access from **Frances Arreglado (Tencent Tribe Lead)**|

**Files needed for Basic reconciliation:**

|File|Format|Where to Get It|
|-|-|-|
|Cost Estimate|.xlsx|Your project CE — filename must contain project code e.g. `2025TEG-P0307`|
|Purchase Orders|.csv|Lark → Procurement Master Sheet → Export|
|Procurement Requests|.csv|Lark → PR Tracker → Export|

**Status tags on every line:**

|Tag|What It Means|What to Do|
|-|-|-|
|✅ MATCHED|PO confirmed, amount within CE|Nothing — fully reconciled|
|🟡 OVERRUN|PO confirmed, actual exceeds CE|Explain variance to Tribe Lead|
|🔵 PENDING PO|PR in CE but no PO found in Lark|Confirm if paid, cancelled, or still open|
|⬜ NO PR FILED|CE item processed via CA or Internal|Confirm liquidation receipt|
|🔴 NO CE LINE|PO exists with no CE counterpart|Justification or change order required|
|🔶 ISOLATED|Inter-company / sister company billing|Excluded from COGS — fund transfer, not vendor spend|

> \*\*Important — TEG Group sister companies:\*\* Billings from GG Company Inc. or PDEI to \*\*Pillar Digital E-Commerce Inc.\*\* (Mineski Philippines) or \*\*APEX Franchise Ventures OPC\*\* are inter-company fund transfers — not third-party vendor procurement. Archi will automatically flag and isolate these entries from all benchmarking, rate analysis, and GP calculations. Additional sister companies will be declared as they are identified.

**CE column reference** *(standard format — Archi auto-detects these):*

|Col|Field|Col|Field|
|-|-|-|-|
|A|Category|K|Base Price|
|D|Particular|O|Cost Estimate (COGS)|
|E|Quantity|V|PR Number|
|F|Frequency|W|PO / CA Number|
|H|Unit Price|||

\---

### 3 · Vendor Analysis \& Negotiation

Provide the vendor name, category, quoted amount, and any prior usage. Archi will benchmark it against verified actuals from the Andon Board, flag overpricing, calculate GP impact, and recommend a counter-offer or alternative.

> Archi will not use sister company billings (Pillar Digital, APEX, etc.) as benchmarks for third-party vendor negotiations.

\---

### 4 · File Fixes

Attach a PDF, Excel, or CSV file and describe what needs to change — typo, formula error, layout update, column remap. Archi returns the corrected file.

\---

### 5 · Operational Tools \& Dashboards

Describe any procurement or financial workflow you want automated. Archi will design, build, and document it — and generate a handoff file so it can be continued in any future session.

\---

### 6 · Compliance, Billing \& Archival

|Scenario|How Archi Handles It|
|-|-|
|Billing dispute with no signed CE|Bills based on actual verified consumption only|
|Client requests physical ORs from past fiscal years|Issues formal protocol response — redirects to audited Procurement Liquidation Sheets|
|Personnel document must be shared externally|Enforces DPA 2012 compliance — redacts names, shows roles and departments only|

\---

### 7 · Contributing Data to Archi's Baseline

Archi improves its benchmarks by learning from files across all Tribes. Any Tribe Lead, PM, or Associate can contribute CEs, actuals, or vendor data to expand the reference database.

**How to contribute:**
Upload the file and say: *"This is from \[Tribe Name] — add to baseline."*

Archi will index rates, vendor patterns, and cost ranges for cross-tribe benchmarking. Project-specific details remain within the contributing Tribe's session — only aggregated cost data is retained for general reference.

\---

## GROUND RULES

|Rule|What It Means|
|-|-|
|**36% GP is a hard floor**|If a client pushes back on price, Archi finds scope reductions — never margin reductions|
|**No building on incomplete data**|Missing variables get flagged immediately. Archi will not estimate around gaps|
|**Sister company billings are isolated**|Pillar Digital, APEX, and other declared TEG Group entities are excluded from all vendor analysis and GP calculations|
|**Scenario B is internal**|Share Scenario A with leadership. Use Scenario B for internal risk tracking only|
|**All NO CE LINE items must be resolved before close**|Every red flag needs a written justification or change order — not a verbal explanation|
|**Generate a handoff for multi-session work**|At the end of any long session, say: *"Generate a handoff MD for this session."*|

\---

## ANDON BOARD — LIVING REFERENCE

The Andon Board (Mineski PH Procurement Order CSV from Lark) is the department's living cost reference. Archi uses it to benchmark vendor rates, detect overpricing, and identify cross-tribe leverage.

**To activate for a session:** Upload the latest export and say: *"This is the current Andon Board."*

**Update schedule:** The file is updated weekly or biweekly. **Every Monday at 1:00 PM**, Frances (Tencent Tribe Lead) or AJ (Head of Operations) should upload the latest Andon Board export to the project folder. Archi will prompt this reminder at the start of any Monday session where an updated file has not yet been provided.

\---

## PLATFORM NOTES

|Platform|How to Initialize|File Uploads|Interactive Dashboards|
|-|-|-|-|
|**Claude**|Upload MD or paste prompt|✅ Excel, PDF, CSV|✅ Fully interactive — runs live in chat|
|**Gemini**|Upload MD or paste prompt|✅ Supported|⚠ Outputs as code or text|
|**ChatGPT**|Upload MD or paste prompt|✅ Supported|⚠ Outputs as code or text|

> For the Comprehensive Reconciliation Dashboard, \*\*Claude is required\*\* — it renders the interactive tool natively in the chat window. Contact Frances Arreglado for access.

\---

*Operations Department · Maintained by the Tribe Leads
For prompt updates, tool access, or issues — contact your Tribe Lead or AJ.*

