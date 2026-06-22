**Carbon Capture in Steam Methane Reforming — LCA Study**

A gate-to-gate Life Cycle Assessment (LCA) of CO₂ capture integrated with Steam Methane Reforming (SMR), submitted for the Sustainability Assessment course at Otto-von-Guericke University Magdeburg (Summer Semester 2026).

## Overleaf Project

View and edit the LaTeX report on Overleaf: [Open in Overleaf](https://www.overleaf.com/read/dgffffrgnmvg#042823)

**Overview****

Steam Methane Reforming is the dominant industrial route for hydrogen production but generates significant CO₂ emissions. This study quantifies the material and energy inputs required to capture 1 kg of CO₂ from an SMR-based hydrogen plant, modelled end-to-end in DWSIM and assessed in OpenLCA.

The system comprises three stages:


SMR Reactor — CH₄ + H₂O → CO + 3H₂ (endothermic, catalytic)
Water-Gas Shift (WGS) Reactor — CO + H₂O → CO₂ + H₂
CO₂ Separation & Compression — PSA unit, compound separator, three-stage compression train to supercritical conditions (110 bar)



**Key Results**

MetricValueFunctional unit1 kg captured CO₂CO₂ capture efficiency88.0%Total compression energy1.132 kWMethane input per kg CO₂0.979 kgSteam input per kg CO₂2.937 kgDominant energy consumerCompressor 6 — Stage 3 (1.532 MJ/kg CO₂)Dominant material consumerCooler 8 steel (1.50 × 10⁻⁴ kg/kg CO₂)

The final compression stage accounts for the majority of energy demand, owing to the high pressure ratio required to reach supercritical CO₂ conditions. The remaining 12% of CO₂ is recycled to the reformer furnace as fuel gas, keeping atmospheric emissions near zero.


**System Boundary**

This is a gate-to-gate analysis. The boundary starts at the natural gas inlet and ends at the compressed CO₂ product stream ready for transport.

Included:


Material and energy flows for CH₄ and H₂O inputs
CO₂ separation and multi-stage compression
Steel consumption of capture unit equipment
Electricity demand of compressors


Excluded:


Upstream natural gas extraction and pipeline transport
Plant construction and decommissioning
CO₂ transport, injection, and storage
End-use of co-produced hydrogen



**Tools & Methods**

ToolPurposeDWSIMProcess simulation (Peng-Robinson EOS)OpenLCALife cycle inventory modelling and impact assessmentISO 14040/14044LCA framework and methodology

The flowsheet mirrors Air Liquide's CRYOCAP™ H₂ technology (Port-Jérôme, France), which has been in commercial operation since 2015 at 100,000 t/yr CO₂ and >97% capture rate (TRL 9).


**Repository Structure**

├── report/
│   └── LCA_Sprint_3_Final.pdf       # Full course report
├── simulation/
│   └── SMR_CCS.dwsim                # DWSIM process flowsheet
├── lca/
│   └── openLCA_model/               # OpenLCA project files
└── README.md


**References**

Key references underpinning this work:


Spath & Mann (2001). Life Cycle Assessment of Hydrogen Production via Natural Gas Steam Reforming. NREL.
Dufour et al. (2009). Life cycle assessment of hydrogen production by steam reforming. Int. J. Hydrogen Energy, 34(3), 1370–1376.
IEAGHG (2017). Techno-economic evaluation of SMR-based hydrogen plant with CCS. Report 2017/02.
Antonini et al. (2020). Hydrogen production from natural gas with CCS — a techno-environmental analysis. Sustainable Energy & Fuels, 4(6), 2967–2986.
ISO 14040:2006. Environmental Management – Life Cycle Assessment – Principles and Framework.


Full reference list in report/LCA_Sprint_3_Final.pdf.


**Course**

Sustainability Assessment (LCA) — Faculty of System and Process Engineering, M.Sc. Chemical and Energy Engineering
Supervisor: Prof. Dr. Lissa Rikho-Struckmann · Otto-von-Guericke University Magdeburg

