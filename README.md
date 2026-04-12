# Urban Infrastructure Issues Dataset (AI + GIS)

A structured geospatial dataset of public infrastructure and utility issues, generated through an AI-assisted reporting pipeline.

---

## Overview

This dataset contains geolocated records of infrastructure and utility issues identified through a combination of:

- image-based AI classification  
- user validation  
- geospatial processing  

Each record represents a real-world issue detected in public space and converted into structured GIS-ready data.

This repository provides a **sample and overview of the dataset**, not the full data.

---
## 🔗 Live Demo

This project includes a fully functional demo application and a live GIS visualization of the generated dataset.

You can explore and test the system through the following links:

- **Web Application (AI Reporting Tool):**  
  [Open App](https://ai-gis-reporting.vercel.app/)


The web application allows users to submit and validate infrastructure issues using AI-assisted classification, while the interactive map displays the resulting geospatial dataset.

---

## What this dataset represents

The dataset captures typical urban infrastructure issues such as:

- potholes  
- garbage accumulation  
- graffiti  
- damaged signs  
- broken public lighting  
- water leaks  
- sidewalk damage  
- fallen trees  

All records are:

- geo-referenced  
- time-stamped  
- categorized into controlled issue types  

---

## Data structure (sample)

Each entry includes:

- `issue_type` – classified category  
- `description` – AI-generated summary  
- `latitude` – geographic coordinate  
- `longitude` – geographic coordinate  
- `gps_accuracy` – estimated location precision (meters)  
- `reported_at` – timestamp  

---

## Methodology

Data is generated through a structured pipeline:

1. User captures an image of a public infrastructure issue  
2. AI analyzes the image and proposes classification  
3. User can optionally provide clarification  
4. AI refines or confirms the result  
5. Only visually verifiable public issues are retained  
6. The final record is stored as a geospatial feature and published on a map  

This approach ensures consistency and reduces noise in the dataset.

---

## Data quality and constraints

- Classification is based strictly on visible evidence  
- Indoor and private context is excluded  
- Controlled taxonomy is used for consistency  
- Edge cases may still require manual validation  

This dataset is designed for **practical usability**, not theoretical completeness.

---

## Use cases

This dataset can be used for:

- smart city analytics  
- infrastructure monitoring  
- GIS visualization  
- predictive maintenance models  
- urban planning  
- machine learning training datasets  

---

## Access & Collaboration

The full dataset is not publicly available.

Access can be provided upon request for:

- research  
- commercial use  
- integration into existing systems  

If you are interested in accessing the dataset or exploring collaboration opportunities, feel free to get in touch.

---

## Notes

This repository is intended to showcase the dataset structure and methodology.

The full dataset includes additional records and may be continuously updated.
