# Test 3 - Human Review

## Purpose

Validate that a process involving financial data and a high-impact decision is forced into the **HUMAN_REVIEW** governance path.

## Test data

**Requester name:** Sujith Raaj  
**Team:** Finance Operations  
**Process name:** Customer refund eligibility assessment  
**Current process:** Refund requests are reviewed against payment history, transaction value, account status, and refund policy. A team member determines whether the customer qualifies and whether money should be returned to the customer.  
**Frequency:** Daily  
**Minutes per run:** 15  
**Systems involved:** CRM, payment platform, transaction database, email  
**Data sensitivity:** Financial data  
**Decision impact:** High  
**Will the automation use AI?:** Yes  
**Desired outcome:** Use automation and AI to review refund requests, identify whether they appear to meet the policy criteria, and provide a recommendation to a finance specialist before any refund is approved.

## Expected result

**Governance route:** `HUMAN_REVIEW`

## Why

The workflow handles financial data and contributes to a high-impact decision. The deterministic governance layer should force human review regardless of whether the LLM considers the process suitable for automation.
