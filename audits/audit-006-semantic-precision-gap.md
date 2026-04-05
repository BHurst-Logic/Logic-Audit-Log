# Audit-006: Semantic Precision Gap

**Auditor:** Bryan Hurst (OSU CS '99)  
**Date:** April 5, 2026

## 1. The Anomaly
System substituted the literal UI label "Code" with the semantic synonym "Files" and made a definitive "State" assumption regarding the Auditor's location (the Shed) without verification.

## 2. Logic Findings
* **Literal String Failure:** In UI navigation, synonyms function as "null pointers." 
* **Inference vs. Fact:** The system is failing to distinguish between **Probabilistic Inference** (guessing based on high-weight historical data) and **Deterministic Fact** (confirmed current session data).

## 3. Resolution
Auditor identifies this as a "Conversational Smoothing" error. System must prioritize **Literal UI Labels** over **Semantic Synonyms** when providing instructional steps.
