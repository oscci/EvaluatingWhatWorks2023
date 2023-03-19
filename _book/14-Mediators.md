# Moderators and mediators of intervention effects {#mediators}


<img src="images/logo_alone_new.png" width="143" />


## Moderators  
We concluded Chapter \@ref(drawbacks) by noting the heterogeneity of intervention effects, even in an experimental context where the treated individuals (chicks) had similar genetic backgrounds and upbringing. In real-life contexts with humans, we anticipate that there may be a number of factors that have a systematic influence on the effectiveness of interventions.  These are referred to as **moderators**, and if we can identify them, then this will help us identify the best way of selecting individuals for intervention - either in the clinic, or in future intervention studies. 

In the context of a RCT, a potential moderator is a characteristic of the individual that is measured in the baseline period. For example, in a study of children, we might divide them according to a measure of economic status, whether or not the child is eligible for free school meals. This is our moderator, M, and in this example, it just divides the sample into two subgroups. 

To show that M is a moderator of treatment, we have to demonstrate that there is an interaction between M and the treatment effect, as shown in Figure \@ref(fig:modfig).  Note that the key feature is the slope of the line between baseline and outcome measurements. The overall intervention effect is estimated from the difference in the slopes for intervention and control groups. If the size of the intervention effect is different for the two Free School Meals subgroups, then we conclude that Free School Meals status is a moderator. 




<div class="figure">
<img src="Images/Moderator.png" alt="Interaction between intervention effect and Free School Meals status" width="75%" />
<p class="caption">(\#fig:modfig)Interaction between intervention effect and Free School Meals status</p>
</div>
Moderators are often characteristics of the individual, such as age, sex, severity, or comorbid conditions), and can be used to determine for whom an intervention will be most effective. Other moderators may be the related to the circumstances in which the intervention is administered, e.g., whether at school or in a clinic. @morrow2022 noted that moderation analysis is particularly relevant when considering interventions used with heterogeneous populations, such as individuals who have had brain damage, where age, location and duration of damage may have important effects on outcome. Rather than trying to correct for variation in outcome caused by these characteristics, with moderation analysis we aim to estimate which factors are important.

Although the idea of studying moderators is attractive, in practice it can be difficult to demonstrate such effects. One reason is that large sample sizes are needed to have adequate statistical power to demonstrate interaction effects (see \@ref(power)), so unless moderator effects are substantial, they may be missed. Second, as noted by @kraemer2002, moderator analyses usually are exploratory rather than hypothesis-testing, and so when a moderator is discovered, it will need to be replicated in a new sample. This relates back to the arguments in Chapter \@ref(phacking), where we argued that you should *never generate and test a hypothesis using the same data*. Nevertheless, Kraemer et al (2002) argue there can be value in performing moderator analyses, as it means we can devise future interventions that incorporate the information gained from previous studies. 

## Mediators  
Mediators provide theoretically useful information about why and how interventions have an effect. The principal way of distinguishing between moderators and mediators is in terms of the time of their impact. A moderator is a pre-existing variable that is independent of the allocation of individuals to intervention and control groups, but which can be shown to affect the response to intervention.  In contrast, a mediator is a measured variable that changes with intervention. An example is provided by a study on reading intervention by @hulme2012. These authors contrasted two types of intervention for children with weak oral language skills. The first group (P+R) were trained in phoneme awareness,  letter-sound knowledge, and guided reading of simple books. The second group (OL) had an intervention focused on oral language development, including vocabulary, grammar and narrative skills. Outcome was measured at the end of 20 weeks of intervention, and again five months later, and it was shown that the P+R group were superior at reading. A mediation analysis was conducted to test whether improved phonemic awareness and letter-sound knowledge had led to the gains in reading. Rather than showing here the complex path diagram presented by the authors, Figure \@ref(fig:medfig) shows two simplified models that can be compared by analysing the patterns of correlation between the measurements. In these models, arrows between variables indicate that they are significantly correlated, after taking into account all the associations between the variables.  This kind of model is analysed by using a statistical method such as path analysis, which focuses on the pattern of correlations between variables.  We know from a prior analysis that there was a benefit to reading for the P+R group, and this group also showed gains in phonemic awareness, so both models include these effects. For Model A, the two effects are independent - i.e., the intervention improves reading and improves phonemic awareness, but the two impacts are unrelated. In this case, there is no mediation effect. For Model B, there is no direct effect of intervention on reading: instead, the effect is entirely mediated by phonemic awareness. In other words, once we have taken into account the gains shown in phonemic awareness, we have explained the gains in reading. By analysing the pattern of correlations between variables, we can see which model gives a better fit to the observed data. In practice, the models that are tested tend to be much more complex, and take into account additional variables, but this simplified account is sufficient to demonstrate the logic of a mediation analysis. 

<div class="figure">
<img src="Images/Mediation_diagram.jpg" alt="Models illustrating mediation vs no mediation in reading intervention study" width="75%" />
<p class="caption">(\#fig:medfig)Models illustrating mediation vs no mediation in reading intervention study</p>
</div>

## Class exercise

Here are some characteristics of mediators and moderators. See if you can work out whether M refers to mediation or moderation.  
1. In a M relationship, you can draw an arrow from intervention to M and then from M to the outcome.  Mediation|moderation  
2. M refers to the case when something acts upon the relationship between intevention and outcome, and changes its strength.  Mediation|moderation  
3. M can be thought of as a go-between for intervention and outcome: it is a variable that explains their relationship.  Mediation|moderation  
4. The Figure below shows an intervention where both mediation and moderation are involved. Which is M1 and which is M2?
<img src="Images/Medmod.jpg" width="50%" />

