# RNAseq-DEG-DESeq2
Differential Gene Expression using DESeq2 in R
# 🧬 RNA-seq Differential Expression Analysis with DESeq2

This repository contains a complete pipeline for RNA-seq **Differential Gene Expression (DGE)** analysis using **DESeq2** in R. The example is structured to compare multiple tissue types or treatments and includes code for data normalization, visualization, and downstream GO enrichment.

---

## 📁 Project Structure


---

## 📚 Tools Used

- **R (v4.x)**  
- **DESeq2**, **tximport**, **clusterProfiler**  
- **ggplot2**, **pheatmap**, **EnhancedVolcano**

---

## 🔬 Workflow Summary

1. **Input Data**
   - `counts_matrix.csv`: raw gene counts matrix
   - `sample_metadata.csv`: sample info (condition, replicate, tissue)

2. **Pipeline Steps**
   - Import counts & metadata
   - Create `DESeqDataSet` object
   - Normalization & transformation (VST or rlog)
   - Differential expression analysis
   - Volcano & PCA plots
   - Export significant DEGs
   - (Optional) Functional enrichment analysis (GO/KEGG)

---

## 📈 Example Visuals

| PCA Plot | Volcano Plot |
|----------|--------------|
| ![PCA](plots/PCA_plot.png) | ![Volcano](plots/Volcano_plot.png) |

---

## 📦 Installation

```r
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

BiocManager::install(c("DESeq2", "tximport", "clusterProfiler", "pheatmap", "EnhancedVolcano"))

---

### ✅ Next Steps:

1. Create a new repo: `RNAseq-DEG-DESeq2`
2. Add folders: `data`, `scripts`, `plots`, `results`
3. Upload the `README.md` content above
4. Ask me anytime to help you write the R script `DESeq2_pipeline.R`!

Would you like me to now generate the `.R` script template as well for this pipeline?
