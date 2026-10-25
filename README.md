<style>
  body, body * {
    font-family: "Times New Roman", Times, "Liberation Serif", serif !important;
  }
</style>

These are external animations for Alejandro Navarro's PhD Dissertation.

- [Telomere end-processing workflow](telomere_workflow.html)
- [Replication Initiation Workflow](replication-initiation.html)
- [Replication Initiation Chapter 5 Supplement](replication-initiation-tour.html)
- [Algorithmic End Fate Tree](algorithmic-end-fate.html)

---

These are the full data files for the dissertation's supplemental sections.

**Supplemental 3: Yeast Two-Hybrid**

- [Yeast Two-Hybrid Full Data](pdfs/Y2H_Raw_Data.pdf)

**Supplemental 4: QuantaColony Analytical Outputs**

- [Anbalagan Dataset](pdfs/Anbalagan_Overview_Selected.pdf)
- [Historical Dataset](pdfs/Historical_Overview_Selected.pdf)
- [Crowding Dataset](pdfs/Crowding_Overview_Selected.pdf)
- [Rescue Full](pdfs/Rescue_Overview_Full.pdf)
- [Rescue Selected](pdfs/Rescue_Overview_Selected.pdf)

---

These are the source code and data that produce the Supplemental 4 outputs.

**QuantaColony Source Code**

- [QuantaColony](QuantaColony.zip): open-source MATLAB application used for colony detection, measurement, and data organization

**Analytical Pipeline**

- [Analytical Pipeline](Analytical-Pipeline.zip): MATLAB code that builds the composite dataset from the QuantaColony project files and generates the Supplemental 4 PDFs. Unzip and run `run_all.m`. On the first run, the pipeline downloads Complete Analyses from the release below, checks each file against its SHA-256 checksum, and installs it. Requires MATLAB R2021b or later with the Statistics and Machine Learning Toolbox. Setup and run instructions are in the included README.
- [Complete Analyses](https://github.com/Anava13/Dissertation-External-features/releases/tag/complete-analyses): QuantaColony project files for the Crowding (P2), Rescue (P3), Anbalagan, and Historical datasets, one zip per dataset (2.2 GB total)
