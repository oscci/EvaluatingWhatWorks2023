# The randomized controlled trial as a method for controlling biases {#RCT}


<img src="images/logo_alone_new.png" width="143" />

The randomized controlled trial (RCT) is regarded by many as the gold standard method for evaluating interventions. In the next chapter we will discuss some of the limitations of this approach that can make it less than ideal for evaluating certain kinds of non-medical interventions. But in this chapter we'll look at the ingredients of a RCT that make it such a well-regarded method, and introduce the basic methods that can be used to analyse the results.

A RCT is effective simply because it is designed to counteract all of the systematic biases that were covered in previous Chapters.

<table class="table table-striped table-bordered" style="width: auto !important; margin-left: auto; margin-right: auto;">
<caption>(\#tab:rctchart)How the RCT design deals with threats to study validity</caption>
 <thead>
  <tr>
   <th style="text-align:center;"> Biases </th>
   <th style="text-align:center;"> Remedies </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:center;"> Spontaneous improvement </td>
   <td style="text-align:center;"> Control group </td>
  </tr>
  <tr>
   <td style="text-align:center;"> Practice effects </td>
   <td style="text-align:center;"> Control group </td>
  </tr>
  <tr>
   <td style="text-align:center;"> Regression to the mean </td>
   <td style="text-align:center;"> Control group </td>
  </tr>
  <tr>
   <td style="text-align:center;"> Noisy data (1) </td>
   <td style="text-align:center;"> Strict selection criteria for participants </td>
  </tr>
  <tr>
   <td style="text-align:center;"> Noisy data (2) </td>
   <td style="text-align:center;"> Outcome measures with low measurement error </td>
  </tr>
  <tr>
   <td style="text-align:center;"> Selection bias </td>
   <td style="text-align:center;"> Random assignment to intervention </td>
  </tr>
  <tr>
   <td style="text-align:center;"> Placebo effects </td>
   <td style="text-align:center;"> Participant unaware of assignment </td>
  </tr>
  <tr>
   <td style="text-align:center;"> Experimenter bias (1) </td>
   <td style="text-align:center;"> Experimenter unaware of assignment </td>
  </tr>
  <tr>
   <td style="text-align:center;"> Experimenter bias (2) </td>
   <td style="text-align:center;"> Strictly specified protocol </td>
  </tr>
  <tr>
   <td style="text-align:center;"> Biased drop-outs </td>
   <td style="text-align:center;"> Intention-to-treat analysis </td>
  </tr>
  <tr>
   <td style="text-align:center;"> Low power </td>
   <td style="text-align:center;"> A priori power analysis </td>
  </tr>
  <tr>
   <td style="text-align:center;"> False positives due to p-hacking </td>
   <td style="text-align:center;"> Registration of trial protocol </td>
  </tr>
</tbody>
</table>

We cannot prevent changes in outcomes over time that arise for reasons other than intervention (Chapter \@ref(nonspecific)), but if we include a control group we can estimate and correct for their influence. Noisy data in general arises either because of heterogenous participants, or because of unreliable measures: in a good RCT there will be strict selection criteria for participants, and careful choice of outcome measures to be psychometrically sound (see Chapter \@ref(reliability)).  Randomization of participants to intervention and control groups avoids bias caused either by participants' self-selection of intervention group, or experimenters' determining who gets what treatment.  In addition, as noted in Chapter \@ref(nonspecific) and Chapter \@ref(experimenter), where feasible, both participants and experimenters are kept unaware of who is in which treatment group, giving a double-blind RCT.

In Chapter \@ref(phacking), we noted that the rate of false positive results in a study can be increased by p-hacking, where many outcome measures are included but only the "significant" ones are reported. This problem has been recognized in the context of clinical trials for many years, which is why clinical trial protocols are usually registered specifying a primary outcome measure of interest: indeed, as is discussed further in Chapter \@ref(prereg), many journals will not accept a trial for publication unless it has been registered on a site such as https://clinicaltrials.gov/. Note, however, that, as discussed in Chapter \@ref(phacking), multiple outcomes may increase the statistical power of a study, and are not a problem if the statistical analysis handles the multiplicity correctly. Secondary outcome measures can also be specified, but reporting of analyses relating to these outcomes should make it clear that they are much more exploratory. In principle, this should limit the amount of data dredging for an effect that is loosely related to the hypothesis of interest (typically, "is the intervention effective?"). 

RCTs have become such a bedrock of medical research that standards for reporting them have been developed. In Chapter \@ref(dropouts) we saw the CONSORT flowchart, which is a useful way of documenting the flow of participants through a trial. CONSORT stands for Consolidated Standards of Reporting Trials, which are endorsed by many medical journals. Indeed, if you plan to publish an intervention study in one of those journals, you are likely to be required to show you have followed the guidelines. The relevant information is available on the 'Enhancing the QUAlity and Transparency Of health Research' [EQUATOR](http://www.equator-network.org) network website. The EQUATOR network site covers not only RCTs but also the full spectrum guidelines of many types of clinical research designs. 

For someone starting out planning a trial, it is worth reading the CONSORT Explanation and Elaboration document [@moher2010], which gives the rationale behind different aspects of the CONSORT guidelines. This may seem rather daunting to beginners, as it mentions more complex trial designs as well as a standard RCT comparing intervention and control groups, and it assumes a degree of statistical expertise (see below). It is nevertheless worth studying, as adherence to CONSORT guidelines is seen as a marker of study quality, and it is much easier to conform to their recommendations if a study is planned with the guidelines in mind, rather than if the guidelines are only consulted after the study is done.

## Statistical analysis of a RCT

Statisticians often complain that researchers will come along with a collection of data and ask for advice as to how to analyse it. Sir Ronald Fisher (one of the most famous statisticians of all time) commented:

> “To consult the statistician after an experiment is finished is often merely to ask him to conduct a post mortem examination. He can perhaps say what the experiment died of.”

-Sir Ronald Fisher, Presidential Address to the First Indian Statistical Congress, 1938.

His point was that very often the statistician would have advised doing something different in the first place, had they been consulted at the outset. Once the data are collected, it may be too late to rescue the study from a fatal flaw.  

Many of those who train as allied health professionals get rather limited statistical training. We suspect it is not common for them to have ready access to expert advice from a statistician. We have, therefore, a dilemma: many of those who have to administer interventions have not been given the statistical training that is needed to evaluate their effectiveness.

We do not propose to try to turn readers of this book into expert statisticians, but we hope to instill a basic understanding of some key principles that will make it easier to read and interpret the research literature, and to have fruitful discussions with a statistician if you are planning a study. 

The answer to the question "How should I analyse my data?" depends crucially on what hypothesis is being tested. In the case of an intervention trial, the hypothesis will usually be "did intervention X make a difference to outcome Y in people with condition Z?"  There is, in this case, a clear null hypothesis – that the intervention was ineffective, and the outcome of the intervention group would have been just the same if it had not been done.  The null hypothesis significance testing approach answers just that question: it tells you how likely your data are if the the null hypothesis was true. To do that, you compare the distribution of outcome scores in the intervention group and the control group, as explained in Chapter \@ref(power). And as emphasized earlier, we don't just look at the difference in means between two groups, we consider whether that difference is greater than you'd expect given the variation _within_ the two groups. (This is what the term "analysis of variance" refers to).

## Steps to take before data analysis  

- General sanity check on dataset - are values within expected range?
- Check assumptions  
- Plot data to get sense of likely range of results

### Sample dataset with illustrative analysis
To illustrate data analysis, we will use a real dataset that can be retrieved from the [ESRC data archive](https://reshare.ukdataservice.ac.uk/852291/) [@burgoyne2016].  We will focus only on a small subset of the data, which comes from an intervention study in which teaching assistants administered an individual reading and language intervention to children with Down syndrome. A wait-list RCT design was used (see Chapter \@ref(crossover)), but we will focus here on just the first two phases, in which half the children were randomly assigned to intervention, and the remainder formed a control group.  Several language and reading measures were included in the study, giving a total of 11 outcomes. Here we will illustrate the analysis with just one of the outcomes - letter-sound coding - which was administered at baseline (t1) and immediately after the intervention (t2). Results from the full study have been reported by @burgoyne2012 and are discussed in the demonstration of MEff by @bishop2023b. 
<!---this is the measure with the strongest effect - I considered using others but they are not great for illustrative purposes, as they aren't very normal! Script below written so that we could easily substitute one of the other measures if we wished (but then text would also need redoing in places)-->

<div class="figure">
<img src="12-RCT_files/figure-epub3/piratefigRCT-1.png" alt="Data from RCT on language/reading intervention for Down syndrome by @burgoyne2012" width="75%" />
<p class="caption">(\#fig:piratefigRCT)Data from RCT on language/reading intervention for Down syndrome by @burgoyne2012</p>
</div>
Figure \@ref(fig:piratefigRCT) shows results on letter-sound coding after one group had received the intervention.  This test had also been administered at baseline, but we will focus first just on the outcome results. 

Raw data should always be inspected prior to any data analysis, in order to just check that the distribution of scores looks sensible. One hears of horror stories where, for instance, an error code of 999 got included in an analysis, distorting all the statistics. Or where an outcome score was entered as 10 rather than 100. Visualising the data is useful when checking whether the results are in the right numerical range for the particular outcome measure.  The [pirate plot](https://www.psychologicalscience.org/observer/yarrr-the-pirates-guide-to-r) is a useful way of showing means and distributions as well as individual data points. 

A related step is to check whether the distribution of the data meets the assumptions of the proposed statistical analysis. Many common statistical procedures assume that data are normally distributed on an interval scale (see Chapter \@ref(reliability)). Statistical approaches to checking of assumptions are beyond the scope of this book, but there are good sources of information on the web, such as [this website](http://www.sthda.com/english/articles/39-regression-model-diagnostics/161-linear-regression-assumptions-and-diagnostics-in-r-essentials/) for linear regression. But just eyeballing the data is useful, and can detect obvious cases of non-normality, cases of ceiling or floor effects, or "clumpy" data, where only certain values are possible. Data with these features may need special treatment and it is worth consulting a statistician if they apply to your data. For the data in Figure \@ref(fig:piratefigRCT), although neither distribution has an classically normal distribution, we do not see major problems with ceiling or floor effects, and there is a reasonable spread of scores in both groups.  
<!-- maybe add a figure showing egs of nonnormal distribution, ceiling effect, clumpy data-->


<table class="table table-striped table-bordered" style="width: auto !important; margin-left: auto; margin-right: auto;">
<caption>(\#tab:table2gp)Summary statistics on letter-sound coding at posttest</caption>
 <thead>
  <tr>
   <th style="text-align:center;"> Group </th>
   <th style="text-align:center;"> N </th>
   <th style="text-align:center;"> Mean </th>
   <th style="text-align:center;"> SD </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:center;"> Intervention </td>
   <td style="text-align:center;"> 28 </td>
   <td style="text-align:center;"> 22.286 </td>
   <td style="text-align:center;"> 7.282 </td>
  </tr>
  <tr>
   <td style="text-align:center;"> Control </td>
   <td style="text-align:center;"> 26 </td>
   <td style="text-align:center;"> 16.346 </td>
   <td style="text-align:center;"> 9.423 </td>
  </tr>
</tbody>
</table>


The next step is just to compute some basic statistics to get a feel for the effect size. Table \@ref(tab:table2gp) shows the mean and standard deviation on the outcome measure for each group. The mean is the average of the individual datapoints shown in Figure \@ref(fig:piratefigRCT), obtained by just summing all scores and dividing by the number of cases. The standard deviation gives an indication of the spread of scores around the mean. As discussed in Chapter \@ref(power), the SD is a key statistic for measuring an intervention effect. In these results, one mean is higher than the other, but there is overlap between the groups.  Statistical analysis gives us a way of quantifying how much confidence we can place in the group difference: in particular, how likely is it that there is no real impact of intervention and the observed results just reflect the play of chance.  In this case we can see that the difference between means is around 6 points and the average SD is around 8, so the effect size (Cohen's _d_) is about .75 - a large effect size for a language intervention. 

### Simple t-test on outcome data  
The simplest way of measuring the intervention effect is to just compare outcome (posttest) measures on a t-test. We can use a one-tailed test with confidence, given that we anticipate outcomes will be better after intervention.  One-tailed tests are often treated with suspicion, because they can be used by researchers engaged in p-hacking (see Chapter \@ref(phacking)), but where we predict a directional effect, they are entirely appropriate and give greater power than a two-tailed test: see [this blogpost by Daniël Lakens](http://daniellakens.blogspot.com/2016/03/one-sided-tests-efficient-and-underused.html).  
When reporting the result of a t-test, researchers should always report all the statistics: the value of t, the degrees of freedom, the means and SDs, and the confidence interval around the mean difference, as well as the p-value. This not only helps readers understand the magnitude and reliability of the effect of interest: it also allows for the study to readily be incorporated in a meta-analysis. Results from a t-test for the data in Table \@ref(tab:table2gp) are shown in Table \@ref(tab:ttestoutcomes). Note that with a one-tailed test, the confidence interval on one side will extend to infinity: this is because a one-tailed test assumes that the true result is greater than a specified mean value, and disregards results that go in the opposite direction.  <!-- not sure that is at all clear-->

<table class="table table-striped table-bordered" style="width: auto !important; margin-left: auto; margin-right: auto;">
<caption>(\#tab:ttestoutcomes)T-test on outcomes</caption>
 <thead>
  <tr>
   <th style="text-align:center;"> t </th>
   <th style="text-align:center;"> df </th>
   <th style="text-align:center;"> p </th>
   <th style="text-align:center;"> mean diff. </th>
   <th style="text-align:center;"> lowerCI </th>
   <th style="text-align:center;"> upperCI </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:center;"> 2.602 </td>
   <td style="text-align:center;"> 52 </td>
   <td style="text-align:center;"> 0.006 </td>
   <td style="text-align:center;"> 5.94 </td>
   <td style="text-align:center;"> 2.117 </td>
   <td style="text-align:center;"> Inf </td>
  </tr>
</tbody>
</table>



### T-test on difference scores  
The t-test on outcomes is easy to do, but it misses an opportunity to control for one unwanted source of variation, namely individual differences in the initial level of the language measure. For this reason, researchers often prefer to take difference scores: the difference between outcome and baseline measures, and apply a t-test to these. While this had some advantages over reliance on raw outcome measures, it also has disadvantages, because the amount of change that is possible from baseline to outcome is not the same for everyone. A child with a very low score at baseline has more "room for improvement" than one who has an average score. For this reason, analysis of difference scores is not generally recommended.  

### Analysis of covariance on outcome scores  
Rather than taking difference scores, it is preferable to analyse differences in outcome measures after making a statistical adjustment that takes into account the initial baseline scores, using a method known as analysis of covariance or ANCOVA. In practice, this method usually gives results that are very similar to those you would obtain from an analysis of difference scores, but the precision, and hence the statistical power is greater.  However, the data do need to meet certain assumptions of the method. This [website](#https://www.datanovia.com/en/lessons/ancova-in-r/) walks through the steps for performing an ANCOVA in R, starting with a plot of  to check that there is a linear relationship between pretest vs posttest scores in both groups - i.e. the points cluster around a straight line, as shown in Figure \@ref(fig:ds-prepost).
<div class="figure">
<img src="12-RCT_files/figure-epub3/ds-prepost-1.png" alt="Pretest vs posttest scores in the Down syndrome data"  />
<p class="caption">(\#fig:ds-prepost)Pretest vs posttest scores in the Down syndrome data</p>
</div>
Inspection of the plot confirms that the relationship between pretest and posttest looks reasonably linear in both groups. Note that it also shows that there are rather more children with very low scores at pretest in the control group. This is just a chance finding - the kind of thing that can easily happen when you have relatively small numbers of children randomly assigned to groups.  

<table class="table table-striped table-bordered" style="width: auto !important; margin-left: auto; margin-right: auto;">
<caption>(\#tab:ancova-compare)Analysis of posttest only (ANOVA)</caption>
 <thead>
  <tr>
   <th style="text-align:center;"> Effect </th>
   <th style="text-align:center;"> DFn </th>
   <th style="text-align:center;"> DFd </th>
   <th style="text-align:center;"> F </th>
   <th style="text-align:center;"> p </th>
   <th style="text-align:center;"> ges </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:center;font-weight: bold;"> group </td>
   <td style="text-align:center;"> 1 </td>
   <td style="text-align:center;"> 52 </td>
   <td style="text-align:center;"> 6.773 </td>
   <td style="text-align:center;"> 0.012 </td>
   <td style="text-align:center;"> 0.115 </td>
  </tr>
</tbody>
</table>

<table class="table table-striped table-bordered" style="width: auto !important; margin-left: auto; margin-right: auto;">
<caption>(\#tab:ancova-compare)Analysis adjusted for pretest scores (ANCOVA)</caption>
 <thead>
  <tr>
   <th style="text-align:center;"> Effect </th>
   <th style="text-align:center;"> DFn </th>
   <th style="text-align:center;"> DFd </th>
   <th style="text-align:center;"> F </th>
   <th style="text-align:center;"> p </th>
   <th style="text-align:center;"> ges </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:center;"> pretest </td>
   <td style="text-align:center;"> 1 </td>
   <td style="text-align:center;"> 51 </td>
   <td style="text-align:center;"> 94.313 </td>
   <td style="text-align:center;"> 0.000 </td>
   <td style="text-align:center;"> 0.649 </td>
  </tr>
  <tr>
   <td style="text-align:center;"> group </td>
   <td style="text-align:center;"> 1 </td>
   <td style="text-align:center;"> 51 </td>
   <td style="text-align:center;"> 9.301 </td>
   <td style="text-align:center;"> 0.004 </td>
   <td style="text-align:center;"> 0.154 </td>
  </tr>
</tbody>
</table>
Table \@ref(tab:ancova-compare) shows the same data analysed by first of all by using ANOVA to compare only the post-test scores (upper chart) and then using ANCOVA to adjust scores for the baseline (pretest) values. The effect size is shown as ges, which stands for "generalized eta squared". You can see there is a large ges value, and correspondingly low p-value for the pretest term, reflecting the strong correlation between pretest and posttest shown in Figure \@ref(fig:ds-prepost). In effect, with ANCOVA, we adjust scores to remove the effect of the pretest on the posttest scores; in this case, we can then see a slightly stronger effect of the intervention: the effect size for the group term is higher and the p-value is lower than with the previous ANOVA.  
For readers who are not accustomed to interpreting statistical output, the main take-away message here is that you get a better estimate of the intervention effect if the analysis uses a statistical adjustment that takes into account the pre-test scores.  


#### T-tests, analysis of variance, and linear regression  {-}

<div id="custom">Mathematically, the t-test is equivalent to two other methods: analysis of variance and linear regression. When we have just two groups, all of these methods achieve the same thing: they divide up the variance in the data into variance associated with group identity, and other (residual) variance, and provide a statistic that reflects the ratio between these two sources of variance. This is illustrated with the real data analysed in Table \@ref(tab:ancova-compare). The upper analysis gives results that are equivalent to the t-test in Table \@ref(tab:ttestoutcomes): if you square the t-value it is the same as the F-test. In this case, the p-value from the t-test is half the value of that in the ANOVA: this is because we specified a one-tailed test for the t-test. The p-value would be identical to that from ANOVA if a two-tailed t-test had been used.  
See [this blogpost](http://deevybee.blogspot.com/2017/11/anova-t-tests-and-regression-different.html) for more details.
<!-- reminder to self: blogposts referenced in the book should be uploaded to figshare or another place with DOI--></div>



### Linear mixed models (LMM) approach  
Increasingly, reports of RCTs are using more sophisticated and flexible methods of analysis that can, for instance, cope with datasets that have missing data, or where distributions of scores are non-normal. 
<!---With a linear mixed model (LMM), we can also take into account individual differences in response to intervention. These are very evident when we plot the baseline and posttest scores for individual participants (Figure \@fig(indsubs-plot)).-->




An advantage of the LMM approach is that it can be extended in many ways to give appropriate estimates of intervention effects in more complex trial designs - some of which are covered in Chapter \@ref(adaptive) to Chapter \@ref(Single)). Disadvantages of this approach are that it is easy to make mistakes in specifying the model for analysis if you lack statistical expertise, and the output is harder for non-specialists to understand.  If you have a simple design, such as that illustrated in this chapter, with normally distributed data, a basic analysis of covariance is perfectly adequate [@oconnell2017].


<!--- Paul's help needed here?  I had assumed LMM would give more precise estimates, but the OConnell paper suggests ANCOVA is optimal-->


Table \@ref(tab:table-procon) summarises the pros and cons of different analytic approaches.

<table class="table table-striped table-bordered" style="width: auto !important; margin-left: auto; margin-right: auto;">
<caption>(\#tab:table-procon)Analytic methods for comparing outcomes in intervention vs control groups</caption>
 <thead>
  <tr>
   <th style="text-align:center;"> Method </th>
   <th style="text-align:center;"> Features </th>
   <th style="text-align:center;"> Ease of understanding </th>
   <th style="text-align:center;"> Flexibility </th>
  </tr>
 </thead>
<tbody>
  <tr>
   <td style="text-align:center;"> t-test </td>
   <td style="text-align:center;"> Good power with 1-tailed test. 
Suboptimal control for baseline. 
Assumes normality. </td>
   <td style="text-align:center;"> High </td>
   <td style="text-align:center;"> Low </td>
  </tr>
  <tr>
   <td style="text-align:center;"> ANOVA </td>
   <td style="text-align:center;"> With two-groups, equivalent to t-test, 
but two-tailed only. 
Can extend to more than two groups. </td>
   <td style="text-align:center;"> ... </td>
   <td style="text-align:center;"> ... </td>
  </tr>
  <tr>
   <td style="text-align:center;"> Linear regression/ ANCOVA </td>
   <td style="text-align:center;"> Similar to ANOVA, but can adjust 
outcomes for covariates, 
including baseline. </td>
   <td style="text-align:center;"> ... </td>
   <td style="text-align:center;"> ... </td>
  </tr>
  <tr>
   <td style="text-align:center;"> LMM </td>
   <td style="text-align:center;"> Flexible in cases with missing data, 
non-normal distributions. </td>
   <td style="text-align:center;"> Low </td>
   <td style="text-align:center;"> High </td>
  </tr>
</tbody>
</table>


## Class exercise  

1. Find an intervention study of interest and check whether the protocol was deposited in a repository before the study began. If so, check the analysis against the preregistration, cf. @goldacre2019. 
Note which analysis method was used to estimate the intervention effect.  
Did the researchers provide enough information to give an idea of the effect size, or merely report p-values? Did the analysis method take into account baseline scores in an appropriate way?  

2. In Chapter \@ref(drawbacks) we consider drawbacks of the RCT design. Before you read that chapter, see if you can anticipate the issues that we consider in our evaluation. 


