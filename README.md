# Dream-House

# Structural Analysis & Design of RC Multi-Story Building

## 📋 Project Overview
This project involves the structural analysis and design of a multi-story reinforced concrete building. The geometry and preliminary drafting were handled in **AutoCAD**, while the structural modeling, loading, and Finite Element Analysis (FEA) were performed using **Bentley STAAD.Pro**.

The structure is modeled as a 3D Space frame consisting of beam elements, column elements, and shell (plate) elements for slabs.

## 🛠️ Tools & Technologies
* **STAAD.Pro:** For structural modeling, load application, and stiffness matrix analysis.
* **AutoCAD:** For architectural planning and geometric drafting.

## 🏗️ Structural Specifications
Based on the input data (`autocad_project _Abhinav.std`), the structure possesses the following properties:

### Geometry & Materials
* [cite_start]**Structure Type:** Space Frame (3D) [cite: 1]
* [cite_start]**Material:** Isotropic Concrete [cite: 80]
    * [cite_start]Young's Modulus ($E$): $21.7 \times 10^6$ kN/m² [cite: 80]
    * [cite_start]Density: $23.56$ kN/m³ [cite: 80]
    * [cite_start]Concrete Strength ($f_{cu}$): $27,579$ kN/m² (approx M25/M30 grade) [cite: 80]
* [cite_start]**Support Conditions:** Fixed supports at the foundation level (Nodes 77-96)[cite: 80].

### Section Properties
| Element Type | Dimensions | Description | Source |
| :--- | :--- | :--- | :--- |
| **Beams** | 230mm x 230mm | [cite_start]Prismatic (0.23m x 0.23m) | [cite: 80] |
| **Columns** | 230mm x 230mm | [cite_start]Prismatic (0.23m x 0.23m) | [cite: 80] |
| **Slabs (Plates)** | 150mm | [cite_start]Thickness (0.15m) | [cite: 80] |

## 📉 Load Cases & Combinations
The structure is designed for the following load conditions:

### [cite_start]1. Dead Load (DL) [cite: 80]
* **Self-Weight:** Applied in the global Y-direction (-1 factor).
* [cite_start]**Wall/Member Loads:** * Uniform distributed load of **-14.72 kN/m** on main beams[cite: 81].
    * [cite_start]Uniform distributed load of **-4.6 kN/m** on secondary members[cite: 81].
* [cite_start]**Floor Finish/Dead Load:** Plate pressure of **-1.0 kN/m²**[cite: 80, 81].

### [cite_start]2. Live Load (LL) [cite: 81]
* [cite_start]**Floor Live Load:** Plate pressure of **-2.5 kN/m²** acting on shell elements[cite: 81].

### [cite_start]3. Load Combinations [cite: 81]
* **Ultimate Limit State:** `1.5 x Dead Load + 1.5 x Live Load`

## 📂 File Structure
```text
├── autocad_project _Abhinav.std    # Main STAAD.Pro Input File
├── autocad_project _Abhinav.dwg    # AutoCAD Geometry File (Optional)
└── README.md                       # Project Documentation

```
### 🚀 How to Run the Analysis

### 1. Clone the Repository
Open your terminal or command prompt and run the following command:

```bash
git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
```

### 2. Open in STAAD.Pro
1. Launch **STAAD.Pro Connect Edition**.
2. Navigate to the cloned folder.
3. Open the file: `autocad_project _Abhinav.std`.

### 3. Run Analysis
1. Go to the top menu: **Analysis** -> **Run Analysis**.
2. Once finished, check the Output file (`.ANL`) to verify the results and ensure there are no errors.

### 4. View Results
Switch to **Post-Processing** mode to visualize:
* **Displacement:** Nodal deflections.
* **Bending Moments:** Moment diagrams (Mz).
* **Shear Forces:** Shear diagrams (Fy).

---

## 📷 Visuals
* STAAD 3D Render
* AutoCAD Plan

---

## 👤 Author
**Abhinav**
*Civil/Structural Engineer*
