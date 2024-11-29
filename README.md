# vendor_invoice_desc_grouper
vendor_invoice_desc_grouper is a Python-based utility designed to group similar vendor invoice descriptions using the StringGrouper library. It helps consolidate variations in descriptions (e.g., typos, different word orders) to improve invoice processing, reporting, or deduplication workflows.

# Key Features
Fuzzy Matching: Groups similar descriptions based on similarity scores.
Efficient: Uses vectorized operations to handle large datasets.
Customizable Thresholds: Allows setting similarity thresholds to tune grouping sensitivity.
Scalable: Works efficiently with thousands of invoice descriptions.

# How It Works
Input: A list or dataframe column containing vendor invoice descriptions.
Similarity Calculation: StringGrouper computes pairwise similarities between all descriptions.
Grouping: Descriptions with a similarity score above the defined threshold are assigned to the same group.
Output: Returns a mapping of each description to its group or canonical form.

# Installation
To use vendor_invoice_desc_grouper, first install the required dependencies:
pip install string-grouper pandas

# Customization Options
min_similarity: Adjust the similarity threshold to control grouping sensitivity.
Preprocessing: Use custom cleaning (e.g., lowercasing, removing special characters) before grouping.

# Contributing
Contributions are welcome! If you find bugs or have suggestions for improvements, please create an issue or submit a pull request.
