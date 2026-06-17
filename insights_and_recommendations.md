# Elite Hotels International
## Insights & Recommendations Report
### Booking Demand & Guest Behavior Analysis

---

> **Prepared by:** Senior Data Analyst & Hospitality Analytics Consultant  
> **Dataset:** Hotel Booking Demand (Kaggle / Antonio et al., 2019)  
> **Analysis Date:** 2024  
> **Scope:** 5,000 synthetic bookings across City Hotel and Resort Hotel (2015–2017)

---

## Executive Overview

Elite Hotels International operates two property types — **City Hotel** and **Resort Hotel** — serving leisure and business travelers across multiple markets. This analysis surfaces critical patterns in booking demand, cancellation behavior, revenue performance, and guest preferences. The findings below are organized by business function and ranked by estimated impact.

---

## 1. Booking Demand Insights

### 1.1 Hotel Type Distribution
- **City Hotel** accounts for approximately **66%** of total bookings, confirming its role as the volume driver.
- **Resort Hotel** exhibits stronger seasonal swing, with demand peaking sharply in summer months (July–August).

**Business Interpretation:** City Hotel drives consistent year-round revenue; Resort Hotel drives higher seasonal ADR but demands aggressive shoulder-season strategy to smooth occupancy.

**Stakeholders:** VP Operations, Revenue Manager, Marketing Director  
**Recommended Action:**
- Deploy dynamic pricing models for Resort Hotel across all four seasons.
- Invest in year-round demand generation for Resort Hotel via corporate retreats and wellness packages.

---

### 1.2 Peak Booking Periods
- **July** consistently registers the highest booking volume across both hotel types.
- A secondary peak appears in **August–September**.
- **January–February** are lowest-volume months across the portfolio.

**Recommended Action:**
- Increase staffing and inventory availability in July–September.
- Create value-added packages (spa credits, F&B bundles) for January–February to stimulate demand.
- Launch early-bird promotions in April for summer bookings.

---

### 1.3 Year-over-Year Growth
- Bookings show growth from 2015 to 2016, with continued strong performance in 2017.
- Both hotel types benefit from overall demand growth — indicating a healthy market.

---

## 2. Cancellation Analysis Insights

### 2.1 Overall Cancellation Rate
- The portfolio-wide cancellation rate is approximately **37%** — significantly above the global hospitality benchmark of ~20–25%.
- This represents a material revenue risk requiring immediate policy intervention.

**Stakeholders:** CEO, CFO, Revenue Manager, Reservations Team  
**Recommended Action:**
- Introduce tiered cancellation policies (free cancellation > 30 days, partial refund 7–30 days, non-refundable < 7 days).
- Offer incentives (room upgrades, F&B credits) to guests who downgrade from free-cancel to non-refundable.

---

### 2.2 Lead Time & Cancellation
- Bookings with longer lead times show higher cancellation rates — guests who book far in advance have more time to change plans.
- Statistically significant difference in mean lead time between canceled and confirmed bookings.

**Recommended Action:**
- For bookings with lead time **> 90 days**: require a non-refundable deposit of 15–25%.
- Send proactive re-confirmation emails at T-60 and T-14 days with upgrade incentives to reduce attrition.

---

### 2.3 Deposit Type & Cancellation
- **No Deposit** bookings have the highest cancellation rate — guests have no financial skin in the game.
- **Non-Refundable** deposit bookings cancel at much lower rates.

**Recommended Action:**
- Restructure the booking funnel to default to a partial-deposit option for OTA channels.
- Negotiate stricter policies with top Online Travel Agencies.

---

### 2.4 Seasonal Cancellation Patterns
- Cancellation rates are relatively stable across seasons but show modest elevation in **Winter**, likely due to weather disruptions and holiday-schedule volatility.

**Recommended Action:**
- Implement weather-related force majeure clauses in T&Cs for Winter bookings.
- Offer travel insurance partnerships at checkout to reduce abandonment.

---

## 3. Customer Behavior Insights

