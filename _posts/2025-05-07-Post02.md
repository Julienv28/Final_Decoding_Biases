---
layout: post
title: Commenting our results
subtitle: "5 - Discussion"
date: 2025-05-07
cover-img: /assets/img/cover_2.jpg
share-img: /assets/img/cover_2.jpg
tags: [Discussion, Critical_Thinking]
comments: true
mathjax: true
author: Kai MÜTSCHELE
---

## Technical Perspective

Our analysis reveals substantial limitations in the investigated facial recognition model’s ability to accurately predict both gender and age - particularly for transgender individuals. From a technical standpoint, this outcome underscores fundamental issues in the model’s training data and design. Caffe-based systems like the one used in this project were among the earliest deep learning frameworks for image recognition. While efficient for image classification tasks, they were developed with static architectures that limit flexibility and adaptability in diverse contexts (İşbilen, 2022, p. 2; Jain, 2024, pp. 2–3).
We hypothesise that this is likely due to the fact that these early models often relied on constrained datasets that predominantly featured white, cisgender, male, and young faces, which limited their generalizability. As noted in Jain (2024), Caffe’s popularity in academic and early industrial contexts was based more on its speed than on its inclusivity or adaptability (p. 2). This stands in contrast to more recent frameworks such as TensorFlow and PyTorch, which support dynamic computation graphs and have enabled improvements in training on demographically diverse datasets (Grother, Ngan, & Hanaoka, 2019, pp. 2–3; Raji & Buolamwini, 2019, p. 432).

## Societal Perspective

Beyond technical shortcomings, our results raise pressing concerns about the societal impact of facial recognition technology. By systematically misgendering transgender individuals and forcing all subjects into a rigid male/female binary, the algorithm reinforces outdated gender norms and marginalizes those who do not conform to them. This phenomenon is well-documented in the academic debate: Keyes (2018) shows that most gender classification systems conceptualize gender as a binary attribute determined visually and, in doing so, excluding non-binary and transitioning identities (pp. 6–9). The consequences of this are not only epistemic but material: One could even argue that transgender individuals face systematic algorithmic erasure and misrecognition, which can affect their safety and social legitimacy (Keyes, 2018, pp. 12–13).
This technological rigidity reflects developers’ assumptions about “normal” appearances and identities, often shaped by white, cisgender, Western norms (Buolamwini & Gebru, 2018, p. 2). Crucially, these assumptions, when encoded in algorithms, reinforce broader structural inequalities. As Hamidi, Scheuerman, and Branham (2018) emphasize, gender recognition systems can act as tools of surveillance and discipline, particularly for trans users who already experience social marginalization (pp. 3–5). If deployed in settings such as hiring, policing, or public service delivery, such misclassification can result in exclusion, loss of income, or even discriminatory targeting. This is not a theoretical discussion as we have already seen such consequences in real-world cases that involve ride-share driver verification failures (Melendez, 2018) and police misidentification (Garvie, Bedoya, & Frankle, 2016, pp. 22–25).

## Limitations

While our study reveals these meaningful patterns, it is important to acknowledge its own limitations. The composition of our sample introduces potential biases that may have shaped the results of our study: In particular, the transgender group of our sample is disproportionately composed of trans women (approximately 80%), limiting the comparative analysis of misgendering across the full range of trans identities. Additionally, almost all transgender individuals included in the dataset had completed their medical transitions. While this provided more consistent gender presentation for algorithmic analysis, it excluded individuals that are in the process of transitioning and non-binary subjects. This reduces the representativeness of our dataset as it is not fully reflecting the entire spectrum of trans identities.
Another critical limitation is the dataset’s racial homogeneity: Most images - both cis and trans - depict white individuals. In a way, this omission reflects the broader trends in available image-generation tools and open datasets, which often underrepresent people of color. As Buolamwini and Gebru (2018) demonstrate, commercial classifiers misgender dark-skinned women at a rate of 34.7%, compared to 0.8% for light-skinned men (p. 7). Similarly, the NIST Face Recognition Vendor Test found that false positive rates were up to 100 times higher for individuals from African and East Asian populations than for white individuals in one-to-many matching scenarios (Grother, Ngan, & Hanaoka, 2019, p. 2). Such disparities underline the importance of intersectional analyses, which our dataset was not able to fully support. We therefore caution against generalizing our findings beyond our narrowly defined sample.

## References

Buolamwini, J., & Gebru, T. (2018). Gender shades: Intersectional accuracy disparities in commercial gender classification. Proceedings of Machine Learning Research, 81, 1–15. https://proceedings.mlr.press/v81/buolamwini18a/buolamwini18a.pdf

Garvie, C., Bedoya, A., & Frankle, J. (2016). The perpetual line-up: Unregulated police face recognition in America. Georgetown Law Center on Privacy & Technology. https://www.perpetuallineup.org/

Grother, P., Ngan, M., & Hanaoka, K. (2019). Face recognition vendor test (FRVT) part 3: Demographic effects(NISTIR 8280). National Institute of Standards and Technology. https://doi.org/10.6028/NIST.IR.8280

Hamidi, F., Scheuerman, M. K., & Branham, S. M. (2018). Gender recognition or gender reductionism? The social implications of automatic gender recognition systems. In Proceedings of the 2018 CHI Conference on Human Factors in Computing Systems (Paper 8). ACM. https://doi.org/10.1145/3173574.3173582

İşbilen, E. (2022). What is Caffe? Built In. https://builtin.com/machine-learning/caffe

Jain, A. (2024). Caffe, ONNX, TensorFlow and PyTorch frameworks. Medium. https://medium.com/@abhishekjainindore24/caffe-onnx-tensorflow-and-pytorch-frameworks-5c01c7045644

Keyes, O. (2018). The misgendering machines: Trans/HCI implications of automatic gender recognition. Proceedings of the ACM on Human-Computer Interaction, 2(CSCW), Article 88. https://doi.org/10.1145/3274357

Melendez, S. (2018, August 9). Uber’s face recognition tool has locked out some transgender drivers. Fast Company. https://www.fastcompany.com/90206668

Raji, I. D., & Buolamwini, J. (2019). Actionable auditing: Investigating the impact of publicly naming biased performance results of commercial AI products. In Proceedings of the 2019 AAAI/ACM Conference on AI, Ethics, and Society (pp. 429–435). https://doi.org/10.1145/3306618.3314244
