---
layout: post
title: What has been Done so Far ?
subtitle: "2 - Litterature review"
date: 2025-05-07
cover-img: /assets/img/cover_3.png
share-img: /assets/img/cover_3.png
tags: [Litterature, Academics]
comments: true
mathjax: true
author: Yajing HU
---

Facial-recognition technologies inherit and even magnify biases of the data on which they are trained. People of racial, gender, and age minorities are particularly susceptible to misrepresentation and discrimination due to such biases. Previous studies have extensively examined how facial recognition algorithms discriminate against minority groups and the implications of these biases. To better understand the scope and consequences of these biases within the transgender community, this section examines existing studies on facial-recognition systems’ gender and age bias, their implications in real-world applications, and the specific gaps in addressing the transgender population.

## Gender Bias
There are extensive studies investigating the gender biases of facial recognition algorithms. These studies consistently confirm that facial recognition algorithms exhibit bias against people of gender minorities. For instance, Klare et al. (2012) show that facial recognition algorithms consistently yield lower matching accuracies on the same demographic cohorts–those of females, Blacks, and the age group 18 to 30. In addition, by surveying existing benchmark databases used to train models for facial recognition and gender classification tasks, Wu et al. (2020) discovered that the current databases employ binary classifiers (male/female) to label gender data, thereby excluding gender minority subgroups from representation. This absence of gender representation significantly contributes to the accuracy disparities of gender recognition because the trained model relies exclusively on the majority sample to optimize accuracy rates, leaving gender minorities largely ignored. Furthermore, in the context of commercial facial analysis, Buolamwini et al. (2018) find that people of racial and gender minorities, especially darker-skinned females, are the most misdetected groups with error rates of up to 34%, whereas the maximum error rate for lighter-skinned males is less than 1%. 

More importantly, the gender bias of facial recognition algorithms can foster detrimental consequences for people of gender minorities, especially those who fall outside of the binary gender category, such as transgender people (Wu et al., 2020). Being misgendered can have negative impacts on one’s self-confidence and overall mental health (Keyes, 2018). Such bias can be more problematic in the context of healthcare: gender biases in the technical design choices from data collection and labeling to model training and development can contribute to systemic discrimination against transgender population (Parks, 2025). For example, biased diagnostic algorithms and insurance eligibility systems may lead to misdiagnosis, mistreatment, and unjust denials of care for transgender patients.

Furthermore, studies have demonstrated that inclusion of gender minority samples can drastically increase the accuracy of gender detection, which further emphasizes the fundamental limitations of the binary-coding of gender. By extending the current binary gender classifier to include a non-binary gender class, Wu et al. (2020) assembled two new facial image databases that are both racially and gender inclusive. The results yield an overall accuracy score of over 90%, which is a more than 38% improvement from the baseline binary gender classifier. Even more notably, once incorporating more gender non-binary subsets into the training data, facial recognition algorithms can provide a more accurate detection of sexual orientation than human brains can (Wang & Michal Kosinki, 2018). Collectively, their findings indicate the necessity of incorporating a more gender diverse dataset to train AI models. 

## Age Bias
Studies have shown that AI systems are even more susceptible to biases than humans when estimating age from facial images. For example, by comparing human and AI performance in age estimation, Ganel et al. (2022) find that AI is significantly less accurate in estimating the ages of older adults, smiling faces, and female faces. Moreover, Chu et al. (2023) point out that the dataset used to train AI models is often subject to a variety of biases, particularly the representation bias and omitted-variable bias. Specifically, they find that data sets tend to under-represent older or very young faces due to the lack of representation of older-adult images, which significantly diminishes the accuracy for estimating the age of elderly people. Additionally, algorithms are observed to directly remove the already scarce images of elderly people or omit confounding variables such as makeup and ethnicity, which further skew age estimates. Thus, it’s clear that the facial recognition algorithms present structural weaknesses in age estimation, which highlights the need to reexamine and refine the training data to be more inclusive and representative.

Age bias of facial recognition algorithms can be harmful in a variety of contexts. For example, in medical imaging applications, age bias can lead to underdiagnosis of older people (Seyyed-Kalantari et al., 2021). Moreover, studies have found that facial recognition models are perpetuating ageism (Chu et al., 2022). Since older populations face higher barriers to digital technologies, their values and interests are less visible compared to those of younger populations. As society transitions to an increased use of technology, the mismatch between the mainstream technological systems and the older populations would be further intensified, thereby reinforcing social inequity, exclusion, and marginalisation in various settings such as healthcare and information & communication. (Chu et al., 2022).

