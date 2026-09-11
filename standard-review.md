# Test 2 - Standard Review

## Purpose

Validate that an AI-assisted process involving personal data and medium decision impact is routed to **STANDARD_REVIEW**.

## Test data

**Requester name:** Sujith Raaj  
**Team:** Customer Operations  
**Process name:** Customer support request classification  
**Current process:** Incoming customer support requests are manually reviewed, categorized by issue type and urgency, and assigned to the appropriate support queue. The requests can contain customer names, email addresses, and account information.  
**Frequency:** Multiple times per day  
**Minutes per run:** 8  
**Systems involved:** CRM, support inbox, ticketing system  
**Data sensitivity:** Personal data  
**Decision impact:** Medium  
**Will the automation use AI?:** Yes  
**Desired outcome:** Use AI to classify incoming requests, suggest the appropriate support queue, and reduce manual triage while allowing support staff to review the recommendation.

## Expected result

**Governance route:** `STANDARD_REVIEW`

## Why

The process uses AI, handles personal data, and influences operational routing. A human remains involved, so the workflow should require additional review without treating it as the highest-risk category.
