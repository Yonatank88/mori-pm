# PM Foundations
### Product Management Basics Program
*Built on the MBL learning method*

---

## Program Curriculum

### Weekly Content

The following materials are intended for reading **before** each meeting:

| Week | Learning Unit | Page |
|------|--------------|------|
| 1 | **The Product Manager's Job and Methods** | – |
| 2 | **User Flows** — Mapping the User's Journey | – |
| 3 | **Needs & Requirements** — Problem Framing and Requirements Gathering | – |
| 4 | **Specification** — User Stories and the Single-Page Spec | – |
| 5 | **Project Management** — Prioritization and Working with Developers | – |

### Recommended Further Reading

1. *Inspired* — Marty Cagan
2. *The Goal* — Eliyahu M. Goldratt
3. *The Lean Startup* — Eric Ries

---

## Structure of the Weekly Meetings

Meetings take place once a week, for two hours.

### Preparation Before Each Meeting

1. Go over the materials of the relevant unit (about one hour).
2. Each chapter opens with the **pre-reading** — this is the main thing. Don't leave it to the last minute.
3. After the reading you will find **guiding questions** to help process the material and locate your gap. You don't have to answer them — you can write out answers if it helps, or just keep them in mind while reading.
4. Each chapter closes with the **Weekly Challenge** — use the full week between meetings to practice it on real work. Its output is that week's **draft artifact** (a problem statement, a user flow, a spec…), built on a real, live project — the centerpiece of the meeting.

### Preparing the Artifact for the Meeting

Use the following questions:

1. Relative to this week's material — where is the gap between the method as described and my current practice?
2. Where does this show up concretely? Bring a real example: what happened, when, where, and with whom.
3. What would you like to achieve? What would count as success? What question do you want to bring to the discussion?

### The Meeting Itself

**1. Check-in** *(10%)*
What's on my plate for the week, what project I'm collaborating on this week, and where is HK's focus this week.

**2. Discussion of the material** *(20%)*
Key concepts from the reading. What resonated, what raised questions, where each of us sees the gap between the method and our current practice — with a concrete example.

**3. Artifact workshop** *(50%)*
Deep dive into the draft prepared in advance.
The presenter walks through the artifact and the real case behind it: what is the project, who are the users and stakeholders, where they got stuck.
Then: live revision of the artifact based on the feedback.

**4. Weekly challenge briefing** *(10%)*
What will be practiced on the job this week, and on which project.

**5. Check-out** *(10%)*
One sentence: what am I taking from today's meeting? What commitment am I making for the coming week?

---

# Unit 1 — The Product Manager's Job and Methods

**Pre-reading:**

