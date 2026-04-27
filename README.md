# Project: The "Sugar Trap" Market Gap Analysis 
**Client:** Helix CPG Partners  
**Objective:** Identify "Blue Ocean" opportunities in the snack market by locating high-protein, low-sugar product gaps.

---

## A. Executive Summary
Our analysis of over 100,000 cleaned products from the Open Food Facts dataset reveals a significant **"Blue Ocean"** opportunity in the **Savory Snacks** category. While the market is oversaturated with high-sugar options (e.g., Sweet Snacks showing a low 0.63 efficiency ratio), Savory Snacks represent a clear demand gap for products offering over **15g of protein** with less than **10g of sugar**. 

Data shows that the most successful high-protein products currently rely on **Milk, Soy, and Peanuts** as primary protein sources. We recommend developing a savory snack line that targets a **Protein Efficiency Ratio of 1.5 or higher** to dominate this underserved healthy snacking segment.

---

## B. Project Links
*   **Interactive Notebook:** https://colab.research.google.com/drive/1v2XE2Ibj6A2gvm38fZn9VEXQqYPsoplM?usp=sharing
*   **Interactive Dashboard:** https://github.com/Ivan-SHYAKA/sugar-trap-market-analysis/blob/main/Helix_CPG_Dashboard.html
*   **Strategic Presentation:** https://docs.google.com/presentation/d/e/2PACX-1vRvGnww72QPpnjAaGh649656POApAM-xQ8tbykPjMgywV5qUoUx01SCvw58VORmsKTVf7J1OeLOA7_H/pub?start=true&loop=false&delayms=3000

---

## C. Technical Explanation

### **1. Data Cleaning (Story 1 & 2)**
*   **Handling Ingestion:** Processed a 500,000-row subset of the Open Food Facts database.
*   **The Clean Up:** Removed 396,330 rows with missing names, sugars, or proteins to ensure statistical integrity. I further filtered for biologically plausible values (0g-100g per 100g).
*   **Category Wrangling:** Developed a keyword-based logic to map 10,000+ messy tags into 5 clean "Primary Categories": *Savory Snacks, Sweet Snacks, Dairy, Beverages, and Ready Meals.*

### **2. The Nutrient Matrix (Story 3 & 4)**
*   Developed an interactive Plotly scatter plot to visualize the sugar-to-protein relationship.
*   Identified the **"Blue Ocean Quadrant"** (Top-Left: High Protein/Low Sugar), specifically highlighting Savory Snacks as the prime area for R&D focus.

### **3. The Hidden Gem (Story 5)**
*   Analyzed the `ingredients_text` of the high-protein cluster.
*   **Top 3 Protein Sources Identified:** 
    1. **Milk** (1,786 products)
    2. **Soy** (945 products)
    3. **Peanuts** (512 products)

### **4. Candidate's Choice: Protein Efficiency Metric**
*   **The Innovation:** I introduced the **"Protein Efficiency Ratio"** ($Protein / (Sugar + 1)$).
*   **Why?** Raw totals don't tell the whole story. This metric allows Helix CPG to identify which categories provide the most "nutritional bang for your buck." 
*   **Result:** **Dairy Products** lead with a 9.34 ratio, but **Savory Snacks (1.57)** represent the best growth opportunity for a traditional snack manufacturer compared to the failing **Sweet Snacks (0.63)**.
