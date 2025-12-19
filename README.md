# claims-annalysis
# Healthcare Claims Data Analysis

## Project Description
This project analyzes a sample of prospective healthcare claims data to identify billing patterns, common diagnoses/procedures, payer mix, place of service patterns, and relationships between claim complexity and charges.

## Data Source Information
The analysis uses three relational CSV files:
- **HEADER** (`*_HEADER.csv`): one row per claim (claim identifiers, provider/payer, service dates, place of service).
- **LINE** (`*_LINE.csv`): one row per service line (HCPCS/CPT codes and line-level charges).
- **CODE** (`*_CODE.csv`): one row per diagnosis code on the claim (ICD-10 codes).

Key join key across all files: `ProspectiveClaimId`.

## How to Run the Notebook
### Google Colab (recommended)
1. Open `notebook.ipynb` in Google Colab.
2. Upload the three CSV files into the Colab session (Files panel → Upload).
3. Run cells top-to-bottom.

### Local (optional)
1. Install dependencies:
   ```bash
   pip install -r requirements.txt
