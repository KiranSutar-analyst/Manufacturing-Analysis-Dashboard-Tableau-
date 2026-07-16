Manufacturing Analysis Dashboard (Tableau)

A Tableau dashboard built to track where manufacturing wastage comes from — broken down by machine, employee, department, and delivery timeline — so quality issues can be spotted and acted on quickly rather than discovered at month-end.

📸 Dashboard_preview.png



Note: The underlying dataset is not shared publicly due to confidentiality; this repo showcases the dashboard design and analytical approach.

📌 What This Dashboard Answers

Working with production and rejection logs, this dashboard was designed to answer a few recurring operational questions:


How much is actually being manufactured, processed, and rejected — and at what rate?
Which specific machines are driving the most rejections?
Is any one employee or shift responsible for higher defect rates, or is it more systemic?
Does delivery urgency (early vs on-time vs late) affect quality?
How does output and wastage move together across the year?


📊 Headline Numbers

MetricValueManufactured Qty60.05MProcessed Qty60.02MRejected Qty491.02KWastage %1%

🔍 What Stood Out in the Data


Two machines — MC027 and MC026 — drive a disproportionate share of rejections (80.05K and 68.46K respectively), well ahead of every other machine. If maintenance budget is limited, these two are the obvious starting point.
Rejection numbers across employees are close together (120K–127K range), which points toward the problem sitting more with equipment or process than with any individual's work.
Rushing deliveries seems to cost quality: Early-delivery batches had the highest rejection count (167.59K) versus On Time (160.28K) and Late (163.15K).
Rejections track volume, not a fixed defect rate — the months with the highest output (like March and June) also show the sharpest spikes in rejected units, rather than rejections staying flat regardless of how much was produced.
Knitwear stands out among departments, carrying the highest combined manufactured and rejected quantity — worth a closer quality-control look.


🛠️ How the Dashboard Was Built


Calculated fields for the KPI summary cards and the wastage percentage
Dashboard-wide filter actions across Month of Doc Date, Delivery Period, Buyer, Employee Name, and Department Name, so every chart updates together from a single filter change
A consistent color-intensity legend (light to dark) applied across all rejection-related bars, so scanning for "worst offenders" is visual rather than numeric
A mix of chart types — horizontal bars, a donut breakdown, a combo bar-and-line trend chart, and ranked bar lists — chosen individually based on what each question needed rather than defaulting to one chart style throughout
A collapsible filter panel — the funnel icon expands the full set of filters and legends for users who want to dig in, and collapses back down to keep the view clean for a quick glance


📁 What's in This Repo

Manufacturing-Analysis-Dashboard-Tableau/
├── manufacturing_analysis.twbx    # Tableau workbook
├── screenshots/
│   └── dashboard_overview.png      # Dashboard preview image
└── README.md

🎯 Why This Matters for the Business

A dashboard like this gives a plant manager a fast way to:


Prioritize which machines need servicing based on actual rejection data, not guesswork
Weigh whether pushing for early deliveries is worth the quality trade-off
Track department and employee performance without building a report by hand each time
Back quality-control investment decisions with numbers instead of instinct



Part of my data analytics portfolio — happy to hear feedback or questions.
ContentREADME.md71 linesmd
