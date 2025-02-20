# Instructions for Setting Up OCR Repository and Text Extraction

## Overview
These instructions detail how to prompt Claude to create a repository for OCR text extraction and manage the extracted content effectively.

## Step-by-Step Instructions

### 1. Repository Creation
```
Create a new repository called "OCR-Tests"
```
This simple command will initiate the repository creation process.

### 2. Directory Structure Setup
```
Make a folder called "images" and another called "Extracted text" in the repository
```
This creates the basic structure needed for organizing our content.

### 3. Text Extraction and Storage
When providing an image to Claude, use this prompt structure:
```
Extract ALL text from this image. Include:
- Main headers and subheaders
- All body text
- Any figure labels and captions
- Diagram annotations and labels
- Special characters and symbols
- Mathematical notation
- Any footnotes or additional text
```

### 4. Verification and Completion
After initial extraction, use this prompt to ensure completeness:
```
Compare this with any previously extracted text and identify any missing elements. Create a comparison table showing what was missed.
```

### 5. Text File Updates
If any content was missed:
```
Replace the original extracted text document with the new FULLY extracted text, ensuring all previously missed content is now included.
```

## Best Practices
1. Always request ALL text - Claude can sometimes focus on main body text and miss annotations or labels
2. Ask for a comparison when updating existing extractions
3. Maintain clear file organization with images and extracted text in separate folders
4. Use markdown formatting for the extracted text files to maintain readability
5. Keep track of each image and its corresponding text file with matching names

## Repository Structure
```
OCR-Tests/
├── images/
│   └── .gitkeep
├── Extracted text/
│   └── cell_structure_text.txt
└── Instructions/
    └── ocr_repository_setup.md
```