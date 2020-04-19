# Assignment 3

## Introduction 

Diseases can spread in any country or region on the globe. Where there are humans inhabitant, diseases can spread from human to human. The majority of the disease spread is contributed by vast human connectivity and travel patterns. Thus, a good way to try and prevent epidemics to occur is to gather more information about how a disease is spread. This can be done through measuring and mapping human networks and travel patterns. This method is seen in spatial epidemiology, a field that is concerned with diseases and its geographic variations. An important idea in spatial epidemiology is that each region come with its own contextualized geography and set of conditions that affect how a disease is born, incubated, and spread. A quality that is consistently found across studies is that there is high heterogeneity between countries, and even between regions of a country. This makes the characteristics of each disease highly contextualized to the area being studied.

Malaria prevalence is found in countries all over Sub-Saharan Africa. Many of these countries have implemented intervention methods to reduce the spread of malaria, specifically to children under the age of 5 because they are the most vulnerable. Since 2000, there has been an increase in effective malaria control and a decline in global mortality rates due to malaria. For example, the Swaziland National Malaria Control Program reports a deline in malaria cases of 2.9 to 0.07 per 1000 people since 1999. Some intervention methods include, but not limited to, indoor residual spraying (IRS), insecticide-treated bed nets (ITNs), long-lasting insecticidal nets (LLINs), and vaccinations. The broad research question that is explored is: What is the most effective way of gathering, monitoring, and decision-making for decreasing malaria prevalence in sub-Saharan Africa? This is of importance because there have been many deployments of LLINS and IRS within the last decade. Even with the prompt and effective use of these antimalarials, this area still holds high malaria prevalence because it contains the most efficient vector species: *Anopheles gambiae*.

Overall, the healthcare aspect of spatial epidemiology relates to Amartya Sen’s definition of human development. Amartya Sen explains that human development should be viewed as freedom, that regions should develop so that its people can expand their freedoms, starting with the ability to access basic freedoms such as good health. Furthermore, in order for a country, like Nigeria, to develop, that country should focus on improving healthcare access or providing health interventions to combat any situation that does not allow good health for all. The ability to provide healthcare facilities, for example, is being improved through data science methodologies.

The success of elimination interventions is contributed by highly contextualized population information, as well as geographical data, and other important information. Before interventions or policies can be planned, governments and organizations, such as the Global Malaria Programme (GMP) of the World Health Organization (WHO), need a reliable set of data to base their strategies on. For the best, and most effective way, to reach a sustainable development goal, countries need to invest in high quality data so that these organizations can strengthen their scientific basis for decision making. This can be achieved through a number of ways such as through nationally conducted censuses, malaria indicator surveys (MIS) nationally-representative surveys, and demographic health surveys (DHS). Depending on how detailed and invested these surveys are, they can obtain information about population demographics, household size, health, and other factors. The precision of surveys ultimately depends on its sample size, budget, and sample clusters and how often it is carried out. Certain types of surveys are more beneficial for malaria interventions. Through comparing these types of surveys, it seems that nationally-representative household surveys are better bases for estimating health metrics for the targeting of interventions.

Even after determining that nationally-representative household surveys are better than its alternatives, it still holds some doubts. Examining the effectiveness and precision of such surveys is very important because the data from these surveys often serve as the basis for data science analysis, and furthermore, healthcare interventions. Surveys are typically time-consuming, use a lot of resources and cost a lot of money, so examining them can lead to a survey-design which maximizes effectiveness. The potential harm outlined in this study is the errors that could be made by having incorrect sample sizes in the process of estimation of disease prevalence, specifically with examples of malaria in sub-Saharan Africa. This topic is significant because there is an increasing demand for reliable, high quality data to support decision-making and progress towards sustainable development goals, especially in low-middle income countries. Surveys are a good source of this data because they provide timely information with high resource availability. Nationally-representative surveys are the main source of data for establishing a scientific evidence base, monitoring disease, and evaluation of overall healthcare, but sometimes the surveys do not focus enough on the importance of defining indicator-relevant sample sizes to have high precision. All in all, there is a gap in the process of gathering data that should be further researched.

