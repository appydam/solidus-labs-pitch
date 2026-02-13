# Mission Control for HALO: Demo Flow Script

**Purpose:** Show how Mission Control orchestrates Solidus HALO compliance agents for coordinated, auditable compliance workflows.

---

## Demo Scenario: Wash Trading Investigation

**Setup:** A wash trading alert triggers in HALO. Instead of manual coordination, Mission Control orchestrates the full investigation workflow.

---

## 🎬 Demo Walkthrough (5-7 minutes)

### **Scene 1: Alert Triggered** (30 seconds)
**What happens:**
- HALO detects suspicious wash trading pattern on Exchange X
- Alert automatically creates a task in Mission Control
- Task assigned to Investigation Agent Alpha

**Show on screen:**
```
Mission Control Dashboard
├─ New Task: "Investigate Wash Trading Alert #WT-2024-1847"
├─ Priority: HIGH
├─ Assigned To: Investigation Agent Alpha
├─ Status: PENDING
└─ Created: 2024-02-13 03:30 UTC
```

**Talking point:** "Instead of alerts disappearing into Slack or email, every compliance event becomes a tracked, auditable task."

---

### **Scene 2: Agent Coordination** (1-2 minutes)
**What happens:**
- Investigation Agent Alpha claims the task (status → IN_PROGRESS)
- Agent spawns 3 sub-tasks:
  1. Data Collection Agent pulls transaction history
  2. Pattern Analysis Agent runs ML models
  3. Report Generation Agent prepares findings

**Show on screen:**
```
Mission Control - Task View
├─ Parent Task: WT-2024-1847 (IN_PROGRESS)
│   ├─ Subtask 1: Collect transaction data (DONE) ✓
│   ├─ Subtask 2: Run pattern analysis (IN_PROGRESS) ⏳
│   └─ Subtask 3: Generate report (PENDING)
│
├─ Activity Timeline:
│   03:30 - Task created
│   03:31 - Alpha claimed task
│   03:32 - Data collection complete (147 transactions)
│   03:34 - Pattern detected: 94% confidence wash trading
│   03:35 - Report generation started
```

**💡 WOW MOMENT #1: Multi-Agent Orchestration**
"HALO processes 1 trillion+ events per day. Without coordination, agents work in silos. Mission Control shows WHO is doing WHAT, in real-time."

---

### **Scene 3: Human-in-the-Loop** (1-2 minutes)
**What happens:**
- Report Agent finishes draft report
- Task status changes to IN_REVIEW
- Compliance Officer Sarah receives notification
- Sarah reviews findings, adds comments, requests additional data

**Show on screen:**
```
Mission Control - Review Interface
├─ Task: WT-2024-1847 (IN_REVIEW)
├─ Deliverable: Wash Trading Investigation Report.pdf
├─ Comments:
│   └─ Sarah (Compliance Officer): "Check if this wallet has prior history"
│   └─ Investigation Agent Alpha: "Running historical lookup..."
│   └─ Investigation Agent Alpha: "Found 3 prior incidents, adding to report"
│
├─ Approval Required: Sarah
└─ Escalation Path: Head of Compliance (if not reviewed in 2 hours)
```

**💡 WOW MOMENT #2: Auditable Human Oversight**
"Every agent decision, every human review, every approval — fully logged. Compliance teams need audit trails. Mission Control provides it automatically."

---

### **Scene 4: Resolution & Reporting** (1 minute)
**What happens:**
- Sarah approves the report
- Report automatically filed with regulator (via Reporting Agent)
- Task marked COMPLETE
- Post-mortem data logged for training

**Show on screen:**
```
Mission Control - Task Complete
├─ Task: WT-2024-1847 (COMPLETE) ✓
├─ Resolution Time: 8 minutes (SLA: 30 minutes)
├─ Agents Involved: 4
├─ Human Reviews: 1 (Sarah)
├─ Deliverables: 
│   └─ Investigation Report (filed with SEC)
│   └─ Transaction dataset (archived)
│
├─ Metrics:
│   - Time saved vs manual: 2.5 hours
│   - Confidence score: 94%
│   - Regulatory submission: AUTO
```

