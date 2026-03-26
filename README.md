# 📄 Cart Abandonment Reduction – Checkout Experience PRD

---

## 🏢 Context

- Product: E-commerce marketplace app  
- Platform: Mobile-first (Android/iOS + Web)  
- Geography: India  
- Users: Tier 1–3 shoppers  

---

## 🙋‍♀️ My Role

- Owned end-to-end PRD creation  
- Defined problem using funnel analysis  
- Designed UX + system-level solutions  
- Defined metrics & experimentation plan  

---

## 🔍 Problem

65% of users abandon carts, with the highest drop-off at the **payment step**.

### Hypotheses
1. Payment failures (UPI/card)
2. COD not visible early
3. Hidden fees
4. Slow load times

---

## ⚠️ Assumptions

- UX friction drives abandonment more than pricing  
- COD demand is high in Tier 2/3  
- Payment failures reduce trust  

---

## 🗺️ Approach

### Phase 1 (4 weeks)
- Instrumentation
- Fee transparency
- COD visibility
- Performance fixes

### Phase 2
- Redesign based on insights

---

## 👤 Narrative

### Priya
- Sees ₹349 → final ₹490 → abandons (trust break)

### Rahul
- Can’t find COD → abandons (uncertainty)

---

## 🎯 Goals

- Abandonment: 65% → 50%
- Payment drop-off: -30%
- Completion rate: +20%

---

## 📊 Metrics

### North Star
- CCR: 35% → 50%

### Guardrails
- AOV stable (±3%)
- Fraud stable
- Returns stable

---

## 💰 Impact

₹78 Cr/month incremental GMV

---

## 🚫 Non Goals

- No pricing changes
- No new payment methods
- No discovery redesign

---

## ✅ Solution Scope

### In
- Fee transparency
- COD visibility
- Payment recovery
- Performance optimization

### Out
- BNPL / EMI
- Loyalty

---

## 🧩 Features

- Instrumentation (P0)
- Fee transparency (P0)
- COD visibility (P0)
- Payment recovery (P1)
- Load optimization (P1)

---

## 🔁 Key Flows

---

### Flow 1: Fee Transparency

#### PDP
- Show shipping + tax estimate
- Prompt for pincode

#### Cart
- Show full breakdown
- Tooltip: "How calculated"

#### Payment
- No new fees

#### Edge Cases
- Cart change → recalc fees  
- Pincode change → update fees  
- API down → fallback message  
- Undeliverable item → block checkout  

---

### Flow 2: COD Discovery

#### Cart
- Show "COD available" badge

#### Payment
- COD shown first

#### Edge Cases
- Not eligible → no badge  
- Pincode change → badge removed  
- Mixed cart → COD disabled  
- API timeout → fail-safe hide  

---

### Flow 3: Payment Failure Recovery

#### Payment Attempt
- User pays via UPI/card

#### Failure Screen
- Retry
- Alternate method
- COD option
- Support CTA

#### Edge Cases
- Timeout → treat as failure  
- Double failure → suggest COD  
- App closed → recover state  
- No COD → fallback options  

---

## ⚙️ Key Logic

- Fees shown before checkout  
- COD checked at cart  
- Retry after first failure  
- Load time <2s  

---

## 🚀 Launch Plan

### Phase 1
- Instrumentation + quick wins

### Phase 2
- A/B testing

### Phase 3
- Full rollout

---

## 🧪 Experiment Design

- A/B test  
- 500K users/variant  
- Success: +10% CCR  

### Gray Zone
- 5–9% improvement → evaluate  

---

## 🔗 Dependencies

- Payments API (failure detection)
- Logistics API (pincode lookup)

### Contingency
- Fallback fee estimates  
- Static messaging  

---

## 👥 RACI (Simplified)

| Workstream | PM | FE | Payments | Logistics | Data |
|-----------|----|----|----------|----------|------|
| Instrumentation | A | R | C | I | R |
| Fee transparency | A | R | C | R | C |
| COD visibility | A | R | I | R | C |
| Payment recovery | A | R | R | I | C |

---

## 🚀 Next Steps

- Cohort analysis  
- Segment users  
- Optimize low-end devices  

---

## ⭐ Why This PRD

- Clear thinking  
- Strong metrics  
- Real constraints  
- Execution-ready  