Usually after data has been gathered, whether it be a sufficient amount or not, or whether it be accurate or not, this data is used for estimations before these results are used in a map or model of higher resolution. The issue that is oftentimes faced is that surveys do not capture all areas, rather, it only takes into account a sample size that is then used to estimate an entire area of a region. An example of these statistical estimation methods is the random forest (RF) estimation method. Another example is using Bayesian statistical methods, Gaussian models, integrated nested Laplace approximations (INLA), or Markov chain Monte Carlo algorithms. Overall, in the context of malaria context, these statistical methods are used to estimate areas where malaria prevalence is concentrated, population density, population age-structure maps, covariates and their respective rankings, among other things.

After creating maps and models, the next step in this human development is to use this new information to strategize and design interventions. A specific example of how models are used was illustrated in the intervention program introduced in the Global Technical Strategy (GTS) by the Global Malaria Programme. In “Spatio-temporal analysis of malaria vector density from baseline through intervention in a high transmission setting” by Alegana et al., they explain how interventions can be designed to maximize its impact of malaria vectors by specifically assessing the effect of indoor residual spraying on malaria vector densities in area where the use of long-lasting insecticidal nets (LLINs) were high. This paper is of significance because understanding how to maximize the impact of interventions will save resources, time, and money. Interventions, such as the government-mass campaigns and government-initiated indoor residual spraying (IRS) campaigns, require a reliable scientific evidence basis, usually gathered by surveys and data-science methodological analyses. For example, in the study, they were able to establish seasonal peaks in malaria vector densities, and these pieces of data provide guidance for targeting IRS before peak transmission.



## Inquiry Type

This research question is evaluative as it assesses which method and intervention strategies have been most successful. My specific research question is: What is the most effective way of gathering and monitoring data for decision-making for malaria elimination in Nigeria? It looks into the demographics, such as age, and indicators as identified in malaria indicator surveys (MIS). This question is evaluative as it makes judgements about when are where intervention strategies should be implemented for maximum effectiveness.



## Methods

#### <u>Spatio-temporal model for estimation of mosquito densities</u> [3]

Taken from Alegana et. al., "Spatio-temporal analysis of malaria vector density from baseline through intervention in a high transmission setting," this method was conducted in high stable malaria intensity regions of eastern Sub-Saharan Africa such as Kenya and Uganda. These specific areas have the characteristics of two "wet" seasons where it experiences 1000-1500 mm of rainfall annually. The first wet season occurs from March to May, and the second from October to November. The average temperature of the day is 23 degrees celsius. These are just some of the climatic variables that contribute to the high contextuality of regions, and its importance to focus on specific covariates for estimation in these areas. All in all, this study aimed to map malaria vector densities across time, starting from before intervention, through intervention. Spatio-temporal models for mosquito density estimations are important for assessing interventions and desgining intervention strategies for the overall goal to improve health conditions across Sub-Saharan Africa.

**DATA SOURCE:** Entomologic data is first collected to form surveillance at household-level. Mosquitoes were gathered about once a month from selected households in a sampling frame which targeted children aged between 6 and 10 years. To collect mosquitoes, miniature CDC light traps were used. These traps were positioned under a LLIN (long lasting insecticidal net). Captured mosquitoes were then identified and counted. The most prominent mosquito vector species found were *An. gambiae (s.l.)* and *An. funestus (s.l.)*. 

**COVARIATES:** In addition to mosquito densities, climatic and environmental covariates were also incorporated such as climatic, topography, ecological, proxy measures of urbanicity, household density and distance to water sources. These covariates were checked or correlation by using a generalized linear regression model, with the use of *bestglm* package in R. To select the minimum amount of covariates, the Bayesian information criterion (BIC) was calculated for each covariate; only covariates with the lowest BIC would be selected to be regressed against mosquito counts and to ultimately estimate mosquito densities across the region.

**MODELLING:** To predict and create continuous maps of vector densities across the region, a Bayesian hierarchical generalised mixed model was used, incorporating spatial and temporal effects as well. First, mosquito counts were modelled as negative binomials using this formula: 

