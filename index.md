How to perform analyses in the light of ASA’s recent statement on
p-values
================
Matthew Loop
2019-08-09

# Introduction

The American Statistical Association (ASA) released a statement in March
urging the scientific community to abandon the use of the phrase
“statistically significant.” Specifically, it said,

> We conclude, based on our review of the articles in this special issue
> and the broader literature, that it is time to stop using the term
> “statistically significant” entirely. Nor should variants such as
> “significantly different,” “p \< 0.05,” and “nonsignificant”
> survive, whether expressed in words, by asterisks in a table, or in
> some other way.
> 
> — Ron Wasserstein, Allen Schirm, and Nicole Lazar

Why did the ASA make this recommendation? Well, earlier in the editorial
they mention the following:

> If you’re just arriving to the debate, here’s a sampling of what not
> to do:
> 
>   - Don’t base your conclusions solely on whether an association or
>     effect was found to be “statistically significant” (i.e., the
>     p-value passed some arbitrary threshold such as \(p < 0.05\)).  
>   - Don’t believe that an association or effect exists just because it
>     was statistically significant.  
>   - Don’t believe that an association or effect is absent just because
>     it was not statistically significant.  
>   - Don’t believe that your p-value gives the probability that chance
>     alone produced the observed association or effect or the
>     probability that your test hypothesis is true.  
>   - Don’t conclude anything about scientific or practical importance
>     based on statistical significance (or lack thereof)

# The problem

So statisticians are telling me I’m wrong…again\! What am I supposed to
do?

> Don’t. Don’t. Just…don’t. Yes, we talk a lot about don’ts. The ASA
> Statement on p-Values and Statistical Significance (Wasserstein and
> Lazar 2016) was developed primarily because after decades, warnings
> about the don’ts had gone mostly unheeded. The statement was about
> what not to do, because there is widespread agreement about the
> don’ts. Knowing what not to do with p-values is indeed necessary,
> but it does not suffice. It is as though statisticians were asking
> users of statistics to tear out the beams and struts holding up the
> edifice of modern scientific research without offering solid
> construction materials to replace them. Pointing out old, rotting
> timbers was a good start, but now we need more.

# My background

  - Background in Biology, but PhD in Biostatistcs and work as an
    applied statistician
  - Served as both lead author and collaborating statistician on applied
    papers
  - I’ve said “statistically significant” about p-values quite a
lot

# 3 recommendations for what to do\[1\]

## 1\. Talk about risk/odds/hazard ratios that are consistent with the data

So if you aren’t supposed to say something is “statistically
significant,” what do you say? I’ve started thinking about my results in
terms of

1.  values are consistent with the data?
2.  what values are inconsistent/ruled out by the data

For example let’s say you estimated an odds ratio of 1.1 with a
confidence interval of (0.95, 1.27) for the treatment versus control
group on medication adherence over the next 7 days. Now, in the old
paradigm, I would say that there was “no statistically significant
evidence of an association between the treatment on medication
adherence.” This interpretation comes strictly from the null hypothesis
significance testing framework, where we claim all we are interested in
is whether the odds ratio is 1 or not. But in reality, it’s unlikely any
treatment has an effect of exactly 0.

Nowadays, I look at a result like this and think the following:

> Well, our best estimate is that the odds are 10% higher for being
> adherent in the treatment group compared to the control. In fact, the
> data are consistent with having a 25% increase in adherence, which
> would be great\! However, because of the large amount of uncertainty,
> we can’t rule out the fact that the treatment may reduce adherence.
> How can we reduce variation in our estimate? Are we sure the treatment
> was administered in exactly the same way? Do we have better, more
> accurrate ways to measure adherence? Is there a lot of measurement
> error? Are there other variables that do a good job of predicting
> adherence, so that we can reduce the uncertainty in the estimate of
> our treatment effect? If I were going to bet on it, the treatment is
> probably helpful, given that a larger proportion of the odds ratios
> consistent with the data are positive. But we need to rule out a
> negative effect, if this treatment is truly effective. Let’s do
> another study…

This reaction, and the follow up actions, are much different than
saying, "Well, we didn’t find an effect. So there probably isn’t
one.\[2\]

## 2\. Ask yourself, “Did I learn anything?”

Now let’s present a little bit different scenario, where your
traditional interpretation would be the same as the previous one.

Let’s assume that the odds ratio you estimated was 1.05 (0.1, 11.03).
The traditional approach would be the same: “we found no statistically
significant evidence of an effect of treatment on adherence.”

I would say something different. I would put forth that you learned
absolutely nothing from doing this study. The thinking goes like this.

> I do observational research on behavioral interventions on adherence.
> Most odds ratios tend to be small, with a high probability of being
> between 0.8 and 1.2. An effect bigger than that would be considered
> absolutely huge and a big breakthrough. Now, I just got this range of
> values consistent with the data from 0.1 to 11.03. But I was expected
> any real treatment effect to be much closer to one. I haven’t learned
> anything.

A result like this definitely brings to light major problems with the
study. It’s likely you didn’t have enough sample size, or your
measurements were too noisy, to really be able to study the effect of
your intervention at all. A bigger, better study is definitely needed.

## 3\. Avoid treating statistics as “uncertainty laundering”\[3\]

Somehow, the p value became the ultimate and final judge of whether a
scientific theory was true. Some of that “success” might be because
we’re simply more comfortable with binary thinking: this study found
something; this one didn’t. This treatment improves cancer remission
rates; this one doesn’t. But we shouldn’t let a tool that was designed
to help make a *decision* stand in for our hard thinking about what is a
*fact.*

Science isn’t that simple, and we know it.

# How to do it

## Rewriting a results section

![](figure.png)<!-- -->

*Of the total sample (\(n=20,150\)), 1,633 participants (8%) were
classified as cognitively impaired at their most recent follow-up. Table
5 shows the odds ratios and approximate 95% Wald’s confidence intervals
for a 10 µg/m3 change in PM\(_{2.5}\) for each of the four models, both
for the main analysis (impaired on the most recent assessment) and
sensitivity analysis (impaired on both of the two most recent
assessments). Model 1 indicated that there was no association between
PM2.5 and the odds of incident cognitive impairment. The odds ratio
decreased sharply after demographics were added (model 2), with an odds
ratio close to 1. This estimated odds ratio was more or less constant
for models 3 and 4.*

## Responding to a journal reviewer

# How the world could be different

1.  Most of my opinions about this and how I’ve changed in my
    interpretations of p-values have to do with the thoughts of [Frank
    Harrell](https://www.fharrell.com/post/) and [Andrew
    Gelman](https://statmodeling.stat.columbia.edu). I’ve borrowed
    heavily from them, and I highly recommend that you do the same.

2.  Even though that’s the incorrect interpreation of a p value, that’s
    often how they are used.

3.  Term ‘uncertainty laundering’ comes from Andrew Gelman in this same
    editorial as well as at
    <https://statmodeling.stat.columbia.edu/2016/03/07/29212/>
