#Revision of the Solow growth model with R

##Description

This repository provides a revision of the Solow growth model based on the paper of Mankiw, Romer & Weil (1992) (source).*Gregory N. Mankiw, David Romer, and David N. Weil. A contribution to the empirics of economic growth. Number 3541 in Working Paper Series. December 1992.*

The model was replicated and tested in R. Also, the original results of Mankiw, Romer & Weil (1960 - 1985) were enhanced with up-to-date data (1985 - 2010). This project is documented in the paper:*Maike Warneke, Justs Hövelmann, Laura Gabrysiak Gomez. A Revision of the Solow Model in R. Humbold University. July 2015.*

If you use the code/dataset for your work, please **cite** the paper. **BiBTeX entry**:
```
@paper{solow_r_2015,
   author = {Maike Warneke, Justus H\"{o}velmann, Laura Gabrysiak G\'{o}mez},
   title = {{A Revision of the Solow Model in R}},
   month = July,
   year = {2015}
}
```
If you have questions, email laura [dot] gabrysiak [at] gmail


##Introduction

Ever since Robert Solow developed his path breaking model of economic growth in
the 1950s, it has served as a benchmark for considerations about economic develop-
ment and technological progress. Moreover, it still functions as an important tool to teach the mechanics of economic
growth even in the context of state of the art macroeconomic theory. Though
reviewed and augmented by a variety of scholars since its first formulation, the basic
mechanics behind the model have in general been unaltered.
One of the most acknowledgeable contributions to the textbook model has been
made by Mankiw, Romer and Weil in 1992. By incorporating the role of human
capital accumulation as an additionally defined variable they succeed in providing
regressions with a much better statistical fit in comparison to the ”default” model
settings.

While first and foremost focusing on the traditional textbook model, we also consider
the augmentations made by MRW to reassess the Solow model’s goodness of
fit for different modifications. Thus, we are able to review the main predictions of
the model in the light of world wide’s economic development during the past 50
years.

The paper is structured as follows: We will first provide a theoretical overview about
the Solow model’s assumptions, its derivation and its implications for the theory of
economic growth (see Section 3). After a short summary of literature (see Section
2) and an overview of our process of data generation (see Section 4) we will focus
on replicating the traditional Solow model in R using the assumptions formulated
by MRW (see Section 5). This setup includes the original time horizon from 1960
to 1985 and the default country grouping mentioning OECD countries, Non-Oil and
Intermediate economies. Data is provided by World Bank (WDI) and Penn World.

In the following, Mankiw, Romer and Weil (1992) will be abbreviated by MRW.
4Tables, which can in part be included in R as packages. In addition, we program
the augmented model formulated by MRW in 1992, incorporating human capital
formation as a crucial element (see Section 5).
After checking the quality of our resembled models by comparing regression output
with the results of the original paper, we apply some modifications to check for
potential breaks in the theory.

For the default model without human capital we apply different time horizons (1986
to 2010 as well as 1960 to 2010) to the model.
Furthermore, we are able to apply a recently developed dataset to the original model.
While MRW had to rely on a proxy for estimating the effect of human capital
formation on the technological progress of an economy, the latest version of our data
source (Penn World Tables 8.0) introduces a newly developed Human Capital
Index. This variable is not only based on the average years of schooling - as also
used by the original authors - but serves as a combination of relevant factors, e.g.
an assumed rate of return associated with higher education and the worker’s level
of job training.

We use the data from this source to assess the model’s predictive power for one
subsample (Non-Oil) and different time spans compared to the default version of
the augmented model.

Our empirical work leaves us with the conclusion that the original Solow model as
well as its augmented version by MRW still combine a fairly elegant way of describing
the processes behind capital formation in a closed economy, whilst delivering a high
predictive power and a good statistical fit.

