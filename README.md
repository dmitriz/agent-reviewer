# agent-reviewer

## Purpose

This agent performs post-execution analysis and system-level review  
to ensure expected outcomes, detect anomalies, and provide corrective signals  
within an automated investment system.

## Responsibilities

- Review trade execution results and flag discrepancies  
- Validate portfolio updates against expected states  
- Analyze trends, thresholds, or statistical deviations  
- Provide summaries or escalation alerts  
- Feed corrections or learning signals to planners or orchestrators

## Inputs

- Execution logs from agent-trade  
- Portfolio state snapshots from agent-portfolio  
- Event triggers from agent-orchestrator  
- External signals or anomaly events

## Outputs

- Anomaly reports or alerts  
- System health summaries  
- Corrective action suggestions or downgrade flags  
- Optional long-term review logs

## Update Triggers

- Post-execution events  
- Periodic scheduled reviews  
- Ad hoc validation requests

## Design Principles

- Passive validation only — does not initiate trades  
- Lightweight and interpretable metrics  
- Modular checks and filters per agent  
- Support both rule-based and statistical review models

## Integration

- Receives data from agent-trade, agent-portfolio, and agent-orchestrator  
- Sends feedback to planner agents or agent-orchestrator  
- Informs investor-index with review summaries or system health signals

## Status

This file defines the complete planning scope for `agent-reviewer`.  
No separate PRD is required.