1. [WHAT Does a Product Manager Actually Do?](https://stephenanderson.medium.com/what-does-a-product-manager-actually-do-bee1d853f420) — Stephen P. Anderson

**Guiding questions** *(optional — answer if it helps, or just hold them in mind while reading)*:

1. Who are my customers as the digital lead at HK? (participants? alumni? program directors? donors?)
2. What process do I currently have before committing to a solution?
3. How do I define a business outcome at HK?
4. What transparency do I provide my stakeholders into the product process?

**Weekly Challenge:**

Start a **running request log** — and backfill it.

1. **Backfill:** Go through all the requests you've received recently (email, Slack, meetings, hallway conversations) and add them to the log. For each one, determine: did it arrive as a **feature** (a ready-made solution) or as a **problem**?
2. **Keep it running:** During the coming week, add every new request that lands on your desk as it arrives.

Map it as a table:

| Requester Name | Request | Request Type (feature / problem) |
|----------------|---------|----------------------------------|
| | | |
| | | |

Don't act differently yet — just observe and log. Bring the table to the next meeting.

---

# Unit 2 — User Flows

**Goal of this unit:** Learn to map the *complete* process a user goes through — including everything that happens behind the scenes (back office: staff actions, systems, automations) to make each step possible.

**Pre-reading** *(in this order)*:
1. **Start here:** [User Journeys vs. User Flows](https://www.nngroup.com/articles/user-journeys-vs-user-flows/) — Nielsen Norman Group.
   Read this first to understand the difference between a user *journey* and a user *flow*. **Note: neither of these is this week's task.** They are the vocabulary. Our task is the next level — mapping the full process *including what happens behind the scenes*:
2. [Service Blueprint](https://blog.uxtweak.com/service-blueprint/) — UXtweak. **This is the task** — the map of the entire process: what the user experiences, alongside everything that happens behind the scenes to make it possible.
   *Note: disregard the "physical evidence" lane — it's not important for our purposes. Focus on the user's actions, frontstage, backstage, and support processes.*
3. [Swimlanes](https://ux-prasad.medium.com/swimlanes-ccfb16632e9a) — Prasad Kantamneni. Short read with some nice practical pointers for building the map itself.

**Weekly Challenge:**

**Step 1 — List the PIF registration flow:** Write a simple, ordered list of everything a student goes through in the **PIF registration flow** — from first contact **until the user completes registration**. Every step, in order, one line each — including what happens behind the scenes.
**Scope:** participant-facing process only. Anything that is for facilitators — assume it has been taken care of, and leave it out.

*Example — a person buying a burger at McDonald's:*

1. Customer arrives at the restaurant
2. Customer orders at the self-service kiosk
3. Order appears on the kitchen screen (beep)
4. Cook makes the burger
5. Burger is sent to the counter
6. Customer picks it up from the counter
7. Customer eats at the table

**Step 2 — Turn the list into a service blueprint:** Sort each step from your list into 3 lanes:
1. **User interaction** — everything the user touches: forms, emails, pages
2. **System** — what happens automatically behind the scenes (CRM)
3. **Team** — steps handled by people on the team

*The McDonald's example as a blueprint:*

```
TIME ──────────────────────────────────────────────────────────────────▶

USER        ┌────────┐   ┌───────────┐                ┌─────────┐   ┌────────┐
(kiosk,     │ Arrive │──▶│ Order at  │                │ Pick up │──▶│ Eat 🍔 │
forms)      └────────┘   │ kiosk     │                │ counter │   └────────┘
                         └─────┬─────┘                └────▲────┘
............................. │ ..........................│............
SYSTEM                   ┌────▼──────┐                     │
                         │ Kitchen   │                     │
                         │ screen 🔔 │                     │
                         └─────┬─────┘                     │
............................. │ ..........................│............
TEAM                     ┌────▼──────┐   ┌──────────────┐  │
                         │ Cook makes│──▶│ Burger sent  │──┘
                         │ burger    │   │ to counter   │
                         └───────────┘   └──────────────┘
```
- Start at first contact and end when the user completes registration
- Every place you don't actually know what happens — mark with a **"?"** instead of guessing
Use **Miro**, **draw.io**, or any other tool you like for the drawing.
Bring the map (with the question marks) to the meeting.

**Guiding questions** *(answer before the meeting, in writing)*:
1. Choose one journey at HK: where does it truly begin for the user, and what is their end goal?
2. Which steps in that journey are visible to the user — and which happen back office (staff actions, systems, emails, spreadsheets)?
3. Where do users get stuck or drop off along the way? Do I *know* this, or am I assuming?
4. For each back-office step: who owns it, and what happens when they're unavailable?

---

# Unit 3 — Needs & Requirements

*[Content placeholder]*

**Pre-reading:** *[placeholder — curated articles]*

**Guiding questions:** *[placeholder]*

**Weekly Challenge:** *[placeholder]*

---

# Unit 4 — Specification

*[Content placeholder]*

**Pre-reading:** *[placeholder — curated articles]*

**Guiding questions:** *[placeholder]*

**Weekly Challenge:** *[placeholder]*

---

# Unit 5 — Project Management

*[Content placeholder]*

**Pre-reading:** *[placeholder — curated articles]*

**Guiding questions:** *[placeholder]*

**Weekly Challenge:** *[placeholder]*
