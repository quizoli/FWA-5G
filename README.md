# README: 50-Site 5G NR Band n50 (1.5 GHz) GIDA FWA Network & OPEX Financial Model

## 1. Project Overview & Scope
This project delivers a complete technical rollout plan, spatial GIS dataset, interactive web portal, and financial sustainability model for a **50-site Fixed Wireless Access (FWA)** network operating on **5G NR Band n50 (1.5 GHz / 1432–1517 MHz TDD)**.

The network targets the highest-density unserved and underserved rural/GIDA clusters in the Philippines, identified through spatial analysis of all **42,048 Philippine barangays** cross-referenced with **251,898 crowdsourced Ookla Speedtest tiles (2026 Q1–Q3)**.

### Core Architecture & Business Model Directives
1. **Physical Planning Scope**: Strictly **50 Base Station (BTS) Sites** (`N50-0001` to `N50-0050`), each with a **6.0 km coverage radius** on Band n50.
2. **Cluster Reach**: The 50 sites collectively cover **473 unserved and underserved barangays** (372 Tier 1 True Unserved + 101 Tier 2 Underserved) with a total 2020 Census population of **836,264 citizens**.
3. **Addressable Households (No Arbitrary 1,000 Subs Cap)**: Based on official Philippine Statistics Authority (PSA) 2020 Census of Population and Housing (CPH) regional average household sizes, these 473 barangays contain **175,820 estimated households** (averaging **3,516 households per site**, ranging from 1,852 to 8,057 HH/site).
4. **Non-Recoverable Government CAPEX Grant**: The government infuses 100% of the initial capital expenditure (CAPEX) for base station infrastructure and customer premises equipment (CPE) as a public social infrastructure grant. **The government does not recover this CAPEX from subscriber tariffs (0% capital recovery burden on tariffs).**
5. **No Core Network CAPEX ($0 Upfront Core)**: Core hardware and software ($2.805M) are eliminated from CAPEX. Instead, the Core Supplier is compensated on a pay-as-you-grow basis at **₱10.00 per active subscriber per month** in OPEX.
6. **Regulatory Spectrum User Fee (SUF)**: In lieu of the established NTC bandwidth/station SUF, the regulatory fee is set at a flat **₱5.00 per active subscriber per month**.
7. **OPEX-Only Pricing & ROI Dimensioning**: Because CAPEX recovery is 0%, subscriber tariffs and break-even / return-on-investment (ROI) thresholds are calculated **strictly against annual operating expenditure (OPEX)**.

---

## 2. Directory of Project Deliverables

