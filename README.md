# 📄 Cart Abandonment Reduction – Checkout Experience PRD

---

## 🏢 Context
- **Product:** E-commerce marketplace app  
- **Platform:** Mobile-first (Android/iOS)  
- **Geography:** India  
- **Users:**  Tier 1–3 shoppers with mixed payment preferences (UPI, Card, COD)    

---

## 🙋‍♀️ My Role

- Owned end-to-end PRD creation  
- Defined problem using funnel analysis  
- Synthesized competing hypotheses across teams  
- Proposed solutions across UX + engineering  
- Designed metrics, guardrails, and experiment strategy  

---

## 🔍 Problem

65% of users abandon their carts before purchasing, with a major drop-off at the **payment step**.

### Key Hypotheses
1. 💳 Unreliable payment flows (UPI/card failures)  
2. 💵 COD not visible early in checkout  
3. 💸 Hidden fees (shipping/taxes appear late)  
4. ⏱️ Slow payment page load  

👉 Result: Users feel **surprised, frustrated, and lose trust**, leading to lost GMV.

---

## ⚠️ Assumptions

- Majority abandonment is driven by **UX friction**, not pricing  
- COD demand is significantly higher in **Tier 2/3 cities**  
- Payment failures reduce **trust and repeat purchase intent**  
- Users value **predictability over discounts** in checkout  

---

## 🎯 Goals

- Abandonment: **65% → 50%**  
- Payment drop-off: **-30%**  
- Checkout completion: **+20%**

---

## 📊 North Star Metric
**Checkout Completion Rate (CCR)**  
- Current: 35% → Target: 50%

---

## 💰 Impact

- 10M monthly carts  
- 10% recovery → 650K orders  
- AOV ₹1,200  

👉 **₹78 Cr/month incremental GMV**

---

## 🧩 Solution Strategy

### Phase 1 (4 weeks)
- Funnel instrumentation  
- Fee transparency  
- COD visibility  
- Performance fixes  

### Phase 2
- Data-driven checkout redesign  

---

## 🔁 Key Solutions

### 1. Fee Transparency
- Show shipping + tax on PDP & cart  
- No surprises at payment  

### 2. COD Visibility
- Show COD availability on cart  
- Prioritize COD in payment  

### 3. Payment Recovery
- Detect failures instantly  
- Show retry + alternate methods + COD  

### 4. Performance
- Payment load time <2s  

---

## ⚙️ Core Rules

- Fees visible before checkout  
- COD checked at cart stage  
- Show alternatives after first failure  

---

## 🚫 Non-Goals

- No pricing/discount changes  
- No new payment methods  
- No discovery redesign  

---


## 👥 Dependencies

- Payments API (failure detection)  
- Logistics API (pincode + COD)  

---

## 🚀 Next Steps

- Segment COD vs prepaid users  
- Optimize for low-end devices  
- Analyze payment failure logs  

---

## ⭐ Why This PRD

- Clear problem → solution mapping  
- Metrics-driven approach  
- Real-world constraints considered  