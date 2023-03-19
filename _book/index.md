--- 
title: "Evaluating What Works"
author: "Dorothy V M Bishop and Paul A Thompson"
date: "March 19, 2023"
documentclass: book
bibliography: [book.bib,packages.bib]
csl: apa.csl
link-citations: true
description: Introduction to methods for evaluating effectiveness of non-medical interventions
site: bookdown::bookdown_site
always_allow_html: true
---



# Preface {-}
<!---- for include_image you need bookdownplus package. This was problematic so I now have the include_graphics version-->


<!---- Useful information on bibtext formatting from Zotero is here: https://retorque.re/zotero-better-bibtex/citing/ -->
<center>
<img src="images/logo_alone_new.png" width="143" />
</center>




## Why did we write this book? {-}

Those who work in allied health professions aim to make people's lives better. Often, however, it is hard to know how effective we have been: would change have occurred if we hadn't intervened? Is it possible we are doing more harm than good? To answer these questions and develop a body of knowledge about what works, we need to evaluate interventions.  

As we shall see, demonstrating that an intervention has an impact is much harder than it appears at first sight. There are all kinds of issues that can arise to mislead us into thinking that we have an effective treatment when this is not the case. On the other hand, if a study is poorly designed, we may end up thinking an intervention is ineffective when in fact it is beneficial. Much of the attention of methodologists has focused on how to recognize and control for unwanted factors that can affect outcomes of interest. But psychology is also important: it tells us that own human biases can be just as important in leading us astray. Good, objective intervention research is vital if we are to improve the outcomes of those we work with, but it is really difficult to do it well, and to do so we have to overcome our natural impulses to interpret evidence in biased ways.

## Who is this book for? {-}

The inspiration for the book came from interactions with speech and language therapists (known as speech-language pathologists or logopeds outside the UK), and the illustrative cases are from that discipline, but the basic principles covered here are relevant for any field where a practitioner aims to influence outcomes of those they work with. This includes allied health professions and education.  

In medicine, practitioners who wish to evaluate treatments typically have access to expert statisticians and methodologists, who can advise them on the most efficient research designs and up-to-date analyses. They may also be able to access substantial amounts of funding to cover the salaries of experienced trials personnel. However, in many fields, professionals who administer interventions have limited training in research design, and little or no support from professional statisticians or methodologists. Training in most professions allied to health and education does not usually include much instruction in research methodology and statistics - particularly as this relates to evaluation of interventions, which is a complex and thorny topic. It seemed, therefore that there was a need for a basic text that would explain the rationale and potential pitfalls of intervention research, as well as providing a template for good practice in the evaluation and design of intervention studies. 

## What is covered? {-}

This book is not a how-to-do-it manual, so much as a why-to-do-it. Our main goal is to instill in the reader awareness of the numerous sources of bias that can lead to mistaken conclusions when evaluating interventions. Real-life examples are provided with the aim of providing an intuitive understanding of these issues. Of course, it is not much use telling people what _not_ to do if you don't also give guidance on approaches that are effective. We will illustrate ways in which different research designs can overcome problems, but it is beyond the scope of this book to give detailed instructions on how to implement different methods: instead, we will point readers to other sources that give more in-depth information. 

Our focus is on quantitative research methods. Qualitative research methods are increasingly recognized as providing an important complementary perspective on intervention research, by throwing light on the reasons why people - both those receiving intervention and those implementing it - behave as they do. Sometimes it makes more sense to do a qualitative study to refine a research question before diving in using methods that require that everything is converted into numbers [@greenhalgh1997]. If you feel that a quantitative study is missing out on something essential and important about how and why intervention works, this may be an indication that a qualitative study is needed to scope out the problem more fully. Our expertise, however, is with quantitative methods, and our aim is to write a basic explainer of how such studies are designed, and what biases and pitfalls they can involve. 

The intended readership is those who have little or no background in statistics. Lack of statistical training is a massive obstacle to practitioners who want to do intervention research: it not only makes design and analysis of a study daunting, but it also limits what messages the reader can take from the existing literature. This book should be seen as complementing rather than substituting for a technical introduction to statistics. Many readers may be reluctant to study statistics in more depth, but it is hoped that the account given here will give them confidence to approach statistics in the published literature with a more critical eye, to recognize when the advice of a professional statistician is needed, and to communicate more effectively with statisticians. We recommend Russell Poldrack's open source text [Statistical Thinking for the 21st Century](https://github.com/statsthinking21/statsthinking21) as a complement to this book for those who wish to learn more about statistics.  

Intervention research is a branch of science, and you can't do good science without adopting a critical perspective – to the research of yourself as well as others. We hope this book will make it easier to do that and so to improve intervention research in a range of non-medical fields. 

## Acknowledgements {-}
We owe a huge debt of gratitude to Yihue Xie, whose work developing the [_bookdown_ package](https://bookdown.org/) made this book possible. It is no exaggeration to say that we would not have attempted to write a book on this topic if we hadn't had _bookdown_ to make it easy. The book [ModernDive: Statistical Inference via Data Science](https://moderndive.com/) by Chester Ismay and Albert Y. Kim was also highly influential in demonstrating what could be done with _bookdown_, and we frequently visited their code to check out ideas for formatting and packaging information.  
Our thanks also to James Pustejovsky whose recommendations were helpful in relation to single case designs. 

## Feedback and contributions {-}
One of the good things about an online open source book is that it can remain a work in progress for some time, giving readers the opportunity to provide suggestions and corrections. We can't guarantee to respond promptly (DB is retired and PT has a demanding job!), but we would be extremely grateful to anyone who lets us know of any errors in the book, and we welcome suggestions for additional or alternative content. Our code is available [here](https://github.com/oscci/bookdown_2023) and we encourage readers familiar with Github to send pull requests with suggestions for changes; otherwise please contact us via bishopdeevy@gmail.com. 

## License {-}
The book is licensed according to the [Creative Commons Attribution-NonCommercial 4.0 Generic (CC BY-NC 4.0) License](https://creativecommons.org/licenses/by-nc/4.0/). Please see the terms of that license for more details.


_[Dorothy V. M. Bishop](https://orcid.org/0000-0002-2448-4033) \& [Paul A. Thompson](https://orcid.org/0000-0001-9940-6913)_