## Literature Gap
Although extensive research has been conducted to investigate the algorithmic bias in gender and age, very few studies have explored the intersection between them. Nevertheless, this intersectional perspective is critical in understanding how AI biases against the transgender community. Age and gender interact crucially in this community: studies have shown that trans adults on hormone therapy face an increased mortality risk caused by lung cancer, cardiovascular disease, HIV, and suicide (JM de Blok et al., 2021). In Brazil, life expectancy for transgender individuals is estimated at 35 years old, which is approximately half the national average (Senado Federal). As facial recognition algorithms systematically misjudge the gender and age of transgender people, transgender people would continue to face substantial barriers in various settings such as healthcare, education, and the workplace. Such barriers would thus reinforce the biased perception of them as unhealthy, short-lived, and uneducated, thereby exacerbating their socioeconomic inequalities.

However, most benchmark databases such as Adience provide only binary male-female classifiers and no reliable non-binary or trans identity labels. As of 2025, there is still a persisting absence of comprehensive data on gender identity, spanning from the number of individuals identifying as transgender to the many instances of gender-based violence that go unreported (Reia et al., 2025). Until scholars are able to collect data using inclusive and accurately labelled images, the compound bias in the algorithms would continue to loom large.


## References
Bortoni. (2017, June 20). Vida de transexuais no Brasil é marcada por preconceito e violência. Senado Federal. https://www12.senado.leg.br/noticias/especiais/especial-cidadania/vida-de-transexuais-no-brasil-e-marcada-por-preconceito-e-violencia

Buolamwini, J., & Gebru, T. (2018). Gender Shades: Intersectional Accuracy Disparities in Commercial Gender Classification. Proceedings of Machine Learning Research, 81, 1–15. https://proceedings.mlr.press/v81/buolamwini18a/buolamwini18a.pdf

Chu, C. H., Donato-Woodger, S., Khan, S. S., Nyrup, R., Leslie, K., Lyn, A., Shi, T., Bianchi, A., Rahimi, S. A., & Grenier, A. (2023). Age-related bias and artificial intelligence: a scoping review. Humanities and Social Sciences Communications, 10(1), 1–17. https://doi.org/10.1057/s41599-023-01999-y

Chu, C. H., Nyrup, R., Leslie, K., Shi, J., Bianchi, A., Lyn, A., McNicholl, M., Khan, S., Rahimi, S., & Grenier, A. (2022). Digital Ageism: Challenges and Opportunities in Artificial Intelligence for Older Adults. The Gerontologist, 62(7). https://doi.org/10.1093/geront/gnab167

de Blok, C. J., Wiepjes, C. M., van Velzen, D. M., Staphorsius, A. S., Nota, N. M., Gooren, L. J., Kreukels, B. P., & den Heijer, M. (2021). Mortality trends over five decades in adult transgender people receiving hormone treatment: a report from the Amsterdam cohort of gender dysphoria. The Lancet Diabetes & Endocrinology, 9(10), 663–670. https://doi.org/10.1016/s2213-8587(21)00185-6

Ganel, T., Sofer, C., & Goodale, M. A. (2022). Biases in human perception of facial age are present and more exaggerated in current AI technology. Scientific Reports, 12(1). https://doi.org/10.1038/s41598-022-27009-w

Keyes, O. (2018). The Misgendering Machines. Proceedings of the ACM on Human-Computer Interaction, 2(CSCW), 1–22. https://doi.org/10.1145/3274357

Klare, B. F., Burge, M. J., Klontz, J. C., Vorder Bruegge, R. W., & Jain, A. K. (2012). Face Recognition Performance: Role of Demographic Information. IEEE Transactions on Information Forensics and Security, 7(6), 1789–1801. https://doi.org/10.1109/tifs.2012.2214212

Parks, M. (2025). The ethics of AI at the intersection of transgender identity and neurodivergence. Discover Artificial Intelligence, 5(1). https://doi.org/10.1007/s44163-025-00257-1

Reia, J., Leach, R., & Li, S. (2025). Libra Open ; Trans digital rights: Improving data visibility, privacy. Virginia.edu. https://libraopen.lib.virginia.edu/public_view/g158bh51g

Seyyed-Kalantari, L., Zhang, H., McDermott, M. B. A., Chen, I. Y., & Ghassemi, M. (2021). Underdiagnosis bias of artificial intelligence algorithms applied to chest radiographs in under-served patient populations. Nature Medicine, 27(12), 2176–2182. https://doi.org/10.1038/s41591-021-01595-0

Wang, Y., & Kosinski, M. (2018). Deep neural networks are more accurate than humans at detecting sexual orientation from facial images. Journal of Personality and Social Psychology, 114(2), 246–257. https://doi.org/10.1037/pspa0000098

Wu, W., Protopapas, P., Yang, Z., & Michalatos, P. (2020). Gender Classification and Bias Mitigation in Facial Images. 12th ACM Conference on Web Science. https://doi.org/10.1145/3394231.3397900
