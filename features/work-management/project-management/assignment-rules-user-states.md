# Assignment Rules & User States  
## When project management becomes a process

---

In @@name, Assignment Rules and User States turn work management from “we organize and assign tasks” into a repeatable process.
Cases reach the right people through explicit routing rules.
Statuses stop being interpretive and become a shared language for teams, managers, and reporting.

### Why this matters

Even when projects are well structured and Cases are clearly described, everyday work raises the same operational questions.
Who takes ownership of this Case now.
When is a Case actually ready, and when is it waiting.
What does a status mean in practice, not just in words.
How do we avoid manual assignment and constant clarifications.

This is the moment where project management moves from a plan to a predictable flow of work.
The goal is not to add bureaucracy.
The goal is to reduce “hidden decisions” and make routing and progress explicit.

---

### Key capabilities

#### 1) Assignment Rules — automated work distribution

Assignment Rules define how and to whom new or updated Cases are assigned without manual intervention every time.
Instead of relying on a manager’s memory or constant “who takes this” messages, @@name applies rules that the organization has defined upfront.

Rules can be evaluated based on a practical set of Case attributes.
This includes project context (such as project, area, milestone, type, or category) and also progress context (System State and User State).
Rules can also use business context such as the Stakeholder Party, so routing can follow “for whom is this work” and not only “what kind of work is it”.

When multiple rules match, @@name resolves the conflict deterministically.
Rules have priority, and when priorities are equal, rule ordering acts as a tie-breaker.
This makes routing stable and explainable, which matters when teams grow and when processes are audited or reviewed later.

Assignment itself can reflect how the organization operates.
A Case can be routed to a specific person.
It can also be routed to a responsible role or team logic, such as the responsible person for the project or for the project area.
This does not replace management decisions.
It removes repetitive coordination and keeps responsibility visible at the point where work enters the system.

**Micro-scenario (Assignment Rules).**
A new Case is created in a client implementation project with category “Testing”.
The Case enters a “Ready” System State with a User State like “For review”.
An Assignment Rule routes it to the reviewer role or a specific QA user.
When the User State changes to “Ready for execution”, another rule routes the same Case to the executor role or the delivery team.
The handover is explicit and recorded as part of the Case, rather than happening in chat.

Where this delivers the most value is predictable.
It helps larger teams with multiple roles.
It helps repetitive work where routing patterns repeat every day.
It helps request intake and operational flows where new Cases arrive continuously.
It helps service and support models where response time depends on fast routing to the right owner.

#### 2) User States — a shared language for real progress

Status words often sound clear until they mean different things to different people.
“In progress” may mean active execution for one person, “we will start soon” for another, and “we are blocked” for a third.
User States solve this by letting the organization define business-meaningful sub-stages that fit the way teams actually work.

In @@name, it helps to separate two concepts.
**System States** are the default, predefined lifecycle phases a Case moves through.
They describe the main flow from intake and preparation to execution and completion.
**User States** are custom sub-stages that add granularity inside a System State.
They let teams express what is really happening without inventing new parallel workflows or relying on free-text explanations.

User States are linked to a specific System State.
They can also be made applicable only for specific Case Categories.
This prevents a “one-size-fits-all” status list and keeps the language relevant to the kind of work being done.
The outcome is simple and practical.
A Case can be in the same System State across the organization, while still carrying the precise business sub-stage that tells the real story.

**Micro-scenario (User States).**
Two Cases are both in the “Waiting” System State.
One has a User State “Waiting for customer information”.
The other has a User State “Waiting for internal approval”.
Both are “waiting”, but the next action, the expected owner, and the management interpretation are different.
Because the distinction is explicit, reporting and daily coordination stop treating both as the same kind of delay.

---

### How it works (high level)

#### Assignment Rules (high level)

When a Case is created, or when key attributes change, @@name evaluates the active Assignment Rules that match the Case context.
Rules can match on project-related attributes and on progress-related attributes, including System State and User State.
If more than one rule matches, @@name selects the rule deterministically using priority and rule ordering.
The result is predictable routing that does not depend on who happened to notice the Case first.

#### System States vs User States (high level)

System States provide the main, shared lifecycle of a Case.
User States refine what “work stage” means inside that lifecycle, using the organization’s own language.
Because User States are linked to System States and can be constrained by Case Category, teams can achieve clarity without turning the process into a heavy methodology.

---

### Use cases

Assignment Rules and User States are especially valuable for service and support teams, where intake is continuous and fast routing matters.
They help organizations with a steady flow of new Cases, where manual assignment becomes a bottleneck.
They support teams with clearly separated roles, where handovers should be explicit and repeatable.
They help companies that want process without micromanagement, because control comes from shared rules and shared meaning, not from constant manual interventions.

Whether for projects, services, or internal coordination, rules and states reduce dependency on individual people.
They make the process understandable even when priorities shift, teams expand, or new colleagues join.

---

### Business benefits

By using Assignment Rules and User States, businesses reduce manual coordination and routine task routing.
They shorten the time from “Case created” to “Case owned”, which improves responsiveness in operational work.
They make accountability clearer because responsibility and real work stage are visible on the Case itself.
They reduce operational noise and “bouncing” because handovers are driven by rules and shared status meaning.
They keep the working model predictable as teams grow and change, because the process is defined explicitly, not carried only in people’s habits.

---

### Continue exploring Project Management

**Back to the main topic:**  
[Project Management in @@name](index.md)

**Read more about:**  
[Project Types, Case Categories & WIP Limits — managing flow and capacity](types-case-categories-wip-limits.md)

**Start from the foundation:**  
[Cases — where tasks turn into real work](cases.md)