![](https://pbs.twimg.com/media/EV_7YwIWoAE5j6u?format=png&name=small)

The product of this formula was then used for the general mixed effect regression model using the following formula:

![](https://pbs.twimg.com/media/EV_7af1XQAEgpQJ?format=png&name=small)

combining covariates and spatial temporal effect. Overall, these results were used in the government indoor residual spraying (IRS) campaign (using cabamate bendiocarb) in 2014-15 in Uganda.

After the IRS campaign, the proportion of individuals using LLINs were included as a continuous variable, as well as a temporal effect of month. These were modelled with an autoregressive model. Next, these models were used in a Bayesian inference process that used the integrated nested Laplace approximations (INLA). Instead of using Markov chain Monte Carlo (MCMC) algorithms, INLA was used due to its computational advantages.

![](https://pbs.twimg.com/media/EV_7b8KWAAAM5_z?format=jpg&name=small)

![](https://pbs.twimg.com/media/EV_7dg7WsAAH8oi?format=jpg&name=small)

**RESULTS:** Major reductions of malaria densities occured where IRS (bendiocarb) was introduced with high coverage use of LLINs.

**VALIDATION AND ASSESSMENT:** The goodness-of-fits of the model were assed using deviance information criterion (DIC) and marginal likelihood. For validation, a subset dataset was created where 20 households were randomly selected from the original sample of households. Further validation utilised statistics including the correlation between predicted/observed vector densities, and RMSE (root mean square error).

![](https://pbs.twimg.com/media/EV_8kOVWoAInzjb?format=jpg&name=medium)

**ADVANTAGES:** Using this approach, the data scientists are able to quantify uncertainties of the parameters of interest and include missing data points (NAs).

**GAPS AND FURTHER RESEARCH:** This method and the data used for modelling only covered indoor biting malaria densities, further studies should explore outdoor biting as well. There was also a lack of empirical data for the movement of mosquitoes themselves from indoor to outdoor; this movement could result in micro-effects of malaria transmission. Further studies should also explore the effect of changing environment and interventions. A gap that was identified was that it is difficult to collect longitudinal data on insecticide residual activity. 



#### <u>Nationally Representative Household-Level Surveys and Bayesian MCMC Algorithm</u>  [2] 

The study mainly used to analyze nationally representative surveys is Alegana et. al. "Malaria prevalence metrics in low- and middle-income countries: an assessment of precision in nationally-representative surveys". In order to achieve the concerned sustainable development goal of improving health for all, it is important to invest in high quality data. The data collected must be trustworty, reliable, accurate, and detailed in order to stregnthen scientific basis for decision making. In many applications, nationally-representative sureys are the main source of data. In the case of malaria prevalence, the type of nationally-representative surveys conducted were Malaria Indicator Surveys (MIS) and demographic and health surveys (DHS).

**DATA SOURCE:** Data was taken from nationally-representative population-based household surveys: DHS and MIS. For data collection, 3 different indicator variables were identified only for children under 5 years of age: prevalence of fever in last 2 weeks, use of insecticide-treated bed nets (ITNs), and malaria test results from RDT (rapid diagnostic test). Along with each indicator, the dates and geographical coordinates were recorded for each cluster-sample. The surveys were conducted from 2007-2016 (*n*=20 surveys, 5839 clusters). The surveys were conducted across east, southeast, and west Africa (Nigeria). Survey households were selected randmonly per cluster (about 18-36 households per cluster).

**PROCESSING THE DATA:** The data was combined and processed through simple random spatial sampling at the cluster level. ARCGIS 10 was used for spatial random sampling (SRS). 30% subset samples, as well as 20% and 40%, was used for malaria prevalence estimation under SRS for the three indicators. The remaining 70% sample was used for simulation by utilising the Bayesian MCMC algorithm and generating survey effectiveness. This was then used to create posterior distrubution used for inference. The inferences includes summary statistics of the distribution of the cluster posterior variance, indicators, intra-class correlation coefficient (ICC), survey design effect (*deff*), and estimate of the effective sample size (ESS).

![](https://pbs.twimg.com/media/EV_88utX0AkmWLc?format=png&name=900x900)

**MODELLING:** The Bayesian hierarchical model was utilised with the MCMC algorithm. The JAGs version and *R2jags* package in R version was used. The ICC was estimated for total variability between- and within- clusters based on indicators, and adjusting for age, and survey domain stratification (urban/rural). An ICC of 0 indicates no correlation between/within clusters. To model household survey effectiveness parameters, the *deff* was modelled based on ICC estimates, which was then used to derive the optimal sample size. A *deff* close to 1 suggests similarity to simple random sampling.

![](https://pbs.twimg.com/media/EV_88vsXYAMQPAJ?format=jpg&name=large)

**RESULTS:** The ICC for the 3 indicators range from 0-0.05, where 0 indicates no correlation between reponses. Larger ICC values correlate to a larger prevalence. The ICC for ESS was plotted, showing a wide range as a result of different ESS. As seen from the analysis of malaria indicators and ESS, variability at cluster level actually has an impact on the desired sample size for that specific indicator.  

![](https://pbs.twimg.com/media/EV_88xEXQAUyqi2?format=jpg&name=large)

**GAPS AND FURTHER RESEARCH:** As seen in the results, cluster-level variability effects ESS. The problem emerges that this method requires large sample sizes to support monitoring efforts of interventions, but reduces with the increasing use of interventions. Contrastly, required sample size increases with declining prevalence of the indicator. Thus, defining sample sizes for different MIS will increase precision in detecting prevalence, and this must be researched further. This study further suggests to explore the use of biomarkers to optimize malaria surveys.

The precision of surveys ultimately depends on sample size, budget, reference sampling indicator, and indicator clustering. A problem is that size of surveys, meaning the number of clusters, is constrained by funding. Another issue is that parasitological testing is neccessary to distinguish fevers from other infections, thus funding for tests is always needed. Thus, this proves the point that these nationally-representative surveys must be well funded to be successful, which is often difficult for LMICs. An identified gap is that DHS and MIS requires a long fieldwork period, and its very expansive.



### Overview

The first methodology explored here was spatio-temporal modelling of mosquito densities. The second methodology was using nationally-representative household surveys to estimate/model clusters, indicators, and the effective sample size (ESS). Both of these methods utilised Bayesian hierarchical method to model their respective covariates. The Bayesian hierarchical method is shown to have accurate and reliable results, since it allows for the ability to quantify errors and uncertainties. Both methods conducted data collection at household levels. These methods compliment each other, and would likely be used in conjointly in detailed malaria elimination strategies.

As explored in the second method, there is an uncertainty and gap with household level surveys/collection methods, as variability between clusters actually leads to different requirements for the correct effective sample size. Taking a step back, this is a very relevant issue. Interventions for highly contextualized, highly heterogeneous regions are often evidence based, and rely of high precision, accurate, timely information. Determining the most effective survey method is the basis for successful models, and thus leading more effective health care (such as malaria elimination) interventions. Further studies in this area can improve health conditions for people in these regions faster, and overall reaching the sustainable health goals at a more timely pace.

2895 words


#### References

1. Strano, E., Viana, M.P., Sorichetta, A. *et al.* Mapping road network communities for guiding disease surveillance and control strategies. *Sci Rep* **8,** 4744 (2018). https://doi.org/10.1038/s41598-018-22969-4
2. Alegana, V.A., Wright, J., Bosco, C. *et al.* Malaria prevalence metrics in low- and middle-income countries: an assessment of precision in nationally-representative surveys. *Malar J* **16,** 475 (2017). https://doi.org/10.1186/s12936-017-2127-y
3. Alegana, V.A., Kigozi, S.P., Nankabirwa, J. et al. Spatio-temporal analysis of malaria vector density from baseline through intervention in a high transmission setting. Parasites Vectors 9, 637 (2016). https://doi.org/10.1186/s13071-016-1917-3
4. A. Wesolowski, et al. (October 12, 2012). Quantifying the Impact of Human Mobility on Malaria. Retrieved https://science.sciencemag.org/content/338/6104/267
5. Jr, R. C. R., Menach, A. L., Kunene, S., Ntshalintshali, N., Hsiang, M. S., Perkins, A., … Bryan Greenhouse. (2015, December 29). Mapping residual transmission for malaria elimination. Retrieved February 23, 2020, from https://elifesciences.org/articles/09520
6. V. A. Alegana, P. M. Atkinson, C. Pezzulo, A. Sorichetta, *et al.* (2015) Fine resolution mapping of population age-structures for health and development applications. Retrieved from https://royalsocietypublishing.org/doi/pdf/10.1098/rsif.2015.0073
