# Simulation Engine Architecture

## Purpose

The simulation engine is the practice layer of CareQuest.

Its job is to turn care training from passive content into realistic decision-making practice.

---

## Core Idea

Learners should not only learn what reinforcement, safety, observation, and communication mean.

They should repeatedly practice applying them in realistic behavioral situations.

---

## Simulation Flow

1. Learner selects a mission
2. System presents a behavioral scenario
3. Learner responds
4. Scenario can branch depending on response quality
5. AI supervisor evaluates response
6. Competency engine updates scores
7. Learning engine recommends next mission

---

## Scenario Inputs

Each simulation can include:

- learner role
- child profile
- environment
- behavioral trigger
- current behavior
- escalation risk
- available intervention options
- supervision goal

---

## Example Scenario Object

```json
{
  "scenario_id": "SC-001",
  "title": "Transition Refusal",
  "difficulty": "Beginner",
  "environment": "Classroom",
  "trigger": "Abrupt transition from play to structured work",
  "behavior": "Child cries and refuses to move",
  "competencies_tested": [
    "empathy",
    "safety",
    "observation",
    "communication",
    "reinforcement"
  ]
}
