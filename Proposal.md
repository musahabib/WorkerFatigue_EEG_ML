# MANU 465 Project - Proposal

** to delete **
Please upload a 1-2 page project proposal, clearly state motivation for choosing this project, the goal in this project (what you wish to achieve), a brief plan and steps to complete this project, and the potential ML algorithm you think, you may use. Suppose you are writing this proposal for a company that asks you to do a data analyses & ML project for them; so you need to show them clearly what is your approach and plan to successfully complete this project. (Only the project's Liaison needs to submit.)

## Authors

|       Name      | Student ID |
|:---------------:|:----------:|
|   Anant Goyal   |  46894325  |
| Alberto Mussali |  50684182  |
|    Musa Habib   |  25899808  |
| Sadul Bombuwala |  76343292  |


## Motivation
To get wasted lmao 420 BLAZE


## Objective and Goals



## Methods

### Features

MindMonitor (MM) allows us to record and extract the following features in a .csv format.

|         Features         | Description                                                            | Range / Units                                 |
|:------------------------:|------------------------------------------------------------------------|-----------------------------------------------|
|         TimeStamp        | Date and Time                                                          | Year-Month-Day Hour:Minute:Second.Microsecond |
| Delta_{TP9,AF7,AF8,TP10} | Delta brainwaves, for each of the four sensors                         | Bels                                          |
| Theta_{TP9,AF7,AF8,TP10} | Theta brainwaves, for each of the four sensors                         | Bels                                          |
| Alpha_{TP9,AF7,AF8,TP10} | Alpha brainwaves, for each of the four sensors                         | Bels                                          |
|  Beta_{TP9,AF7,AF8,TP10} | Beta brainwaves, for each of the four sensors                          | Bels                                          |
| Gamma_{TP9,AF7,AF8,TP10} | Gamma brainwaves, for each of the four sensors                         | Bels                                          |
|  RAW_{TP9,AF7,AF8,TP10}  | RAW brainwaves, for each of the four sensors                           | 0.0 - 1682.815 uV                             |
|         AUX_RIGHT        | RAW brainwaves for the auxiliary USB sensor (not available with MU-01) | 0.0 - 1682.815 uV                             |
|   Accelerometer_{X,Y,Z}  | Gravity. X = tilt up/down, Y = tilt left/right, Z = vertical up/down   | g {-2:+2}                                     |
|       Gyro_{X,Y,Z}       | Gyroscope motion over time (returns to zero)                           | degrees/second {-245:+245}                    |
|        HeadBandOn        | Basic data quality indicator: if the headband is on the head           | 1=True, 0=False                               |
|  HSI_{TP9,AF7,AF8,TP10}  | Data quality, for each of the four sensors (HSI=Horse Shoe Indicator)  | 1=Good, 2=Medium, 4=Bad                       |
|          Battery         | Battery charge percentage                                              | %/100                                         |
|         Elements         | Data markers such as Blink, Jaw_Clench, or numbered markers            | various                                     |
    
Additionally, more features can be engineered in order to provide the ML algorithms with more information. The relative band power, for example, is commonly used in literature. (see [this article](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4712412/), for example.)


    The relative band powers are calculated by dividing the absolute linear-scale power in one band over the sum of the absolute linear-scale powers in all bands. The linear-scale band power can be calculated from the log-scale band power thusly: linear-scale band power = 10^ (log-scale band power).
Retrieved from: [Muse Developer Documentation](https://web.archive.org/web/20181105231756/http://developer.choosemuse.com/tools/available-data#Relative_Band_Powers)

Thus,

$$ \alpha_r = (10^{\alpha_a}) / (10^{\alpha_a} + 10^{\beta_a} + 10^{\delta} + 10^{\gamma_a} + 10^{\theta})) $$







### Models


## Project Plan



## More?

