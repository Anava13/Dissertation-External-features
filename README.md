<style>
  body, body * {
    font-family: "Times New Roman", Times, "Liberation Serif", serif !important;
  }
</style>

These are external resources for Alejandro Navarro's PhD Dissertation.

---

**Interactive Process Models**

Each model runs in any modern browser with no installation.

- [Telomere end-processing workflow](telomere_workflow.html)
- [Replication Initiation Workflow](replication-initiation.html)

---

**Supplemental 3: Yeast Two-Hybrid**

- [Yeast Two-Hybrid Full Data](pdfs/Y2H_Raw_Data.pdf): the complete yeast two-hybrid dataset as a single PDF.

---

**Supplemental 1: Colony Size Modeling**

- [Colony Model](colony-model.html): branching-process model of colony growth that runs in the browser. The user builds a p(success) trajectory from flat segments, ramps, and branch events, sets ε for each segment, and simulates the colony set. Segments and branch points can be dragged on the trajectory plot. The app shows the predicted colony size histogram, KDE, mixture fit, and lineage composition beside a flat control. A Presets panel loads the condition behind every Supplemental 1 figure and table, labeled by figure. A grid preset runs the full parameter sweep and lays out every colony set on an overview map, where selecting a set fits its mixture and shows its plots. Results download as CSV and JSON.

---

**QuantaColony Analytical Outputs**

- [QuantaColony Dataset Reports](https://github.com/Anava13/Dissertation-External-features/releases/tag/complete-analyses): one PDF report per colony dataset, written by QuantaColony from the dissertation projects with a single export command.
  - **Crowding_Overview_Selected.pdf**: the plating-density experiment, one plate per dilution.
  - **Rescue_Overview_Selected.pdf**: the plate selected for each genotype and passage of the rescue experiment.
  - **Rescue_Overview_Full.pdf**: every plate of the rescue experiment, with each genotype and passage on its own pages.
  - **Anbalagan_Overview_Selected.pdf**: every plate of Figures 2C and 8D of Anbalagan et al. (2011), figure by figure.
  - **Historical_Overview_Selected.pdf**: every plate of the published *est* senescence series.

Each report opens with the measurement fidelity of its colonies. A grid of plates by genotype and passage follows, drawn five times: the original photographs, the photographs with every detected colony outlined, density histograms, kernel density estimates with the peak and mean marked, and LogNormal mixture fits with each component drawn. Every cell lists the plate's colony count, Capture Ratio, median radius, and interquartile range. Box plots of colony radius close the grid, with the colony count and median of each plate above its box. The Anbalagan report ends with the lineage panels, and both Rescue reports end with the mixture summaries, the within-state predictors, the selected-plate box plots, and the *dbf4-1* signature.

---

**QuantaColony**

- [QuantaColony (Python)](https://github.com/Anava13/Dissertation-External-features/releases/tag/QuantaColony-Python): open-source application that crops plate photographs, detects and measures colonies, records every correction made in review, and runs the statistical analyses behind every colony figure in the dissertation. Requires Python 3.10 or later. On Windows, the included installer sets up the program and its shortcuts; on other systems it installs as a standard Python package. Setup and run instructions are in the included README.

The four colony datasets of the dissertation ship inside QuantaColony as project files, and the program places them in a folder on its home page at first start. Each project holds the original plate photographs, the cropped plate sections, every detected and hand-added colony, and the edit log of the review.

- **Crowding Dataset**: the plating-density experiment, which relates colony size to the number of colonies sharing a plate.
- **Rescue Dataset**: the experiment testing whether *dbf4-1* rescues *cdc13-2* senescence, covering four genotypes across five passages with plating density and biological replicates as additional variables.
- **Anbalagan Dataset**: every colony in Figures 2C and 8D of Anbalagan et al. (2011), one plate per streak, with four genotypes per source plate.
- **Historical Dataset**: the published senescence plates for *est4-1* (Lendvay et al., 1996) and *est1-1* (Lundblad and Szostak, 1989), each lineage streaked through its passages on a single plate.

Every colony figure and every quoted colony value in the dissertation can be regenerated from these projects inside QuantaColony. Guided tours lead through each figure: one introduces the program on the Crowding Dataset, and four reproduce the figures of the crowding, rescue, published-plate, and historical analyses. Each step names every setting the figure uses, applies it on request, and explains why each setting matters for the experiment. A single export command writes every data figure as a vector PDF at its printed size, with one table per part of the dissertation listing each quoted value next to the value the current analysis computes. A second export command writes the five dataset reports listed under QuantaColony Analytical Outputs.
