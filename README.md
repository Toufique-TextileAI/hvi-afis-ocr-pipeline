# hvi-afis-ocr-pipeline
An automated Python OCR pipeline for extracting, parsing, and consolidating High Volume Instrument (HVI) and Advanced Fiber Information System (AFIS) parameters from unstructured PDF cotton test reports into machine-readable datasets.
Overview
The hvi-afis-ocr-pipeline is a custom data digitization tool designed to bridge the gap between physical textile quality reports and structured data science environments. In the cotton industry, macroscopic bundle data (HVI) and microscopic single-fiber distributions (AFIS) are frequently locked in unstructured PDF formats or printed laboratory reports. This repository provides a reproducible Python workflow (Jupyter Notebook) to extract text from PDF files using Python libraries. It then parses the unstructured strings and consolidates the paired physicochemical data under unified Bale and Lot identifiers.

## Key Features

**Automated OCR Extraction:** Converts rasterized PDF report pages into raw text strings utilizing Tesseract OCR wrappers.

**Rule-Based Pattern Matching:** Employs Python's regular expressions (re library) to create pattern searches that locate semantic anchors within unstructured documents, allowing for the precise extraction of key information.

**Data Synchronization:** Automatically aligns standard HVI commercial metrics (e.g., Micronaire, Strength, UHML) with granular AFIS process indicators (e.g., Neps per gram, Short Fiber Content) based on shared sample IDs.

**Ready for Machine Learning:** Cleans common OCR artifacts and exports the final, consolidated dataset as a structured CSV, optimized for downstream statistical analysis and the training of predictive models (e.g., "Virtual AFIS" algorithms).
