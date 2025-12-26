# Settlement Recognized Loss Calculator

## What Is It?

A web-based calculator tool that computes **recognized losses** for securities litigation settlements. It calculates how much financial loss individual investors experienced during class-action security settlement periods (like Twitter and Kraft Heinz) using the **Simple Average Cost Basis methodology**.

## What It Does

The calculator:
- **Processes settlement data** from multiple securities cases
- **Calculates per-client losses** based on shares sold during settlement periods
- **Aggregates losses by fund** to show which investments were most affected
- **Generates detailed reports** showing loss percentages and distributions
- **Handles CSV file uploads** for easy data input

### Example Results
- **Twitter Settlement**: $146,145.43 total recognized loss across 3 clients
- **Kraft Heinz Settlement**: $9,110,130.10 total recognized loss across 3 clients

---

## Technologies Used

### Frontend
- **HTML5** - Structure and layout
- **CSS3** - Modern styling with grid layouts and responsive design
- **JavaScript** - Core calculation logic and interactivity
- **Papa Parse (CSV parsing library)** - Reads and processes CSV files

### Features
- **Interactive web interface** - No installation required
- **Real-time calculations** - Results update instantly
- **Data visualization** - Tables and metrics display
- **File upload support** - Import client data via CSV
- **Template download** - Pre-formatted CSV templates for data input

---

## How It Works

### 1. **Data Input**
Users upload a CSV file containing:
- Client name
- Fund ID
- Shares purchased
- Purchase price
- Shares sold
- Sale price
- Sale date

### 2. **Calculation Process**
The calculator applies the **Purchase Loss Method**:
```
Recognized Loss = (Sale Price - Average Cost Basis) × Shares Sold
```

Where:
- **Average Cost Basis** = Total purchase cost ÷ Total shares purchased
- **Sale Price** = Market price at time of sale
- **Shares Sold** = Number of shares sold during settlement period

### 3. **Aggregation**
Results are grouped by:
- **Client** - Shows which investors had the largest losses
- **Fund** - Identifies which investment funds were most impacted
- **Total** - Overall settlement loss amount

### 4. **Output**
Displays:
- Loss per client with percentage breakdown
- Loss per fund with share volume
- Visual metrics and formatted tables
- Full data reconciliation

---

## What It's Used For

### For Investors
- **Determine settlement eligibility** - Calculate if you have qualifying losses
- **Understand financial impact** - See exact loss amounts
- **Track fund performance** - Identify which investments were affected most

### For Law Firms
- **Client communication** - Provide clear loss calculations to claimants
- **Settlement claims** - Document losses for submission to settlement administrators
- **Audit trail** - Verify calculations are accurate and defensible

### For Settlement Administrators
- **Claims processing** - Quickly verify investor loss amounts
- **Distribution calculations** - Determine fair settlement payouts
- **Compliance documentation** - Maintain detailed records

---

## Why It's Useful

✅ **Accuracy** - Uses standardized cost basis methodology consistent with securities law
✅ **Speed** - Calculates hundreds of investor losses in seconds
✅ **Transparency** - Shows detailed breakdown by client and fund
✅ **Ease of Use** - Simple interface, no accounting knowledge required
✅ **No Installation** - Works directly in any web browser
✅ **Reconciliation** - Totals automatically verify for accuracy
✅ **Professional Grade** - Used for actual securities litigation settlements

---

## How to Use

1. **Open** `settlement_calculator.html` in your web browser
2. **Select** the settlement case (Twitter or Kraft Heinz)
3. **Upload** your CSV file with client data
4. **View** calculated results instantly
5. **Review** detailed breakdowns by client and fund
6. **Export** or print results as needed

---

## File Structure

```
DDRT-Settlement-Calculator/
├── settlement_calculator.html  # Main calculator application
├── WRITTEN_RESPONSE.txt        # Detailed analysis results
├── README.md                   # This file
├── client-data/
│   ├── Twitter_final.csv       # Sample Twitter settlement data
│   └── Kraft_final.csv         # Sample Kraft Heinz settlement data
└── Screenshots/                # Visual documentation
```

---

## Settlement Cases Supported

### Twitter, Inc. (N.D. Cal.) 2016
- **Total Loss**: $146,145.43
- **Clients**: 3
- **Top Fund**: Fund 22 ($77,259.44)
- **Period**: Securities sold during settlement window

### Kraft Heinz Securities Litigation
- **Total Loss**: $9,110,130.10
- **Clients**: 3
- **Top Fund**: Fund 34 ($5,211,180.23)
- **Period**: Securities sold during settlement window

---

## Technical Details

### Cost Basis Methodology
Uses **Simple Average Cost Basis** (weighted average method):
- Treats all shares of a security as purchased at the average cost
- Most conservative and widely accepted for securities settlements
- Complies with IRS regulations (Rev. Proc. 98-48)

### Accuracy
- Reconciles to the penny
- All client losses sum to total settlement loss
- Fund distributions account for 100% of total

### Browser Compatibility
Works on:
- Chrome/Edge (recommended)
- Firefox
- Safari
- Any modern browser with JavaScript enabled

---


