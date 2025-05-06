---
layout: post
title: How did we lead this study ?
subtitle: "3 - Methodology"
date: 2025-05-07
cover-img: /assets/img/cover_1.jpg
share-img: /assets/img/cover_1.jpg
tags: [methodology]
comments: true
mathjax: true
author: Julien VITRY
---

To conduct this study, we employed a facial recognition algorithm based on CaffeModel, part of the Caffe 1.0 framework. Although now somewhat deprecated, this model remains useful due to its efficiency, ease of use, and accessibility for beginners. It accurately detects faces and estimates both age and gender, making it suitable for our research objective: analyzing how facial recognition algorithms categorize transgender individuals. All AI-generated results were manually annotated to evaluate the model's performance and identify biases in the misgendering of cisgender and transgender individuals.

## Sample Collection
The facial recognition system was applied to a total of 207 individuals: 102 transgender and 105 cisgender. These images were randomly generated using a generative AI model to reduce researcher bias and promote objectivity. However, the AI generation process introduced notable biases. The transgender sample is disproportionately composed of women, approximately 80%, whereas the cisgender sample is balanced, with an equal number of men and women.
This overrepresentation of trans women may reflect broader trends, as male-to-female (MtF) transitions are generally more common and more medically accessible than female-to-male (FtM) ones (Van Caenemgen et al, 2015). Nevertheless, it is important to acknowledge that the inverted tendency is currently happening and there is an increasing amount of operations now for FtM transitions (Aitken et al, 2015). Additionally, all transgender individuals in the dataset have completed their transition, excluding those who are non-binary or in the process of transitioning. While this limits the spectrum of trans identities covered, it allows the study to focus on individuals with stabilized gender expressions, potentially improving the algorithm's classification consistency.
It is important to note that the sample skews heavily toward white individuals, with people of color underrepresented. This narrow demographic range may obscure intersectional biases, but it also isolates the impact of transgender identity on algorithmic behavior. To comply with data protection regulations, all images used are of publicly known transgender celebrities, ensuring the data is legally available and not subject to GDPR restrictions concerning private sensitive data. Each subject’s gender (binary: male/female) and exact age are recorded in an Excel spreadsheet for comparison with the AI’s predictions.

## Facial Recognition Implementation
We used a Python script provided in Jean-Philippe Cointet’s Decoding Biases in AI course, modified for our needs to process multiple images efficiently. An additional feature was added to reduce binary classification bias: if the confidence score of the AI dropped below 0.7, the output was marked as “Uncertain.” This mitigates the risk of forced gender classification when a profile does not align with binary gender norms.
AI-generated results—including estimated gender and age—were logged in two separate Excel files (one for cisgender individuals, one for transgender individuals). Since the algorithm predicts age ranges rather than exact values, we retained the value closest to the actual age to assess match accuracy fairly.

![Sample]({{ '/assets/img/pic_sample.png' | relative_url }})
An example of Facial Recognition Application.

## Data Analysis
We began our analysis by cleaning and standardizing the dataset to align variable names, enabling easy merging of the two datasets when necessary. Rows where the algorithm failed to detect a face were removed (these were identifiable by an age value of 0).

| Personnality | Picture_Found | Male | Female | Non-Binary | Age | Male AI | Female_AI | Uncertain_AI | Age_AI | 
| :------ |:------- | :---------- |:------ |:--- | :--- | :------ |:--- | :--- | :------ |
| Name | 0 - 1 | 0 - 1 | 0 - 1 | 0 - 1 | xx | 0 - 1 | 0 - 1 | 0 - 1 | xx |
Table of Analysis

The resulting dataset includes six binary columns indicating both actual and AI-predicted gender identities (male, female, non-binary), alongside exact and predicted ages.
The data were analyzed in three stages:
- General Gender Mismatch: We examined mismatches between actual and AI-detected gender across the entire dataset.
- Cis/Trans Comparison: We compared classification disparities between cisgender and transgender groups.
- Age Analysis: Using boxplots, we visualized the difference between actual and predicted ages, highlighting distributions, minima, and maxima across groups.
Finally, we synthesized the gender and age results to calculate general matching rates, offering a comprehensive view of the disparities in AI performance across groups.

## References 
Van Caenegem E, Wierckx K, Elaut E, Buysse A, Dewaele A, Van Nieuwerburgh F, De Cuypere G, T'Sjoen G. Prevalence of Gender Nonconformity in Flanders, Belgium. Arch Sex Behav. 2015 Jul;44(5):1281-7. doi: 10.1007/s10508-014-0452-6. Epub 2015 Jan 15. PMID: 25588709.

Aitken M, Steensma TD, Blanchard R, VanderLaan DP, Wood H, Fuentes A, Spegg C, Wasserman L, Ames M, Fitzsimmons CL, Leef JH, Lishak V, Reim E, Takagi A, Vinik J, Wreford J, Cohen-Kettenis PT, de Vries AL, Kreukels BP, Zucker KJ. Evidence for an altered sex ratio in clinic-referred adolescents with gender dysphoria. J Sex Med. 2015 Mar;12(3):756-63. doi: 10.1111/jsm.12817. Epub 2015 Jan 22. PMID: 25612159.



