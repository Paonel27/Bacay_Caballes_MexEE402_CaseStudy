# MexEE 402: Data Preprocessing Case Study

MexEE Elective 2: Data Science and Machine Learning
Batangas State University, Alangilan Campus
1st Semester, AY 2026-2027

## Members

| Name | Student Number | Section |
|---|---|---|
| Bacay, Jonel Andrey A.| 22-05567 | Mexe- 4103 |
| Caballes, Lois Eduard U. | 22-09062 | Mexe- 4103 |

## Notebook links-

| Chapter | Member 1 | Member 2 |
|---|---|---|
| Ch1_2_3 | [link]() |https://colab.research.google.com/drive/1byao2_RiVkra4b956uTP09dBOWqkUjOD?usp=sharing |
| Ch4 | [link]() | (https://colab.research.google.com/drive/1ikGCJhAvy4EYVWpNkv1Cv1dpTzLcJcFc?usp=sharing) |
| Ch5 | [link]() |[ (https://colab.research.google.com/drive/1WkjPMPjNl8oTorq9Qkq4AA3GK9_sCsBD?usp=sharing) |
| Ch6 | https://colab.research.google.com/drive/1rYD2e6XiJD0lR01ltOBGQ-4ICTOg_4Qs?usp=sharing | (https://colab.research.google.com/drive/1bahHdDkbV5rvAoTJLnsDNucLC3CPWoDe?usp=sharing) |
| Ch7 | https://colab.research.google.com/drive/1yI0Yy97TNqhJSK35DYRaRWwGpBo8b_2I?usp=sharing | [link]() |
| Ch8 | https://colab.research.google.com/drive/15-30HfX9-oVz89U-S3fXA0gZSumDqW1I?usp=sharing | [link]() |
| Ch9 | https://colab.research.google.com/drive/1iQmSlDMHwVhFpR4UNTDZkVDEtHgMpf2u?usp=sharing | [link]() |

## What we learned
In Chapter 1-3, these lessons taught me that preparing data properly makes machine learning more accurate and reliable. It showed me that even small details, like missing values or unnecessary columns, can affect the results. I now appreciate that preprocessing is not just a step, but a foundation for good analysis.

In Chapter 4, these lessons showed me that preparing and transforming data is not just about cleaning—it’s about making the data smarter, so the model can understand it better. It taught me that the way we represent information can change how well the model sees patterns and makes predictions

In chapter 5, these lessons showed me that scaling is a way to make data fairer and more balanced. It taught me that choosing the right scaling method can help the model focus on what really matters, instead of being misled by the size of the numbers.

In chapter 6, we thought an outlier was just a mistake to be deleted. But I realized an outlier is simply a data point that lives far away from its peers. Sometimes it’s a sensor glitch or a typo which should be removed or capped but it can be useful sometimes so don't remove it always.

In chapter 7, our biggest conceptual takeaway is that feature selection isn't just about deleting unnecessary columns; it is about balancing quality, efficiency, and model performance. Having more data columns does not automatically make a machine learning model smarter, because irrelevant or highly redundant features introduce noise, slow down algorithms, and can ultimately degrade accuracy. 

In chapter 8, we learned that the central focus shifts from individual data-cleaning techniques to building a structured software pipeline that automates raw data transformation. Using the notebook's conveyor belt analogy, a data preprocessing pipeline passes raw features through a sequence of automated operations such as handling missing values or adjusting scales so that clean, standardized data exits at the end ready for machine learning models. 

In Chapter 9, we learned that data preprocessing is an important step before performing data analysis or developing a machine learning model. Before studying this chapter, we might have thought that having a dataset was enough to begin analyzing information. However, we realized that the quality of the data affects how accurately we can interpret results and discover meaningful patterns. 


## Errors we found
We found an error in chapter 6 were the code in calculating the outliers is not working properly because the set cutoff in the code is 3 while the maximum z-scores in the data set is 2.615 so we change the threshold value into 2.5

## Note on AI tools

We use AI tools in chapter 6 to fix the code in calculating outliers because the cutoff in the code is set to 3 while the maximum z- score in the dataset is 2.615. Since the 2.615 is less than 3, the code evaluates the condition as false. 

I(Bacay) personally use Gemini to discuss the things that are not clear to me in doing the chapter 6 to 9 specifically in understanding the RFECV and LassoCV.

I(Caballes) personally use Copilot, it helps me to understand, and to construct my answers for the entire chapter 1-5, especially 4 and 5.
## References

McKinney, W. (2021). Python for Data Analysis, 3rd ed. O'Reilly.
VanderPlas, J. Python Data Science Handbook.
Any other page or article you used.