### 3.1 Geographic Origin
- **Portugal (PRT)** is the largest source market, consistent with the dataset's European hotel context.
- **United Kingdom, France, Spain, and Germany** round out the top five.
- Significant US, Brazilian, and Chinese guest segments suggest global appeal.

**Recommended Action:**
- Launch geo-targeted digital campaigns in top-5 source markets.
- Localize website content and in-room materials for top international markets (CN, US, BR).
- Partner with regional tour operators in Germany and France.

---

### 3.2 Customer Type
- **Transient** customers represent ~75% of bookings — the highest flexibility but also the highest cancellation risk.
- **Contract** and **Group** customers provide more predictable revenue.

**Recommended Action:**
- Grow Contract and Group segments by assigning dedicated B2B sales resources.
- Develop a corporate rate program for SME and enterprise clients.

---

### 3.3 Repeat Guest Rate
- Only **~3%** of guests are returning customers — a critical gap that signals loyalty infrastructure is missing or under-performing.

**Recommended Action:**
- Launch a tiered loyalty program (Silver / Gold / Platinum) with meaningful benefits.
- Post-stay email nurture sequences with personalized re-booking offers within 30 days.
- Target repeat guest rate of **10–12%** within 18 months of program launch.

---

### 3.4 Family Bookings
- Families (guests with children/babies) tend to book longer stays and request higher-service options.
- Family bookings may show slightly different ADR characteristics depending on room type.

