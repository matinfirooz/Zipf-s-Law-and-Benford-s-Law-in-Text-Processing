# **Analyzing Patterns in Language and Numbers: A Unified Study of Zipf’s Law and Benford’s Law**

## **Overview**
This project explores two fundamental statistical laws:
- **Zipf’s Law** (word frequency distribution in natural language)
- **Benford’s Law** (distribution of leading digits in numerical datasets)

By analyzing text and numeric data together, we uncover hidden patterns in real-world datasets and establish a connection between linguistic and numerical distributions.

## **Project Structure**
```
├── data/               # Raw and processed datasets
├── notebooks/          # Jupyter notebooks for analysis
├── scripts/            # Python scripts for data preprocessing & analysis
├── results/            # Output graphs and statistical results
├── README.md           # Project documentation
└── requirements.txt    # Dependencies
```

## **Tasks and Objectives**
### **1. Zipf’s Law: Text Analysis**
- Process an English text (~1 million characters, ~160,000 words)
- Convert text to uppercase & remove punctuation
- Extract words and compute their frequency
- Plot a **log-log graph** of word rank vs. frequency
- Analyze if the dataset follows **Zipf’s Law**

### **2. Benford’s Law: Numeric Data Analysis**
- Extract leading digits from numerical datasets
- Compute expected probabilities based on **Benford’s Law**
- Plot a **histogram of leading digits** vs. expected distribution
- Test real-world datasets for compliance with Benford’s Law

### **3. Bridging Zipf’s & Benford’s Laws**
- Compare the mathematical properties of both laws
- Check if word-rank frequency exhibits Benford-like behavior
- Analyze their occurrence in different real-world datasets

### **4. Network Analysis & Statistical Comparison**
- Generate random networks using **NetworkX**
- Analyze degree distributions of nodes
- Compare degree distributions with **Benford’s Law**
- Use **KL Divergence** and **Jensen-Shannon Divergence** for statistical validation

## **Installation & Usage**
### **Requirements**
Ensure you have Python installed. Then, install the dependencies:
```bash
pip install -r requirements.txt
```

### **Running the Analysis**
To execute the Zipf’s Law analysis:
```bash
python scripts/zipf_analysis.py
```
To execute the Benford’s Law analysis:
```bash
python scripts/benford_analysis.py
```
To compare both laws and analyze network distributions:
```bash
python scripts/unified_analysis.py
```

## **Results & Discussion**
This project demonstrates that **natural language and numerical datasets share universal statistical properties**. By understanding these laws, we can:
- Improve **linguistic data processing** (e.g., text compression, keyword ranking)
- Detect **fraud and anomalies** in financial reports (Benford’s Law applications)
- Analyze **networks and social graphs** for natural distribution patterns

## **Contributing**
Contributions are welcome! Feel free to fork this repository, make improvements, and submit a pull request.

## **Acknowledgments**
Special thanks to the mathematical and data science community for inspiring this project!
