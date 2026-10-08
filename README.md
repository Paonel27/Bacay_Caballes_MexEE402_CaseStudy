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
| Ch4 | [link]() | [[link]()](https://colab.research.google.com/drive/1ikGCJhAvy4EYVWpNkv1Cv1dpTzLcJcFc?usp=sharing) |
| Ch5 | [link]() |[ [link]()](https://colab.research.google.com/drive/1WkjPMPjNl8oTorq9Qkq4AA3GK9_sCsBD?usp=sharing) |
| Ch6 | https://colab.research.google.com/drive/1rYD2e6XiJD0lR01ltOBGQ-4ICTOg_4Qs?usp=sharing | [[link]()](https://colab.research.google.com/drive/1bahHdDkbV5rvAoTJLnsDNucLC3CPWoDe?usp=sharing) |
| Ch7 | https://colab.research.google.com/drive/1yI0Yy97TNqhJSK35DYRaRWwGpBo8b_2I?usp=sharing | [link]() |
| Ch8 | [link]() | [link]() |
| Ch9 | [link]() | [link]() |

## What we learned

One short paragraph per chapter, Ch1_2_3 to Ch9. Say what the chapter taught
you and what surprised you. Not what the library does, but what you understood.

## Errors we found

List any mistake you found in the original notebooks, and the correct version.
There are real ones in there. Finding them earns points.

## Note on AI tools

Say whether you used an AI tool, and what for. This is not a penalty.
Hiding it is.

## References

McKinney, W. (2021). Python for Data Analysis, 3rd ed. O'Reilly.
VanderPlas, J. Python Data Science Handbook.
Any other page or article you used.

## Chapter 1_2_3 Questions:
1. What is data preprocessing, and why do we do it before machine learning?
- Data preprocessing is the step where we clean and organize raw data before using it. We do it because raw data is often messy, incomplete, or inconsistent. Preprocessing makes the data reliable, improves model accuracy, and saves time and resources later.

2. What does each of these show you: head(), info(), and describe()?
- The functions head(), info(), and describe() are useful tools when working with datasets. The head() function lets you quickly view the first few rows so you can get an idea of how the data looks. The info() function provides details about each column, such as the type of data stored and whether there are missing values. Meanwhile, the describe() function gives a statistical summary of the numeric columns, including values like the mean, minimum, and maximum, which helps you understand the overall distribution of the data.

3. Which columns in the dataset had missing values? How many were missing in each?
- In the dataset, there were missing values in two columns. The Year column had the largest number of missing entries, with a total of 271 values not recorded. Meanwhile, the Publisher column also had incomplete data, with 58 values missing. This shows that both columns had gaps, but the Year column was affected more heavily compared to Publisher.

4. The notebook showed two ways to handle missing data. Name both, and say when you would use each.
- 	Imputation which fill missing values with mean, median, or mode. Use this when you want to keep all rows and the missing data is not too large.
- Deletion which remove rows or columns with missing values. Use this when only a small portion is missing and deleting won’t affect the dataset much.

5. Why was the Rank column dropped from the dataset?
- The Rank column was removed because it doesn’t add useful information for analysis or prediction. It’s just an ordering number, so keeping it would only add noise.

## Chapter 4 Questions:
1. What is feature engineering, in your own words?
- It’s the process of creating new useful data from existing data so that a machine learning model can understand patterns better.

2. How was Lemonade per Degree computed, and what does it tell you about the sales?
- It was calculated by dividing the number of lemonades sold by the temperature. It shows how many lemonades are sold for each degree of heat, helping us see the relationship between sales and temperature.

3. What is binning? List the four temperature labels used in the notebook.
- Binning means grouping numbers into categories. The four labels used were: cool, warm, hot, very hot.

4. What is an interaction feature? Give the example from the notebook.
- An interaction feature is just a new data point made by combining two existing ones. In simple words, it’s like mixing two pieces of information to see how they work together. For example, Ice Cubes per Degree was made by dividing the number of ice cubes by the temperature. This shows how many ice cubes are used for each degree of heat. It helps us understand the relationship between the two factors more clearly.

5. What is the difference between one-hot encoding and ordinal encoding?
- In one-hot encoding, each category gets its own column, and the values are marked as 1 or 0 (yes or no). In ordinal encoding, categories are given numbers based on order, like 0, 1, 2. In simple words, one-hot encoding is like making separate boxes for each category, while ordinal encoding is like putting them in a ranked list with numbers.

6. Why does ordinal encoding fit Little, Medium, Lots, while Sunny, Cloudy, Rainy needs one-hot?
-  Because Little, Medium, Lots have a natural order (small, medium, large). But Sunny, Cloudy, Rainy don’t have an order, so they need one-hot encoding to avoid giving them false ranking.

## Chapter 5 Questions:
1. What is data scaling, and what problem does it solve?
- Data scaling means making the numbers in your dataset more balanced so they can be compared fairly. In simple words, sometimes one column has very big numbers while another has small ones. If we don’t adjust them, the big numbers can control the model’s decisions, even if the small ones are important. Scaling fixes this by putting the values into similar ranges, so every column has a fair chance to affect the result. It’s like making sure no one’s voice is too loud or too soft in a group discussion.

2. What does StandardScaler do to the mean and the standard deviation of a column?
- StandardScaler is a tool that changes the numbers in a dataset so they are easier to compare. In simple words, it makes the average value (mean) of a column become 0, and the spread of the numbers (standard deviation) become 1. This means the data is centered around zero and spread out evenly. By doing this, no column has numbers that are too big or too small compared to others, so the model can treat all features fairly. It’s like resetting the scale so everything starts from the same point and has the same balance.

3. What range of values does MinMaxScaler give you?
- MinMaxScaler transforms values into the range 0 to 1. The lowest value becomes 0, highest becomes 1, and everything else is scaled in between. It squeezes all values between 0 and 1.

4. In the student example, which column had the bigger numbers? Why does that matter to a model?
- The Grades column had bigger numbers (0–100 vs. Study Hours 0–20). This matters because without scaling, the model might give more weight to Grades just because the values are larger, not because they are more important. In the student data, Grades had bigger numbers (up to 100). That matters because the model might think Grades are more important just because they’re larger.

5. Is scaling always needed? What does the answer depend on?
- Scaling is not always required. It depends on the algorithm (e.g., distance based models like k NN, SVM, or gradient descent benefit from scaling). The nature of the data (if ranges are already similar, scaling may not add value). In short, scaling is not always needed. It depends on the algorithm and the nature of the data. 