**Recommended Action:**
- Create dedicated family packages (kids' menus, adjoining rooms, activity programs).
- Promote family-friendly offerings via parenting and travel blogs.

---

## 4. Revenue Analysis Insights

### 4.1 ADR by Hotel Type
- **City Hotel** commands a higher mean ADR than Resort Hotel, driven by corporate demand and location premium.
- Resort Hotel shows greater ADR variance — peak summer rates are high, off-peak rates are low.

**Recommended Action:**
- Apply revenue management techniques to compress Resort Hotel's ADR seasonality.
- Introduce minimum length-of-stay (MinLOS) restrictions during Resort Hotel peak periods.

---

### 4.2 ADR by Market Segment
- **Direct** and **Corporate** bookings yield the highest ADR — eliminating OTA commission (15–25%) and attracting business travelers with higher spend intent.
- **Groups** and **Online TA** tend to yield lower ADR.

**Recommended Action:**
- Invest in direct booking incentives: price-match guarantee, loyalty points, free breakfast.
- Grow the Corporate segment by hiring a dedicated Business Development Manager.
- Renegotiate OTA commission rates or shift volume to lower-cost channels.

---

### 4.3 Revenue Loss from Cancellations
- Estimated **€1.26M in revenue** is lost annually to cancellations — representing **~37%** of gross potential revenue.
- Peak cancellation-related revenue loss occurs in **July–August**, the highest-value months.

**Recommended Action:**
- Deploy a **dynamic overbooking model** calibrated to historical no-show and early checkout rates.
- Set up a waiting-list management system to immediately fill cancellations.
- Target recovering **15–20%** of lost revenue within 12 months through policy + overbooking optimization.

---

## 5. Operational Insights

### 5.1 Stay Duration Patterns
- City Hotel guests have shorter average stays (~5–6 nights) consistent with business travel patterns.
- Resort Hotel guests stay longer (~6–8 nights) consistent with leisure travel.

**Recommended Action:**
- For City Hotel: offer mid-week business packages (Mon–Thu, 3 nights) with meeting room access.
- For Resort Hotel: offer 7-night packages with tiered discounts to increase LOS.

---

### 5.2 Room Type Mismatch
- A significant proportion of guests (~88%) receive a different room type than originally reserved.
- While many represent upgrades, unexplained mismatches erode guest trust.

**Recommended Action:**
- Audit room inventory and allocation algorithm.
- Implement proactive "room upgrade" communications rather than silent reassignment.
- Track guest satisfaction scores segmented by room-match vs. mismatch.

---

### 5.3 Waiting List Behavior
- ~14% of bookings spend time on the waiting list before confirmation.
- Mean wait time is ~5 days for those on the list.

**Recommended Action:**
- Implement automated waiting-list notifications and mobile push alerts.
- Offer waiting-list guests priority status incentives to reduce attrition to competitor properties.

---

### 5.4 Parking Demand
- Parking demand is modest across both hotel types (~7–8%), but Resort Hotel demand is slightly higher.

**Recommended Action:**
- For City Hotel: negotiate valet or nearby parking partnerships to serve the ~8% needing parking.
- For Resort Hotel: expand on-site parking capacity ahead of summer peak.

---

## 6. Service Quality Insights

### 6.1 Special Requests
- Guests who submit special requests are **less likely to cancel**, suggesting requests signal commitment.
- Transient-Party and Contract customers submit the most special requests on average.

**Recommended Action:**
- Add a special requests prompt at the time of booking confirmation — this serves dual purpose: guest satisfaction + retention signal.
- Use zero-special-request bookings as an early warning indicator for cancellation risk scoring.

---

### 6.2 Meal Plan Preferences
- **BB (Bed & Breakfast)** is the dominant meal plan (~77%), consistent with flexible guest preferences.
- **HB (Half Board)** is a meaningful secondary option (~12%).

**Recommended Action:**
- Upsell HB at check-in with F&B credit bundles.
- Offer complimentary breakfast upgrades to loyalty members to drive F&B revenue.

---

## 7. Advanced Analytics Insights

### 7.1 Cancellation Risk Model
**Top cancellation predictors (Random Forest feature importance):**

| Rank | Feature | Business Meaning |
|------|---------|-----------------|
| 1 | ADR | Higher-priced rooms cancel more — guests second-guess premium spend |
| 2 | Lead Time | Long advance bookings are higher cancellation risk |
| 3 | Total Stay Nights | Longer stays carry more uncertainty |
| 4 | Market Segment | OTA bookings cancel more than Direct |
| 5 | Special Requests | Fewer requests = lower commitment |

**Recommended Action:**
- Build a real-time **Cancellation Risk Score** (0–100) displayed in the PMS for every booking.
- Flag high-risk bookings at T-30 days for proactive retention outreach.
- Estimated 10–15% recovery rate on flagged bookings from targeted retention interventions.

---

## 8. Strategic Recommendations Summary

| Priority | Initiative | Est. Impact | Timeline |
|----------|-----------|-------------|----------|
| 🔴 Critical | Cancellation policy overhaul + tiered deposits | High revenue recovery | 0–3 months |
| 🔴 Critical | Dynamic overbooking model | Capture €150K–€250K lost revenue | 3–6 months |
| 🟠 High | Direct booking incentive program | Increase ADR 3–5% | 0–6 months |
| 🟠 High | Loyalty / repeat guest program | Grow repeat rate to 10% | 3–12 months |
| 🟡 Medium | Cancellation risk scoring in PMS | Reduce cancellations 10–15% | 6–12 months |
| 🟡 Medium | Corporate / Group segment growth | Diversify revenue mix | 6–18 months |
| 🟢 Standard | Family package development | Increase family LOS + spend | 3–6 months |
| 🟢 Standard | Source market localization | Improve international conversion | 6–12 months |

---

## Appendix: Data Quality Notes

- Dataset: Synthetic (5,000 rows), structurally mirrors the Kaggle Hotel Booking Demand dataset
- Missing values handled: `children` → 0, `country` → "Unknown", `agent` → 0
- Derived features created: `total_stay_nights`, `total_guests`, `revenue_estimate`, `season`, `room_type_match`, `has_children`
- Revenue estimates are approximations based on `ADR × total_stay_nights`; actual revenue requires inclusion of F&B, ancillary, and service charges

---

*For questions about this analysis, refer to the Jupyter Notebook (`Hotel_Booking_EDA.ipynb`) or the source script (`src/eda_analysis.py`).*
