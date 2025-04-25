# Patterns in Words and Numbers: A Look at Zipf’s and Benford’s Laws

## Table of Contents

1. [What’s This Project About?](#whats-this-project-about)  
2. [Project Structure](#project-structure)  
3. [Main Goals](#main-goals)  
   3.1. [Zipf’s Law – Word Frequency](#1-zipfs-law--word-frequency)  
   3.2. [Benford’s Law – Leading Digits](#2-benfords-law--leading-digits)  
   3.3. [Bridging the Two Laws](#3-bridging-the-two-laws)  
   3.4. [Networks & Statistics](#4-networks--statistics)  
4. [How to Run](#how-to-run)  

---

## What’s This Project About?

This project explores two fascinating statistical patterns that appear across very different types of data: Zipf’s Law and Benford’s Law.

Zipf’s Law describes how word frequencies in language follow a predictable pattern: a small number of words are extremely common, while the majority occur very rarely. Benford’s Law, on the other hand, explains why in many real-world datasets, lower digits (like 1 or 2) appear more often as the first digit in numbers than higher digits.

We use real text and numeric datasets to study these two laws independently, explore potential relationships between them, and examine how they show up in networks and graph structures.

---

## **Project Structure**
```
├── data/               # Raw and processed datasets
│   ├── Text-1.txt     
│   ├── Text-2.txt      
├── notebooks/          # Jupyter notebooks for analysis
│   ├── zipf_analysis.ipynb  
│   ├── benford_analysis.ipynb  
├── README.md           
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

## **Results & Discussion**
This project demonstrates that **natural language and numerical datasets share universal statistical properties**. By understanding these laws, we can:
- Improve **linguistic data processing** (e.g., text compression, keyword ranking)
- Detect **fraud and anomalies** in financial reports (Benford’s Law applications)
- Analyze **networks and social graphs** for natural distribution patterns


---

## Main Goals

### 1. Zipf’s Law – Word Frequency

We start by analyzing a large block of English text, around one million characters long. After standardizing the text (uppercase conversion and punctuation removal), we split it into words and count how often each one appears. By plotting word frequency against word rank on a log-log scale, we can check whether the distribution follows the Zipfian curve.

### 2. Benford’s Law – Leading Digits

For this part, we extract the leading digit from each number in several real-world datasets. We then compare the frequency of these digits with the expected probabilities from Benford’s Law. A histogram visually illustrates how closely the dataset follows the predicted pattern.

### 3. Bridging the Two Laws

We compare the mathematical structure of both laws—Zipf’s logarithmic decline and Benford’s logarithmic distribution. We analyze whether word frequencies from natural language could exhibit Benford-like digit distributions, drawing connections between linguistic and numerical data.

### 4. Networks & Statistics

Using NetworkX, we generate synthetic graphs and analyze the distribution of node degrees (i.e., how many connections each node has). These degree distributions are compared to Benford’s distribution using statistical distance metrics like KL Divergence and Jensen-Shannon Divergence.

---

## How to Run

To explore the project, clone the repository and open the notebooks using Jupyter:

```bash
git clone https://github.com/matinfirooz/Zipf-s-Law-and-Benford-s-Law-in-Text-Processing.git
cd Zipf-s-Law-and-Benford-s-Law-in-Text-Processing
jupyter notebook
