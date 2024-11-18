# Cracking The DNA Protein Binding Code
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white)  
![JavaFX](https://img.shields.io/badge/JavaFX-GUI-blue?style=for-the-badge)  
![License](https://img.shields.io/badge/License-Academic-red?style=for-the-badge)  
![Research Project](https://img.shields.io/badge/Research_Project-Braude_College_of_Engineering-blue?style=for-the-badge)


This project proposes an algorithm to analyze DNA-binding proteins (DBPs) and locate their target sites within the genome. It hypothesizes that certain nucleotide sequences in DNA act as "pointers" to guide the binding process. The tool utilizes a sliding window approach to identify potential "pointer" sequences.

---

## 🧬 Features

- **Graphical User Interface (GUI)**:
  - Built with **JavaFX**, the GUI allows users to interact with the tool easily, select input files, and choose the algorithm for analysis.
- **Biological Analysis**:
  - Detects patterns and frequencies in DNA sequences, comparing biological data with shuffled data to uncover biological signals.

---

## ⚙️ Algorithms Details

### Algorithms Overview
This project includes several algorithms designed to identify potential DNA-binding site pointers by analyzing the distribution and occurrence of nucleotide sequences. Below is a brief description of each algorithm:

1. **Segmented DNA Analysis**: This algorithm divides the DNA sequence into smaller segments around the binding site. It focuses on the segment before the binding site (1/32 segment) and uses a sliding window approach to find words that appear more frequently in this segment. Words with less frequent reverse complements are considered potential pointers.

2. **Word Occurrences DNA Analysis**: This algorithm extracts words from both the upstream and downstream regions of the binding site and compares their frequencies. It identifies words that are more frequent in the downstream region (forward direction) and less frequent in the upstream region (reverse complement), which may point to potential binding sites.

3. **Segmented Word Distribution Analysis**: The DNA sequence is divided into segments, and a sliding window is used to identify unique word sequences. The algorithm checks if the frequency distribution forms an ascending pattern before the binding site and a descending pattern afterward, identifying potential pointers based on this distribution.

4. **Potential PWM Pointers**: This algorithm uses a Position Frequency Matrix (PFM) to construct a Position Weight Matrix (PWM) for the DNA sequence. It then calculates the score for each window using the PWM and identifies potential pointers if the score is close to the maximum and if occurrences are greater downstream than upstream.

---

## 🛠️ Dependencies

The tool is built using **Java** for the GUI (**JavaFX**) and the core algorithm. The following biological databases were used:

- **JASPAR CORE Database**: Contains transcription factor binding sites.
- **NCBI GRCh38.p14 Primary Assembly Dataset**: A reference genome dataset used for analysis.

### Preprocessing:
- DNA sequence files and binding site data files should be preprocessed. (Note: preprocessing is done outside of this repository using C++ and Python, and is **not** included here.)

### Libraries/Frameworks:
- **JavaFX**: For GUI development.
- **Custom Algorithms**: Implemented in Java.

---

## 📝 Installation Instructions

Follow these steps to set up and run the tool on your machine:

1. **Install Java Development Kit (JDK)**:  
   Ensure you have **JDK 8 or later** installed.  
   You can download JDK from [Oracle JDK](https://www.oracle.com/java/technologies/javase-downloads.html).

2. **Clone the Repository**:
   ```bash
   git clone https://github.com/MohamedAboSaleh/Cracking-The-DNA-Protein-Binding-Code.git
   
3. **Compile and Run:**
- Navigate to the project folder.
- Compile the project using your IDE or the terminal.
- Run the Java application.

4. **File Selection:**

- When the GUI opens, you will be prompted to select the following input files:
  - DNA Binding Sites File: Contains the DNA-binding protein sites.
  - DNA Sequence File: Contains the DNA sequence to be analyzed.
- After selecting the input files, choose the algorithm from the GUI and start the analysis.

---
## 📊 Data Requirements
The tool requires DNA sequence data and binding site information in specific formats:

1. **NCBI Data:**
   - Obtain the GRCh38 dataset from [NCBI](https://www.ncbi.nlm.nih.gov).
2. **JASPAR CORE Database:**
   - Access transcription factor binding sites from the [JASPAR Database](https://jaspar.elixir.no).
   
Make sure the files are formatted as per the dataset specifications.

---

## 🚀 Running the Tool
1. **Launch the Application.**
2. **Select Input Files:**
   - Choose the DNA Binding Sites File and the DNA Sequence File.
3. **Choose the Algorithm from the GUI.**
4. **View Results:**
   - The results will display the biological signals detected in the sequence, as outlined in the included research paper.
   
---
##  Testing & Results
The algorithm was tested on shorter DNA sequences where the frequency of each segment was already known. The results show significant signals in biological sequences compared to shuffled data, highlighting potential "pointer" sequences for DNA-binding proteins.

For more details, refer to the findings discussed in the included paper.

---

## 🤝Contributions
This project was a **team effort**. Each contributor worked on different parts of the system, including:

- Algorithm development.
- Database construction.
- GUI implementation.

---

## 🚧 Future Work
Currently, there are no planned improvements or additional features for the tool. Future research may involve further investigation of the biological signals detected.

---
## 📄 Acknowledgements

This project was developed as part of the **Final Year Research Project** at **Braude College of Engineering**. It reflects the culmination of my academic work during the final year and demonstrates my skills in bioinformatics, algorithm development, and GUI design.
