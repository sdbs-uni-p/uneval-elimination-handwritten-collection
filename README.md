# Uneval Elimination: Handwritten Collection

## About

This repository supplements the paper **"Elimination of Annotation Dependencies in Validation for Modern JSON Schema"** by Lyes Attouche, Mohamed-Amine Baazizi, Dario Colazzo, Giorgio Ghelli, Stefan Klessinger, Carlo Sartiani, and Stefanie Scherzinger, under review.  

It contains the **Handwritten collection** of schemas in Modern JSON Schema, used in the experimental evaluation, including: 
- Original input schemas  
- Manually eliminated schemas  
- Eliminated schemas produced by our implementation  
- Instances used in manual witness testing  

## Collection Structure

All schemas and instances of the Handwritten collection are located in the [handwritten](handwritten) directory. The following naming conventions apply:  

- **`*.in.json`** – Original Modern JSON Schema schema containing `"unevaluatedProperties"` and/or `"unevaluatedItems"`  
- **`*.manual_elim.json`** – Schema eliminated through manual translation  
- **`*.out.json`** – Schema eliminated by our prototype, using the original schema as input  
- **`*.instyes.*.json`** – Instance valid for the original schema and, assuming elimination is correct, also valid for both eliminated schemas  
- **`*.instno.*.json`** – Instance invalid for the original schema and, assuming elimination is correct, also invalid for both eliminated schemas  

## License

The datasets in this repository are licensed under the Creative Commons Attribution 4.0 International (CC BY 4.0).