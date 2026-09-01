<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0a192f,50:0d3b66,100:00b4d8&height=230&section=header&text=THEVOIDSYNTAX&fontSize=52&fontColor=ffffff&fontAlignY=38&desc=Mapping%20processes.%20Writing%20specs.%20Automating%20the%20rest.&descSize=15&descAlignY=58&v=4" width="100%" alt="Banner"/>

  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=17&duration=3500&pause=1200&color=00B4D8&center=true&vCenter=true&width=680&height=40&lines=Business+Analyst.+I+write+the+specs.;Mapping+what+users+actually+do%2C+not+what+the+SOP+says.;Automating+the+parts+nobody+wants+to+do+twice.;Learning+AI+workflows+and+defensive+security." alt="Typing SVG"/>
  </a>

  <p align="center">
    <a href="https://rio-wicaksono.com"><img src="https://img.shields.io/badge/Portfolio-rio--wicaksono.com-00b4d8?style=for-the-badge&logo=google-chrome&logoColor=black" alt="Portfolio"/></a>
    <a href="https://linkedin.com/in/riowicaksono"><img src="https://img.shields.io/badge/LinkedIn-Rio_Wicaksono-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
    <a href="mailto:riowicaksono.work@gmail.com"><img src="https://img.shields.io/badge/Email-riowicaksono.work@gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  </p>
</div>

---

Business Analyst. I write the documents that turn "we need a system for this" into something a developer can actually build.

Most of my work is unglamorous — sitting with users, mapping what they actually do versus what the SOP says they do, then writing it down properly. The gap between those two is where most project failures live.

Lately I've been learning AI workflows and defensive security. Not to switch careers. Because when a stakeholder asks "can AI do this?" or "is this data safe?", I'd rather answer than nod and take a note.

---

### Case: Approval Workflow

An internal approval process that took four days. Most of that was waiting, not working.

**Before**

```mermaid
flowchart LR
    A[Request via email] --> B[Manual check<br/>across 3 spreadsheets]
    B --> C[Print, sign, scan]
    C --> D[Re-key into system]
    D --> E[~4 days end to end]

    style E fill:#3b1f1f,stroke:#f87171,color:#fff
```

The re-keying step was the one everyone complained about. It was not the real problem. The real problem was that nobody could tell where a request was sitting, so people chased it by email and the queue never cleared.

**After**

```mermaid
flowchart LR
    A[Request via form] --> B[Auto-validation<br/>T-SQL rules]
    B --> C{Exception?}
    C -->|No| D[Auto-approve]
    C -->|Yes| E[Route to reviewer]
    D --> F[~2 hours end to end]
    E --> F

    style F fill:#1b3a2f,stroke:#4ade80,color:#fff
```

Roughly 70% of requests matched clean rules and no longer needed a human. The remaining 30% went to a reviewer with the validation results already attached. Names and figures are generalised.

---

### How I Decide What to Automate

```mermaid
flowchart LR
    A[Repetitive task] --> B{How often?}
    B -->|Rarely| C[Leave it alone]
    B -->|Weekly or more| D{Rules clear<br/>and stable?}

    D -->|Yes| E[Script it<br/>Python / T-SQL]
    D -->|No, needs judgment| F{Is the judgment<br/>language-based?}

    F -->|No| G[Keep it manual]
    F -->|Yes| H[Test an LLM<br/>with human review]

    style C fill:#3a3320,stroke:#facc15,color:#fff
    style G fill:#3a3320,stroke:#facc15,color:#fff
    style E fill:#0d3b66,stroke:#00b4d8,color:#fff
    style H fill:#0d3b66,stroke:#00b4d8,color:#fff
```

Two of the four outcomes are "don't automate." That ratio is roughly accurate in practice.

---

### Things I Learned the Hard Way

| What happened | What I do now |
|---|---|
| Wrote an FSD from the SOP without watching the actual process. Half the requirements were wrong by UAT. | I sit with users before writing anything. The SOP is a starting hypothesis, not a source. |
| Took UAT sign-off as proof the users understood the change. They signed to end the meeting. | Sign-off requires them to run their own scenario, not the one I prepared. |
| Automated a monthly report nobody was reading. Saved four hours a year. | I ask who reads the output before I touch the process that produces it. |

---

### Stack

| | |
|---|---|
| **Documentation** | BRD, FSD, use case specs, process maps |
| **Tools** | JIRA, Confluence, Visio, Excel |
| **Data** | T-SQL, SQL Server — reconciliation and integrity checks |
| **Testing** | SIT coordination, UAT facilitation, defect tracking |
| **Learning** | Python, LLM APIs, security fundamentals |

---

### Learning Log

Updated when something is actually finished.

| Topic | Where I'm at |
|---|---|
| LLM API integration | Built a few working scripts. See `llm-doc-drafter`. |
| Prompt design for business tasks | Understand what works. Still learning what breaks. |
| Agentic workflows | Reading. Nothing built yet. |
| Security fundamentals | Can follow a threat model conversation. Can't lead one. |
| Threat modeling | Early. Mostly reading case studies. |
| Python for data work | Pandas, file handling, API calls. No production code. |

---

Open to Business Analyst roles, process improvement projects, and requirements consulting. Based in Jakarta.

Fastest reply via [email](mailto:riowicaksono.work@gmail.com) or [LinkedIn](https://linkedin.com/in/riowicaksono).

<div align="center">
  <br/>
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0a192f,50:0d3b66,100:00b4d8&height=120&section=footer&v=4" width="100%" alt="Footer Banner"/>
</div>
