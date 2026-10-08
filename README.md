# MexEE 402: Data Preprocessing Case Study

**MexEE Elective 2: Data Science and Machine Learning**
Department of Electronics Engineering, College of Engineering
Batangas State University, The National Engineering University, Alangilan Campus

1st Semester, AY 2026-2027

> **Deadline: Friday, October 9, 2026, before 5:00 PM.**

---

## 1. What you will do

You were given the Chapter 1 to 9 Google Colaboratory notebooks for this course. Your task is to:

1. Save your own copy of each notebook.
2. Run it, edit it, and answer the questions for that chapter inside the notebook.
3. Build one GitHub repository that holds a README.md with the links to all your notebooks.

You are not building new notebooks. You are working inside mine. Run the cells, change them where the questions ask you to, and write what you understood.

This is your Data Preprocessing Case Study, worth **25% of your final grade**.

---

## 2. Working in pairs

You already have your pair. Work with that partner only.

- **One repository per pair.** Either member can create it.
- **Each member keeps their own Colab copies.** Do not share one copy between you. I need to see both of you working.
- Both members must commit to the repository. A member with zero commits gets no grade.
- Split the chapters however you like, but both of you must be able to explain all seven notebooks. I will pick who answers.

---

## 3. Setting up your Colab notebooks

For each of the seven notebooks:

1. Open my notebook link.
2. Click **File, then Save a copy in Drive.**
3. Rename your copy like this:
   ```
   Ch4_Surname1_Surname2
   ```
4. Click **Share, then General access, then Anyone with the link, then Viewer.** If I cannot open it, it is not submitted.
5. Do your edits and write your answers in that copy.
6. Before you submit, click **Runtime, then Restart session and run all.** If it crashes, fix it.

The seven notebooks:

| Notebook | Topic |
|---|---|
| Ch1_2_3 | Introduction to preprocessing, exploring and cleaning data |
| Ch4 | Transformation, feature engineering, and encoding |
| Ch5 | Scaling and normalization |
| Ch6 | Outlier detection |
| Ch7 | Feature selection |
| Ch8 | Constructing a preprocessing pipeline |
| Ch9 | Full pipeline and visualization |

---

## 4. How to answer the questions

The questions are in Section 7. For every chapter:

- Add a **new markdown cell at the end of the notebook** titled `## Chapter Questions`.
- Write the question, then your answer under it.
- **Two to four sentences per answer.** Short and clear is better than long.
- If a question asks you to run something, add a code cell and run it. Put the actual number you got in your answer.
- If a question asks you to change something, change the cell, run it, and say in one line what you changed.

Answers copied from a classmate, or pasted from an AI tool without understanding, earn zero for that chapter. I will ask you to explain your own sentences.

---

## 5. Your GitHub repository

Name it:

```
<Surname1>_<Surname2>_MexEE402_CaseStudy
```

Example: `Reyes_Santos_MexEE402_CaseStudy`

Set it to **Public**. It needs only one file:

```
Reyes_Santos_MexEE402_CaseStudy/
└── README.md
```

No notebook files, no datasets. Just the README with your links.

---

## 6. Template for your README.md

Copy this, fill it in, and push it:

```markdown
# MexEE 402: Data Preprocessing Case Study

MexEE Elective 2: Data Science and Machine Learning
Batangas State University, Alangilan Campus
1st Semester, AY 2026-2027

## Members

| Name | Student Number | Section |
|---|---|---|
| Surname, First Name | | |
| Surname, First Name | | |

## Notebook links

| Chapter | Member 1 | Member 2 |
|---|---|---|
| Ch1_2_3 | [link]() | [link]() |
| Ch4 | [link]() | [link]() |
| Ch5 | [link]() | [link]() |
| Ch6 | [link]() | [link]() |
| Ch7 | [link]() | [link]() |
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
```

---

## 7. Chapter questions

### Chapter 1, 2, 3: Exploring and cleaning data

1. What is data preprocessing, and why do we do it before machine learning?
2. What does each of these show you: `head()`, `info()`, and `describe()`?
3. Which columns in the dataset had missing values? How many were missing in each?
4. The notebook showed two ways to handle missing data. Name both, and say when you would use each.
5. Why was the `Rank` column dropped from the dataset?

### Chapter 4: Feature engineering and encoding

1. What is feature engineering, in your own words?
2. How was `Lemonade per Degree` computed, and what does it tell you about the sales?
3. What is binning? List the four temperature labels used in the notebook.
4. What is an interaction feature? Give the example from the notebook.
5. What is the difference between one-hot encoding and ordinal encoding?
6. Why does ordinal encoding fit `Little`, `Medium`, `Lots`, while `Sunny`, `Cloudy`, `Rainy` needs one-hot?

### Chapter 5: Scaling and normalization

1. What is data scaling, and what problem does it solve?
2. What does `StandardScaler` do to the mean and the standard deviation of a column?
3. What range of values does `MinMaxScaler` give you?
4. In the student example, which column had the bigger numbers? Why does that matter to a model?
5. Is scaling always needed? What does the answer depend on?

### Chapter 6: Outlier detection

1. What is an outlier?
2. How does the Z-score method find outliers? What cutoff did the notebook use?
3. How does the IQR method find outliers? Write the formula for the lower and upper fence.
4. In the sample data, which value stands out from the rest? What is its Z-score?
5. Once you find an outlier, give two things you can do about it.

### Chapter 7: Feature selection

1. What is feature selection, and why is it useful?
2. What does the filter method use to decide which features to keep?
3. What does `RFECV` do, step by step?
4. What does `LassoCV` do to features that are not important?
5. Which features did each of the three methods choose? Put them in a short table.

### Chapter 8: Constructing a preprocessing pipeline

1. What is a preprocessing pipeline? Explain it using the conveyor belt idea from the notebook.
2. The notebook gives three reasons for using a pipeline. Name all three.
3. What two steps were inside the pipeline, and in what order did they run?
4. What does `ColumnTransformer` do?
5. Which two columns of the Titanic dataset were preprocessed in this chapter?

### Chapter 9: Full pipeline and visualization

1. Which columns were handled as numerical, and which as categorical?
2. How were the missing values filled in each of those two groups?
3. What is discretization? What three age labels did the notebook use, and what age ranges do they cover?
4. Name three of the plots you produced, and say in one sentence what each one shows.
5. Why is it useful to make plots after preprocessing instead of before?

---

## 8. Submission

1. Push your README.md to GitHub. Your last commit before the deadline is what I grade.
2. Submit **only the repository link** on the class page.
3. Check that every Colab link is set to **Anyone with the link, Viewer** before you submit. A link I cannot open counts as a missing notebook.

**Deadline: Friday, October 9, 2026, 5:00 PM.** Late work loses 10 points per day. The page closes Monday.

Be ready to defend your work in class. I will ask either member about any chapter.

---


Deductions:

- A notebook that will not run from a restarted session: **minus 5** each.
- A Colab link I cannot open: **minus 5** each.
- An answer with no number in it where the question asked for one: **minus 2** each.

---

## 9. Honesty

You may use AI tools to help you understand a method or fix an error. You may not submit an answer you cannot explain.

I will ask you to explain your own sentences. If you cannot, that chapter earns zero, whatever is written in it. Say in your README where you used an AI tool and what for. That is good practice, not a penalty.

Copying another pair's answers is academic dishonesty and goes to the department.

---

*Prepared by Engr. Mikko De Torres, Department of Electronics Engineering*