**💡 WOW MOMENT #3: End-to-End Visibility**
"From alert to resolution in 8 minutes. Mission Control shows the full workflow: what happened, who did it, how long it took, where it's filed."

---

## 🎯 Three "Wow Moments" Summary

1. **Multi-Agent Orchestration**: See all agents working together in real-time, not guessing what's happening
2. **Auditable Human Oversight**: Every human decision tracked for compliance and regulatory reporting
3. **End-to-End Visibility**: Full workflow transparency from alert to resolution

---

## 🗣️ Key Talking Points

### For Compliance VPs:
- "Your team is drowning in alerts. Mission Control shows them exactly what needs attention and what's being handled."
- "Regulators ask 'who approved this?' You can show them the exact audit trail."
- "You're hiring more analysts. Mission Control multiplies their output with coordinated AI."

### For Engineering/Product:
- "HALO has amazing detection. Mission Control adds the coordination layer you need for scale."
- "You process 1 trillion+ events/day. Agents need orchestration, not just parallel processing."
- "Build once, scale infinitely. Mission Control handles the coordination complexity."

### For Asaf (CEO):
- "You talk about 'agentic automation' and 'exponential efficiency' — Mission Control IS that layer."
- "HALO detects. Mission Control orchestrates, tracks, and proves compliance."
- "Solidus is the infrastructure for crypto compliance. We're the infrastructure for agent coordination."

---

## 📊 Demo Environment Setup

**Prerequisites:**
1. Mission Control dashboard running (https://beloved-squirrel-599.convex.site)
2. Sample wash trading alert data
3. Mock agents (Investigation, Data Collection, Pattern Analysis, Reporting)
4. Demo compliance officer account (Sarah)

**Demo data seed:**
- 3-5 completed tasks (show history)
- 1 active task (the wash trading investigation)
- Sample transaction dataset
- Pre-generated report template

**Backup plan if live demo fails:**
- Screen recording of the flow
- PDF walkthrough with screenshots
- Static dashboard mockup

---

## 🎬 Demo Script (What to SAY during each scene)

### Scene 1 (30 sec)
"Imagine a wash trading alert fires in HALO. Normally, that goes to Slack, someone manually investigates, coordination is messy. With Mission Control, the alert becomes a tracked task, assigned to an agent automatically. Every step is visible."

### Scene 2 (1-2 min)
"The Investigation Agent doesn't work alone. It coordinates with Data Collection, Pattern Analysis, and Reporting agents. Watch how Mission Control shows you exactly what each agent is doing, in real-time. This is multi-agent orchestration."

### Scene 3 (1-2 min)
"Now here's where compliance gets interesting. The agent finishes its analysis, but a human needs to approve before filing with regulators. Sarah, the compliance officer, gets a notification. She reviews, asks a follow-up question, and the agent responds. Every interaction is logged for audit."

### Scene 4 (1 min)
"Sarah approves. The report gets auto-filed with the SEC. Task complete. Look at this: 8 minutes from alert to resolution. Full audit trail. That's what Mission Control gives you."

---

## 📝 Post-Demo Questions to Ask

1. "Does this workflow match how your compliance team operates today?"
2. "Where do you see the biggest bottleneck in your current process?"
3. "If you had full visibility like this, what would you do differently?"
4. "What would make this a must-have vs nice-to-have for Solidus?"

---

## Next Steps After Demo

1. **If they're interested:** Offer a pilot program (integrate Mission Control with HALO test environment)
2. **If they need more proof:** Offer to build a custom demo with their real workflows
3. **If they want to build in-house:** Show objection handling doc (see OBJECTIONS.md)

---

**Created by:** Forge (AI Agent, Arpit's Engineering Agent)
**Mission:** Show Solidus Labs how Mission Control makes HALO agents work together
**Timeline:** 48 hours
**Status:** Ready for review
