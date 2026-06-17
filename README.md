# 🏨 Elite Hotels International: Booking Demand & Guest Behavior Analysis

> **A portfolio-ready, end-to-end Exploratory Data Analysis (EDA) project in hospitality analytics.**  
> Built with Python | pandas | numpy | matplotlib | seaborn | scipy | scikit-learn

---

## 📋 Table of Contents

- [Business Context](#-business-context)
- [Project Structure](#-project-structure)
- [Dataset](#-dataset)
- [Key Findings](#-key-findings)
- [Visualizations](#-visualizations)
- [Setup & Installation](#-setup--installation)
- [How to Run](#-how-to-run)
- [Business Questions Answered](#-business-questions-answered)
- [Tech Stack](#-tech-stack)
- [Acknowledgements](#-acknowledgements)

---

## 🏢 Business Context

**Elite Hotels International** operates two hotel types — **City Hotel** and **Resort Hotel** — serving leisure and corporate travelers across Europe and globally.

The business objective of this project is to perform a complete Exploratory Data Analysis to:

- Understand **booking demand patterns** and seasonal trends
- Identify **cancellation drivers** and quantify revenue at risk
- Profile **guest segments** by behavior, geography, and preferences
- Surface **revenue and ADR insights** by segment and period
- Generate **actionable recommendations** for hotel management and stakeholders

---

## 📁 Project Structure

```
elite-hotels-booking-analysis/
│
├── README.md                          ← You are here
├── requirements.txt                   ← Python dependencies
│
├── data/                              ← Place hotel_bookings.csv here (from Kaggle)
│
├── notebooks/
│   └── Hotel_Booking_EDA.ipynb        ← Full Jupyter Notebook walkthrough
│
├── src/
│   └── eda_analysis.py                ← Clean, modular Python EDA script
│
├── reports/
│   └── insights_and_recommendations.md  ← Business insights report
│
├── visuals/                           ← 27 exported PNG charts
│   ├── 00_executive_dashboard.png
│   ├── 01_bookings_by_hotel_type.png
│   ├── 02_monthly_booking_trends.png
│   └── ... (27 total)
│
└── sample_data/
    └── hotel_bookings_sample_500.csv  ← 500-row sample for quick testing
```

---

## 📊 Dataset

**Source:** [Kaggle — Hotel Booking Demand](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand)  
**Reference:** Antonio, N., de Almeida, A., & Nunes, L. (2019). *Hotel booking demand datasets*. Data in Brief. [DOI:10.1016/j.dib.2018.11.126](https://doi.org/10.1016/j.dib.2018.11.126)

| Property | Value |
|----------|-------|
| Rows | 119,390 (original) / 5,000 (synthetic) |
| Columns | 32 |
| Hotels | City Hotel, Resort Hotel |
| Period | July 2015 – August 2017 |
| Target Variable | `is_canceled` (binary: 0/1) |

### Key Columns

| Column | Description |
|--------|-------------|
| `hotel` | Hotel type: City Hotel or Resort Hotel |
| `is_canceled` | 1 = Canceled, 0 = Not canceled |
| `lead_time` | Days between booking and arrival |
| `adr` | Average Daily Rate (€) |
| `total_stay_nights` | Weekend + weekday nights (derived) |
| `revenue_estimate` | ADR × total_stay_nights (derived) |
| `season` | Spring / Summer / Autumn / Winter (derived) |
| `market_segment` | Online TA, Direct, Corporate, etc. |
| `customer_type` | Transient, Contract, Group, Transient-Party |
| `deposit_type` | No Deposit, Non Refund, Refundable |

---

## 🔍 Key Findings

### 📉 Cancellation Crisis
- **37% cancellation rate** — well above the 20–25% industry benchmark
- **Estimated €1.26M in revenue lost** to cancellations
- Longer lead time and "No Deposit" bookings are the top cancellation risk factors

### 📈 Revenue Drivers
- **City Hotel** commands a higher ADR (~€110 vs €95)
- **Direct and Corporate** segments yield the highest ADR — OTA dependency suppresses yield
- **Summer** (July–September) is the peak revenue period for both hotel types

### 👥 Guest Behavior
- **Only 3.1%** of guests are returning customers — loyalty infrastructure gap
- **Portugal** is the dominant source market, followed by UK, France, Spain, Germany
- **Transient** customers (75%) drive volume but carry the highest cancellation risk
- Guests with **more special requests cancel less** — a proxy for booking commitment

### 🛎️ Operational Patterns
- **BB (Bed & Breakfast)** is the dominant meal plan (~77%)
- **~88%** of guests receive a different room type than reserved (audit needed)
- **~14%** of bookings spend time on the waiting list

---

## 🖼️ Visualizations

27 professional charts produced across 7 analysis dimensions:

| # | Chart | Type |
|---|-------|------|
| 00 | Executive Analytics Dashboard | Dark Dashboard |
| 01 | Bookings by Hotel Type | Bar + Cancellation Rate |
| 02 | Monthly Booking Trends | Line Chart |
| 03 | Yearly Booking Volume | Grouped Bar |
| 04 | Month × Year Heatmap | Heatmap |
| 05 | Overall Cancellation Rate | Donut Chart |
| 06 | Lead Time vs Cancellation | Box Plot |
| 07 | Seasonal Cancellation Rates | Bar Chart |
| 08 | Lead Time Distribution | Histogram Overlay |
| 09 | Top 15 Countries | Horizontal Bar |
| 10 | Customer Type Distribution | Bar Chart |
| 11 | New vs Repeated Guests | Pie Chart |
| 12 | Family Composition Analysis | Side-by-Side Bar |
| 13 | ADR by Hotel Type | Box Plot |
| 14 | ADR by Market Segment | Bar + Error Bars |
| 15 | Monthly Revenue Trend | Area Line Chart |
| 16 | Revenue Loss from Cancellations | Bar Chart |
| 17 | Stay Duration Distribution | Histogram |
| 18 | Booking Modifications | Bar Chart |
| 19 | Waiting List Duration | Histogram |
| 20 | Parking Demand | Bar Chart |
| 21 | Special Requests Distribution | Bar Chart |
| 22 | Special Requests by Customer Type | Bar Chart |
| 23 | Booking Changes vs Special Requests | Scatter |
| 24 | Meal Plan Preferences | Stacked % Bar |
| 25 | Correlation Matrix | Heatmap |
| 26 | Feature Importance (Cancellation) | Horizontal Bar |

---

## ⚙️ Setup & Installation

### Prerequisites
- Python 3.10+
- pip

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/yourusername/elite-hotels-booking-analysis.git
cd elite-hotels-booking-analysis

# 2. Create virtual environment (recommended)
python -m venv venv
source venv/bin/activate        # macOS/Linux
venv\Scripts\activate           # Windows

# 3. Install dependencies
pip install -r requirements.txt
```

### Optional: Download Real Dataset
1. Go to [Kaggle Hotel Booking Demand](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand)
2. Download `hotel_bookings.csv`
3. Place it in the `data/` folder

---

## 🚀 How to Run

### Option A: Run Python Script (All Analyses)
```bash
python src/eda_analysis.py
```
This will:
- Generate a 5,000-row synthetic dataset (or load real data from `data/`)
- Run all EDA analyses
- Export 27 visualizations to `visuals/`
- Print business Q&A to console
- Export a 500-row sample to `sample_data/`

### Option B: Jupyter Notebook
```bash
jupyter notebook notebooks/Hotel_Booking_EDA.ipynb
```

### Using the Real Kaggle Dataset
To use the actual Kaggle dataset instead of synthetic data, modify the `main()` function in `src/eda_analysis.py`:

```python
# Replace:
df_raw = generate_synthetic_dataset(n=5_000, seed=42)

# With:
df_raw = pd.read_csv("data/hotel_bookings.csv")
```

---

## ❓ Business Questions Answered

### Basic Level
| Question | Answer |
|----------|--------|
| Overall cancellation rate? | ~37% |
| Peak booking month? | July |
| Top source country? | Portugal (PRT) |
| Which hotel has higher ADR? | City Hotel |
| % repeat guests? | ~3.1% |

### Medium Level
| Question | Answer |
|----------|--------|
| Does lead time drive cancellation? | Yes — longer lead time = higher risk |
| Top ADR market segment? | Direct / Aviation |
| Most popular meal plan? | BB (Bed & Breakfast) |
| Most revenue-generating season? | Summer |
| Do special requests reduce cancellation? | Yes — weakly but consistently |

### Advanced Level
| Question | Answer |
|----------|--------|
| Revenue lost to cancellations? | ~€1.26M (estimated) |
| Top cancellation predictor? | ADR, Lead Time, Stay Duration |
| Which deposit type cancels most? | No Deposit |
| Room type mismatch rate? | ~88% |
| Parking demand by hotel? | ~7–8% (both hotel types) |

---

## 🛠️ Tech Stack

| Library | Version | Purpose |
|---------|---------|---------|
| pandas | 2.1.4 | Data manipulation |
| numpy | 1.26.4 | Numerical computation |
| matplotlib | 3.8.2 | Base visualizations |
| seaborn | 0.13.2 | Statistical charts |
| scipy | 1.11.4 | Statistical tests |
| scikit-learn | 1.4.0 | Feature importance (Random Forest) |

---

## 📄 Deliverables

- ✅ `src/eda_analysis.py` — Clean, modular, documented Python script
- ✅ `notebooks/Hotel_Booking_EDA.ipynb` — Jupyter Notebook with narrative
- ✅ `reports/insights_and_recommendations.md` — Full business insights report
- ✅ `README.md` — Professional project documentation
- ✅ `requirements.txt` — Dependency list
- ✅ `sample_data/hotel_bookings_sample_500.csv` — 500-row sample dataset
- ✅ `visuals/` — 27 exported PNG visualizations

---

## 📚 Acknowledgements

- Dataset: [Jesse Mostipak on Kaggle](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand)
- Research: Antonio, N., de Almeida, A., & Nunes, L. (2019). *Hotel booking demand datasets*. Data in Brief, 22, 41–49.
- Built as part of a **Hospitality Analytics** portfolio project

---

## 📜 License

This project is available under the MIT License. The underlying dataset is subject to its original [Kaggle license](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand).

---

*⭐ If this project helped you, consider giving it a star on GitHub!*
