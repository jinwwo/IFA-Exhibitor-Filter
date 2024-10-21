## IFA Exhibitor Filter

This repository contains a tool designed to filter and identify relevant companies participating in the IFA exhibition. 

## Overview

The code in this repository fetches a list of companies exhibiting at the IFA2024 and filters out companies that are most relevant to your business. It compares the similarity between the companies' information and the user's company profile, allowing you to focus on the most pertinent potential partners or competitors.

## Features

- **Company List Extraction**: Automatically retrieves a list of companies participating in the IFA exhibition.
- **Similarity Matching**: Compares the provided company information with each IFA exhibitor to determine relevance.
- **Filtering**: Outputs a refined list of companies that have high relevance to your business.

  (You can choose the number of companies to extract by setting the argument '**top_k**')

## Usage
```bash
python main.py --company_name "YOUR_COMPANY_NAME" --batch_size 32 --top_k 30
```

## Result Example
|company|brand_info|url|score|
|---|---|---|---|
|LG Electronics|we believe that a good life is about savoring all . . .|https://www.ifa-berlin.com/exhibitors/lg-electronics-inc|0.712|
|Homeguard / Raysharp|Raysharp is a  industry-leading group, leveraging their 20+ years of R&D . . .|https://www.ifa-berlin.com/exhibitors/intelligent-security-surveillance-limited|0.706|
|Parallel Space Co.,Ltd.|Parallel Space is IT startup specializing in the development of automated software programs . . .|https://www.ifa-berlin.com/exhibitors/pspace|0.695|
|inovaLab|At inovaLab, our mission is to revolutionize heat generation and material processing through innovative . . . |https://www.ifa-berlin.com/exhibitors/inovalab-srl|0.688|
