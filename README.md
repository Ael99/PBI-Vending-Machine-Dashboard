# Vending Machine Analytics — Power BI Dashboard

## Business Context
Vending machine operations in HCMC, March–May 2020.  
Includes COVID-19 lockdown period (Apr 1–15) — daily revenue dropped 28%.  
**Goal:** Identify revenue growth opportunities via Diagnostic Analysis.

---

## Dataset — Star Schema (7 tables)
| Table | Description | Size |
|-------|-------------|------|
| fBanHang | Transactions (fact) | 115,679 rows |
| dDanhSachMay | Machine master | 177 machines |
| dDiaDiemCha | Location — district/type | 18 districts |
| dSanPham | Products | 260 SKUs |
| dPaymentType | Payment methods | 5 types |
| dDate | Date dimension | — |

---

## Key Findings
- **1,137M VND** total revenue / **115,679** transactions / **177** machines
- **58 machines (33%)** below 50% median — only 4.3% of revenue
- Root cause: Low machines avg **8.4 SKUs** vs **52.1** for Top machines
- **Binh Tan** highest rev/machine (20.2M/month) but lowest digital rate (10.1%)
- Potential uplift: **+186M VND (+16%)** if low machines reach median

---

## Revenue Growth Levers
| Lever | Action | Estimated Uplift |
|-------|--------|-----------------|
| Lever 1 | Activate 58 underperforming machines | +186M VND |
| Lever 3 | Fix digital payment bottleneck (Binh Tan) | +832K VND |

---

## Dashboard Pages
| Page | Content |
|------|---------|
| Overview | KPIs, daily revenue trend, payment & category mix |
| Geography | Rev/machine by district, machine segments, scatter |
| Product | Pareto top 10 SKUs, category mix by location type |
| Payment | Digital rate by district, cash vs digital ticket |
| Machine | Low performer table, uplift potential |
| Report | Summary matrix — month × district × payment |

---

## Tools
- Power BI Desktop June 2026 — 20+ DAX measures, 2 calculated columns
- AppSource: OKViz Card with States, Pareto by sio2Graph
- Python/pandas — EDA & data validation

---

## Files
| File | Description |
|------|-------------|
| `FinalTest-v4.pbix` | Power BI dashboard |
| `Data.xlsx` | Raw data |
| `Revenue_Growth_Analysis.pptx` | Data storytelling deck |

---

## Screenshots
![Overview](images/overview.png)
![Geography](images/geography.png)
![Product](images/product.png)
![Payment](images/payment.png)
![Machine](images/machine.png)
![Report](images/report.png)
