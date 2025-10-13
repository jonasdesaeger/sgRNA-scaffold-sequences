# sgRNA-scaffold-sequences
sgRNA scaffold variants and modifications for SpCas9/CRISPR

This repository provides a curated collection of **sgRNA scaffold variants** and **other RNA modifications** (aptamers, multiplexing sequences, etc.) compiled from published literature. It serves as a clean, standardized dataset for **research, plasmid annotation, and computational workflows**.

The dataset is based on supplementary material from published studies and builds on work described in:

**De Saeger, J.**  
*A Guide to Guides: an overview of SpCas9 sgRNA scaffold variants and modifications*  
(under review, 2025)  

---

## 📂 Repository Contents

- **sgRNA_dataset.xlsx**  
  Combined Excel file with two tabs:  
  - **Scaffolds** (S8)  
  - **Other_mods** (S9)  
Recommended for human browsing; preserves the layout and context of the original supplementary tables.
- **sgRNA_scaffolds.csv**  
  Machine-friendly table of scaffold variants.

- **sgRNA_other_mods.csv**  
  Machine-friendly table of RNA modifications.

- **sgRNA_scaffolds.fasta**  
  FASTA-formatted scaffold sequences.
  
- **sgRNA_other_mods.fasta**  
  FASTA-formatted sequences of aptamers/other modifications.

---

## 🔬 Usage

- **Plasmid annotation**  
  Import the FASTA files as features into your plasmid editor. Each scaffold or aptamer will be automatically detected in plasmid backbones.

- **Bioinformatics**  
  Use the FASTA files for BLAST searches, alignments, or sequence scans.

- **Data analysis**  
  Use the CSV files for structured analyses.

---

## 📊 Example FASTA Entries

From **sgRNA_scaffolds.fasta**:
```text
>Flip + Extension (F+E) sgRNA | DOI:10.1016/j.cell.2013.12.001 2013
GTTTAAGAGCTATGCTGGAAACAGCATAGCAAGTTTAAATAAGGCTAGTCCGTTATCAACTTGAAAAAGTGGCACCGAGTCGGTGC
```

---

## 📚 Citation

If you use this dataset, please cite both:
- The **original references** (DOIs included in each file).  
- The overview article:  
  *De Saeger, J. et al. “A Guide to Guides: an overview of SpCas9 sgRNA scaffold variants and modifications” (under review, 2025).*

---

## 🤝 Contributing

Contributions are welcome!

If you’d like to add new scaffolds or modifications:

1. **Edit CSV files** — add a row with:  
   - Name  
   - Synonyms  
   - Explanation  
   - DOI (reference)  
   - Year  
   - Sequence  
   - Length  

2. **Edit FASTA files** — add an entry in the format:  
Name | DOI:DOI_NUMBER YEAR
SEQUENCE

```
>T-Lock sgRNA | DOI:10.1016/j.cell.2017.05.050 2017
GTTTCAGAGCTATGCTGGAAACAGCATAGCAAGTTAAATAAGGCTAGTCCGTTATCAACTTGAAAAAGTGGCACCGAGTCGGTGC
```

3. **Submit a Pull Request (PR)**  
- Fork this repository  
- Commit your changes  
- Open a PR with a clear description (e.g., `"Add T-Lock sgRNA scaffold"`)  

🔒 Nothing is merged until reviewed and approved.

---

## 📜 License

[MIT License](LICENSE) — free to use and adapt with attribution.