| Deliverable | File Path | Format & Description |
| :--- | :--- | :--- |
| **Interactive Web Portal** | [GIDA_n50_FWA_Portal.html](file:///Users/olivertungol/Library/CloudStorage/OneDrive-Personal/Comclark/GIDA%20FWA/GIDA_n50_FWA_Portal.html) | Standalone 5-tab SPA: Interactive Map (50 sites + 6km rings), OPEX & Pricing Simulator, BoQ & Regional Breakdown, Searchable Directory, and Proposal Reader. |
| **Portal Artifact** | [gida_n50_fwa_portal.html](file:///Users/olivertungol/.gemini/antigravity/brain/732157b4-2583-4984-a2d8-985020cad97c/gida_n50_fwa_portal.html) | Mirror artifact located in Antigravity app data. |
| **Formal DICT Proposal (Word)** | [DICT_50_Site_n50_FWA_Formal_Proposal.docx](file:///Users/olivertungol/Library/CloudStorage/OneDrive-Personal/Comclark/GIDA%20FWA/DICT_50_Site_n50_FWA_Formal_Proposal.docx) | Formal submission document for DICT leadership with executive summary, legal preambles, BoQ, and financial schedules. |
| **Formal Proposal Artifact (MD)** | [government_fwa_proposal.md](file:///Users/olivertungol/.gemini/antigravity/brain/732157b4-2583-4984-a2d8-985020cad97c/government_fwa_proposal.md) | Full text proposal in GitHub-flavored markdown. |
| **Master Financial & GIS Model** | [PH_Unserved_n50_Network_Plan_and_Cost_Model.xlsx](file:///Users/olivertungol/Library/CloudStorage/OneDrive-Personal/Comclark/GIDA%20FWA/PH_Unserved_n50_Network_Plan_and_Cost_Model.xlsx) | 12-sheet Excel model including OPEX ROI model, executive summary, regional/provincial summaries, 50 site details, and national barangay database. |
| **Proposed Sites GIS Layer** | [PH_Proposed_n50_Sites.geojson](file:///Users/olivertungol/Library/CloudStorage/OneDrive-Personal/Comclark/GIDA%20FWA/PH_Proposed_n50_Sites.geojson) | GeoJSON points for strictly 50 sites with population, household, and coverage attributes. |
| **Unserved Barangays Layer** | [PH_Unserved_Underserved_Barangays.geojson](file:///Users/olivertungol/Library/CloudStorage/OneDrive-Personal/Comclark/GIDA%20FWA/PH_Unserved_Underserved_Barangays.geojson) | GeoJSON points for all 3,355 unserved/underserved barangays in the country. |
| **Google Earth KML Layer** | [PH_Unserved_Network_Plan.kml](file:///Users/olivertungol/Library/CloudStorage/OneDrive-Personal/Comclark/GIDA%20FWA/PH_Unserved_Network_Plan.kml) | KML map for viewing in Google Earth Pro / Web. |

---

## 3. Explaining the Financial & Operational Matrix

In the proposal, dashboard, and Excel sheets, you will encounter the **Subscriber & OPEX Sustainability Matrix**. Below is a line-by-line explanation of every column, entry, and metric.

### The Summary Matrix Table

| Pricing Mechanism & Fixed OPEX Case | Gross / Net ARPU | 1. 100% OPEX Break-Even (`1.00x OPEX`) | 2. +15% Operator ROI on OPEX (`1.15x OPEX`) | 3. +20% Operator Net Margin (`1.25x OPEX`) | 4. +30% Operator ROI on OPEX (`1.30x OPEX`) |
| :--- | ---: | ---: | ---: | ---: | ---: |
| **M1: Ultra-Low Social Mix (`₱399/₱599/₱999`)** — *Solar OPEX* | ₱539 / **₱451.81** | **35,988 HHs** *(720/site \| 20.5%)* | **41,387 HHs** *(828/site \| 23.5%)* | **44,985 HHs** *(900/site \| 25.6%)* | **46,785 HHs** *(936/site \| 26.6%)* |
| **M2: Affordable GIDA Social-First (`₱499/₱699/₱1,299`)** — *Solar OPEX* | ₱709 / **₱599.04** | **27,143 HHs** *(543/site \| 15.4%)* | **31,215 HHs** *(624/site \| 17.8%)* | **33,929 HHs** *(679/site \| 19.3%)* | **35,286 HHs** *(706/site \| 20.1%)* |
| **M2: Affordable GIDA + LGU Anchor (`₱54M/yr`)** — *Solar OPEX* | ₱709 / **₱599.04** | **19,631 HHs** *(393/site \| 11.2%)* | **22,576 HHs** *(452/site \| 12.8%)* | **24,539 HHs** *(491/site \| 14.0%)* | **25,521 HHs** *(510/site \| 14.5%)* |
| **M3: Uniform Single Tier (`₱799`)** — *Solar OPEX* | ₱799 / **₱676.99** | **24,018 HHs** *(480/site \| 13.7%)* | **27,621 HHs** *(552/site \| 15.7%)* | **30,023 HHs** *(600/site \| 17.1%)* | **31,223 HHs** *(624/site \| 17.8%)* |
| **M4: Optimum 4-Tier Mix (`₱499/₱899/₱1,699/₱3,499`)** — *Base OPEX* | ₱1,069 / **₱910.83** | **26,350 HHs** *(527/site \| 15.0%)* | **30,302 HHs** *(606/site \| 17.2%)* | **32,937 HHs** *(659/site \| 18.7%)* | **34,254 HHs** *(685/site \| 19.5%)* |
| **M4: Optimum 4-Tier Mix** — *Solar OPEX* | ₱1,069 / **₱910.83** | **17,852 HHs** *(357/site \| 10.2%)* | **20,530 HHs** *(411/site \| 11.7%)* | **22,315 HHs** *(446/site \| 12.7%)* | **23,207 HHs** *(464/site \| 13.2%)* |
| **M4: Optimum 4-Tier + LGU Anchor (`₱54M/yr`)** — *Solar OPEX* | ₱1,069 / **₱910.83** | **12,911 HHs** *(258/site \| 7.3%)* | **14,848 HHs** *(297/site \| 8.4%)* | **16,139 HHs** *(323/site \| 9.2%)* | **16,785 HHs** *(336/site \| 9.5%)* |

---

### Detailed Explanation of Entries

#### 1. "Gross / Net ARPU"
- **Gross ARPU (Average Revenue Per User)**: The weighted average monthly subscription price before taxes and deductions.
  - *Example (M4 Optimum)*: (30% × ₱499) + (45% × ₱899) + (20% × ₱1,699) + (5% × ₱3,499) = **₱1,069.00 / month**.
- **Net ARPU (Net Operating Contribution)**: The actual net cash kept by the operating partner each month per subscriber after mandatory statutory and operational deductions:
  $$\text{Net ARPU} = \left(\text{Gross ARPU} \times \frac{1}{1.12} \times 0.97\right) - \text{SUF (₱5)} - \text{Core Fee (₱10)}$$
  1. **VAT Exclusion ($\frac{1}{1.12}$)**: Removes 12% Value Added Tax.
  2. **Collection Risk Allowance ($0.97$)**: Deducts 3% for rural bad debt, billing disputes, and payment gateway fees.
  3. **SUF Deduction ($-₱5.00$)**: Government regulatory spectrum charge per subscriber.
  4. **Core Supplier Fee ($-₱10.00$)**: Fee paid to the Core software vendor per subscriber.
  - *Result for M4*: `(₱1,069 ÷ 1.12 × 0.97) - ₱5.00 - ₱10.00` = **₱910.83 / month** (or **₱10,929.96 / year**).

#### 2. Fixed Annual OPEX Modes
- **Base OPEX (₱288,000,000 / year = $4.80M / year)**: Unadjusted spreadsheet OPEX covering 50 sites: commercial grid electricity ($1.50M), diesel fuel ($1.08M), active O&M ($0.90M), passive O&M ($0.60M), and 200 Starlink 8TB subscriptions ($0.72M). Average: **₱480,000 / site / month**.
- **Solar-Optimized OPEX (₱195,120,000 / year = $3.252M / year)**: Reflects that every site is equipped with a 16kW solar array + 450AH lithium-ion battery plant in CAPEX, offsetting 60% of grid power and diesel fuel. Average: **₱325,200 / site / month**.
- **LGU Anchor Revenue Deduction (₱54,000,000 / year)**: When DICT/LGUs contract 6 dedicated institutional connections per site (300 endpoints total across 473 barangays: schools, barangay halls, rural health units) at ₱15,000/month, ₱54M/year in guaranteed wholesale revenue offsets the fixed OPEX, lowering the net fixed cash required from retail subscribers to **₱141.12M / year**.

#### 3. "Total HHs" (Total Connected Households)
- The absolute number of active paying households required across all 50 sites to hit the financial milestone.
- **Formula**:
  $$\text{Break-Even Subscribers} = \frac{\text{Fixed Annual OPEX} - \text{Anchor Revenue}}{\text{Net Annual Contribution per Household}}$$
  - *Example (M4 Solar + Anchor)*:
    $$\frac{₱195,120,000 - ₱54,000,000}{₱10,929.96} = \mathbf{12,911\text{ Households}}$$

#### 4. "Subs Per Site" (Average Subscribers per BTS)
- Total connected households divided evenly across the 50 sites:
  $$\text{Subs Per Site} = \frac{\text{Total Connected HHs}}{50}$$
  - *Example*: $12,911 \div 50 = \mathbf{258\text{ subscribers/site}}$.
- **Significance**: In prior versions, an arbitrary cap of 1,000 subscribers per BTS was assumed. Here, 258 subscribers per site is well within the 5G NR n50 radio cell capacity (which can support 1,500+ active connections on a 3-sector site with Starlink/LEO backhaul).

#### 5. "Percentage (%)" (Household Penetration Rate)
- **What it represents**: The percentage of the **total addressable households living within the 50 site footprints** that must subscribe to hit the milestone:
  $$\text{Percentage (\%)} = \frac{\text{Total Connected HHs}}{\text{Total Addressable Households (175,820)}} \times 100\%$$
- **Why it matters**:
  - The 50 sites encompass **175,820 estimated households** (average 3,516 households per site).
  - A break-even figure of **7.3%** means the network becomes self-sustaining if **fewer than 8 out of every 100 households** inside the coverage area sign up.
  - A +20% net margin figure of **9.2%** means that with just **9 to 10 out of every 100 households** subscribing, the private operator covers all operating costs and earns a 20% profit margin.
  - Over **90% of households remain unserved/untapped headroom** for future organic growth.

#### 6. Financial Threshold Columns
1. **100% OPEX Break-Even (1.00x OPEX)**:
   - Operating EBITDA is exactly ₱0.00. Revenue covers 100% of power, Starlink backhaul, site maintenance, ₱5 SUF, and ₱10 Core fee.
2. **+15% Operator ROI on OPEX (1.15x OPEX)**:
   - Retail revenue covers OPEX plus a 15% operating profit surplus for commercial reserves and working capital.
3. **+20% Operator Net Margin (1.25x OPEX)**:
   - Standard commercial benchmark for telecom operating partners. Represents an annual cash surplus equal to 20% of gross revenue (or 25% over net OPEX).
4. **+30% Operator ROI on OPEX (1.30x OPEX)**:
   - High-yield scenario providing ample cash flow to fund local field expansions or community Wi-Fi additions.

---

## 4. Key Takeaway & Policy Recommendations
Because the Philippine government treats this 50-site deployment as a **non-recoverable social connectivity grant**:
1. **Unprecedented Affordability**: Plans as low as **₱499/month (Social Lifeline)** and **₱699/month (Standard Family)** are commercially sustainable for the operating partner.
2. **Minimal Commercial Risk**: The operator achieves full financial self-sufficiency with only **7.3% to 15.4% household market penetration** across the covered GIDA communities.
3. **High Capacity Headroom**: Because the 50 sites average 3,516 households per cell, removing the 1,000-subscriber limit allows high-density barangays to grow dynamically as digital adoption accelerates.
