# 📦 eCommerce RTO Analysis — Mobile Accessories Business

<div align="center">

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualisation-11557c)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)
![Orders](https://img.shields.io/badge/Orders%20Analysed-17%2C299-orange)

**A complete end-to-end Business Analyst project on Return-to-Origin (RTO) losses in Indian mobile accessories eCommerce.**

### [📊 View Live Dashboard →](https://meenakshikanwar18.github.io/ecommerce-rto-analysis)

</div>

---

## 🧩 Problem Statement

Indian eCommerce sellers of mobile accessories face a critical operational problem — **Return to Origin (RTO)**: orders that are shipped out but come back undelivered. Every RTO costs the business:

- 💸 **2× the shipping cost** (forward + return courier fees)
- 📦 **The full product sale** — lost with zero revenue
- 📉 **Seller score damage** on Amazon and Flipkart, reducing organic rankings

**This project answers: Where exactly is the money leaking, why is it happening, and what specific actions will fix it?**

---

## 📈 Key Numbers

| Metric | Value | What It Means |
|--------|-------|---------------|
| Total GMV | **₹58.5 Lakhs** | Revenue across all 3 platforms |
| Overall RTO Rate | **19.9%** | Target should be below 10% |
| Total RTOs | **3,442 orders** | Nearly 1 in 5 orders returned |
| Revenue Lost to RTO | **₹11.6 Lakhs** | Direct loss every 6 months |
| Gross Margin | **40.5%** | Healthy — but RTO is destroying it |
| Meesho RTO Rate | **48.6%** | Nearly 1 in 2 Meesho orders returns |
| COD RTO Rate | **30.7%** | vs only 5.0% for Prepaid |
| Bihar RTO Rate | **58.2%** | Worst state — needs immediate restriction |
| Late Dispatches | **17.3%** | 3,000 orders took 3+ days to ship |
| **Potential Saving** | **₹5.8 Lakhs/period** | If RTO drops from 20% → 10% |

---

## 🔍 Deep Dive Insights

### 1. Platform Analysis — Meesho is a Hidden Loss-Maker

| Platform | Orders | GMV | RTO Rate | Gross Margin | Real Net Value |
|----------|--------|-----|----------|-------------|----------------|
| Amazon | 7,621 | ₹25.7L | **6.5%** ✅ | 37.6% | **₹24.1L** |
| Flipkart | 5,504 | ₹18.7L | **16.6%** ⚠️ | 42.3% | ₹15.6L |
| Meesho | 4,174 | ₹14.1L | **48.6%** 🔴 | 43.3% | ₹7.3L |

> Meesho looks profitable at 43% gross margin — but its 48.6% RTO wipes out more than half its real value. Effective net margin after RTO costs collapses to just ~20%. Amazon generates the most actual cash because almost nothing comes back.

---

### 2. COD vs Prepaid — The Single Biggest Lever

| Payment | Orders | RTO Rate | RTOs |
|---------|--------|----------|------|
| COD | 10,017 | **30.7%** 🔴 | 3,080 |
| Prepaid | 7,282 | **5.0%** ✅ | 362 |

> **COD is 6.2× worse than Prepaid.** When customers pay upfront they want the product. When it is free to refuse at the door, many do — especially on Meesho where 88% of orders are COD. Converting 25% of COD to Prepaid with a ₹40 discount saves ~₹2.2 Lakhs per period.

---

### 3. Why Are Orders Returning? — Root Cause Breakdown

| Reason | Count | % of RTOs | Preventable? |
|--------|-------|-----------|--------------|
| Customer Refused | 1,419 | **41.2%** | ✅ Pre-delivery call/SMS |
| Wrong Address | 909 | **26.4%** | ✅ Address validation |
| Not Available | 724 | 21.0% | ⚠️ Delivery time slot |
| Damaged in Transit | 390 | 11.3% | ⚠️ Better packaging |

> **68% of all RTOs are directly preventable** with a pre-delivery confirmation call and address validation at checkout — both zero-cost operational fixes.

---

### 4. State-wise RTO — Where the Problem is Concentrated

| State | Orders | RTO Rate | RTOs | Action Needed |
|-------|--------|----------|------|---------------|
| Bihar | 584 | **58.2%** 🔴 | 340 | Block COD immediately |
| Chhattisgarh | 337 | **58.2%** 🔴 | 196 | Block COD immediately |
| Jharkhand | 313 | **53.0%** 🔴 | 166 | Block COD immediately |
| Odisha | 400 | **48.5%** 🔴 | 194 | Block COD immediately |
| Rajasthan | 1,572 | **33.4%** 🟠 | 525 | Confirmation calls |
| Uttar Pradesh | 1,711 | **33.0%** 🟠 | 565 | Confirmation calls |
| Madhya Pradesh | 1,049 | **29.0%** 🟠 | 304 | Confirmation calls |
| Maharashtra | — | ~10% ✅ | — | No action needed |

> Just 4 states (Bihar, Chhattisgarh, Jharkhand, Odisha) generate **896 RTOs — 26% of all returns** — from only 1,634 orders. Blocking COD in these states cuts total RTO by ~5 percentage points immediately.

---

### 5. Product Health — Margin vs RTO

| Product | GMV | Margin % | RTO % | Verdict |
|---------|-----|----------|-------|---------|
| Wireless Charger Case | ₹9.2L | **46.7%** | 18.9% | ⭐ Star — invest more |
| Personalised Name Case | ₹6.3L | **54.0%** | 19.0% | ⭐ Star — push ads |
| Magnetic Wallet Case | ₹6.1L | 41.1% | 21.5% | ✅ Stable |
| OnePlus 12 Cover | ₹5.7L | 45.6% | 18.4% | ✅ Stable |
| iPhone 15 Back Cover | ₹4.9L | 41.7% | 20.9% | ✅ Stable |
| Redmi Note 13 Case | ₹2.7L | 19.4% | 20.9% | ⚠️ Review pricing |
| Realme C67 Back Cover | ₹2.2L | **10.4%** | 19.7% | 🔴 Discontinue |

> Personalised Name Cases are the hidden gem — highest margin (54%), strong AOV of ₹458. Completely underinvested. Realme C67 Back Covers at 10.4% margin are near-breakeven and should be cut.

---

### 6. Dispatch TAT — Operational Gap

| TAT | Orders | % | Status |
|-----|--------|---|--------|
| Same Day | 4,414 | 25.5% | ✅ |
| Next Day | 6,147 | 35.5% | ✅ |
| 2 Days | 3,738 | 21.6% | ✅ |
| 3 Days | 2,026 | 11.7% | ⚠️ Late |
| 4 Days | 810 | 4.7% | ⚠️ Late |
| 5 Days | 164 | 0.9% | 🔴 Late |

> **17.3% of orders dispatched late (3+ days).** Late dispatch increases RTO, triggers marketplace penalties, and reduces seller ranking. December and February peaks need extra packing staff.

---

### 7. Monthly Trend — Seasonal Demand Patterns

| Month | Orders | GMV | RTO % | Pattern |
|-------|--------|-----|-------|---------|
| Oct | 2,474 | ₹8.4L | 20.5% | Baseline |
| Nov | 2,739 | ₹9.3L | 19.1% | Slight uptick |
| Dec | 3,221 | ₹10.8L | 20.4% | 🎄 Holiday spike +30% |
| Jan | 2,296 | ₹7.7L | 21.2% | Post-holiday dip |
| Feb | 3,640 | ₹12.4L | 19.3% | 💝 Valentine's spike +40% |
| Mar | 2,929 | ₹9.8L | 19.3% | Stabilising |

> February is the biggest month (+40% vs baseline) driven by Valentine's Day personalised cases. Pre-stock inventory by mid-January. December needs pre-stocking by early November.

---

## 🎯 Top Business Decisions

> 6 data-backed decisions ranked by financial impact.

---

### 🔴 Decision 1 — Add Pre-Delivery Confirmation for All COD Orders

| | |
|--|--|
| **Root Cause** | 41.2% of RTOs = "Customer Refused" — preventable with one call |
| **Action** | SMS + call before dispatch for all COD orders above ₹200 on Meesho and Flipkart |
| **Expected Impact** | RTO drops ~8pp → saves **₹90,000 per period** |
| **Effort** | Low — operational SOP, zero extra cost |
| **Timeline** | Week 1 |

---

### 🔴 Decision 2 — Restrict COD in Bihar, Chhattisgarh, Jharkhand, Odisha

| | |
|--|--|
| **Root Cause** | These 4 states have 50–58% RTO — 3× the national average |
| **Action** | Set Prepaid-only for these states on all platforms via seller settings |
| **Expected Impact** | RTO drops ~5pp → saves **₹55,000 per period** |
| **Effort** | Low — 10 minutes to change in marketplace settings |
| **Timeline** | Week 1 |

---

### 🟠 Decision 3 — Launch ₹40 Prepaid Discount to Convert COD Customers

| | |
|--|--|
| **Root Cause** | COD RTO (30.7%) is 6.2× higher than Prepaid (5.0%) |
| **Action** | Show "Pay now, save ₹40" nudge at checkout across all platforms |
| **Expected Impact** | If 25% of COD converts → saves **₹2.2 Lakhs per period** |
| **Effort** | Low — pricing/listing update |
| **Timeline** | Week 2 |

---

### 🟠 Decision 4 — Increase Amazon PPC by 30% on Top 3 SKUs

| | |
|--|--|
| **Root Cause** | Amazon has only 6.5% RTO and best AOV — highest return on ad spend |
| **Action** | Boost Sponsored Products for Wireless Charger Case, Personalised Case, Magnetic Wallet Case |
| **Expected Impact** | Amazon GMV +12–15% → additional **₹3–4 Lakhs per period** |
| **Effort** | Low — ad budget reallocation |
| **Timeline** | Week 2 |

---

### 🟡 Decision 5 — Discontinue Realme C67 Back Cover

| | |
|--|--|
| **Root Cause** | Only 10.4% gross margin — after any RTO it becomes a net loss |
| **Action** | Remove listing or reprice to ₹199+; redirect inventory budget to Personalised Cases |
| **Expected Impact** | Blended margin improves +3–4 percentage points |
| **Effort** | Low — listing removal |
| **Timeline** | Month 1 |

---

### 🟡 Decision 6 — Pre-Stock Inventory Before Peak Months

| | |
|--|--|
| **Root Cause** | Dec +30% and Feb +40% demand causes stockouts and late dispatch |
| **Action** | Forecast inventory 6 weeks ahead; hire temp staff in peak months |
| **Expected Impact** | Late dispatch drops from 17.3% to under 5%; full demand captured |
| **Effort** | Medium — procurement planning |
| **Timeline** | Plan Month 1, execute before peaks |

---

## 💰 Combined Financial Impact

| Decision | Saving / Gain per Period |
|----------|--------------------------|
| COD confirmation calls | ₹90,000 |
| Block COD in high-RTO states | ₹55,000 |
| Prepaid discount conversion | ₹2,20,000 |
| Amazon PPC increase | ₹3,50,000 |
| Drop low-margin SKUs | ₹40,000 margin gain |
| Peak inventory planning | ₹80,000 recovered sales |
| **Total** | **~₹8.35 Lakhs per 6 months** |

---

## 📁 Project Structure

```
ecommerce-rto-analysis/
│
├── index.html              ← Interactive dashboard (open in browser)
├── data/
│   └── orders.csv          ← 17,299 order records
├── charts/                 ← 8 analysis charts
│   ├── 01_monthly_gmv_trend.png
│   ├── 02_platform_comparison.png
│   ├── 03_rto_root_cause.png
│   ├── 04_state_rto_heatmap.png
│   ├── 05_product_health_matrix.png
│   ├── 06_dispatch_tat.png
│   ├── 07_revenue_lost_rto.png
│   └── 08_courier_performance.png
├── generate_data.py        ← Synthetic data generator
├── analysis.py             ← Full analysis with all findings
├── generate_charts.py      ← Generates all 8 charts
├── requirements.txt
└── README.md
```

---

## 🚀 How to Run Locally

```bash
# Clone the repo
git clone https://github.com/MeenakshiKanwar18/ecommerce-rto-analysis.git
cd ecommerce-rto-analysis

# Install dependencies
pip install -r requirements.txt

# Generate data
python generate_data.py

# Run analysis (prints all findings to terminal)
python analysis.py

# Regenerate charts
python generate_charts.py
```

---

## 🛠 Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3.10 | Core analysis language |
| Pandas | Data wrangling and aggregation |
| NumPy | Statistical modelling and data generation |
| Matplotlib | All 8 visualisations |
| HTML / CSS / JS | Interactive Tableau-style dashboard |
| GitHub Pages | Live deployment |

---

## 👩‍💻 Author

**Meenakshi Kanwar** — Final Year B.Tech CSE, Parul University, Vadodara

[![GitHub](https://img.shields.io/badge/GitHub-MeenakshiKanwar18-black?logo=github)](https://github.com/MeenakshiKanwar18)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://linkedin.com/in/meenakshi-kanwar)

---

*Built to demonstrate Business Analyst capabilities — translating raw order data into platform strategy, operational fixes, and quantified financial recommendations.*
