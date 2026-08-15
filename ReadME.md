# Sphere of Petals - Stereolithography (SLA) 3D Printing & Design Iteration

A high-precision hollow geometric sphere featuring a symmetrical floral motif, fabricated using Stereolithography (SLA) technology for **ME 557: Additive Manufacturing**[cite: 2]. This repository documents the CAD modeling, scale iteration, wall-thickness optimization, and post-processing strategies required to print complex organic geometries[cite: 2].

---

## 🛠️ Project Overview

The **Sphere of Petals** is a $4 \times 4 \times 4\text{ cm}^3$ hollow sphere featuring seven circular cutouts aligned to create a mirrored three-dimensional floral motif across its top and bottom surfaces[cite: 2]. The geometry takes advantage of additive manufacturing to produce complex internal voids and fine structural features that are unachievable through traditional subtractive machining[cite: 2].

* **Dimensions:** $4 \times 4 \times 4\text{ cm}^3$[cite: 2]
* **Fabrication Method:** Stereolithography (SLA)[cite: 2]
* **Key Challenge:** Balancing wall thickness against resin fragility during support removal while preserving hollow internal features[cite: 2].

---

## ⚙️ Hardware & Materials

* **3D Printer:** FormLabs SLA Printer[cite: 2]
* **Material:** Clear Resin[cite: 2]
* **Software:** CAD Modeling Software[cite: 2]

---

## 🔄 Design Iteration & Optimization

To achieve a successful print, the geometry underwent an iterative design process to resolve structural failure during post-processing:

| Design Iteration | Dimensions | Wall Thickness | Result & Observation |
| :--- | :--- | :--- | :--- |
| **Initial Concept** | $2 \times 2 \times 2\text{ cm}^3$[cite: 2] | $1\text{ mm}$[cite: 2] | **Failed:** Structure was overly fragile and broke during external support removal with snippers[cite: 2]. |
| **Final Optimized Design** | $4 \times 4 \times 4\text{ cm}^3$[cite: 2] | $3\text{ mm}$ ($+2\text{ mm}$ increase)[cite: 2] | **Success:** Provided sufficient structural integrity for clean external support removal while maintaining the hollow geometry[cite: 2]. |

---

## 💡 Engineering Insights

* **Thin Wall Limitations in SLA:** Extremely thin resin geometries ($1\text{ mm}$) exhibit high fragility before full post-curing, leading to shear failure during mechanical support removal[cite: 2].
* **Support Management:** Increasing the wall thickness to $3\text{ mm}$ enabled safe removal of external supports[cite: 2]. While necessary internal supports remained due to the enclosed hollow structure, the outer aesthetic floral pattern and overall shape remained fully intact[cite: 2].

---

## 📂 Repository Structure

```text
├── CAD/                    # CAD model source files (.STEP, .SLDPRT)
├── STL/                    # 3D Printable STL files
├── media/                  # Print photos and renders
│   └── sphere_of_petals.jpg
└── README.md               # Project documentation
