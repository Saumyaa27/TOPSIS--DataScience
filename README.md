This is a command line program to implement the TOPSIS.
# TOPSIS-Python

**Subject : UCS538**
Assignment 6


Submitted By: **Saumyaa Mathur 101803609**

***

## What is TOPSIS

The Technique for Order of Preference by Similarity to Ideal Solution is a multi-criteria decision analysis method.It is a method of compensatory aggregation that compares a set of alternatives by identifying weights for each criterion, normalising scores for each criterion and calculating the geometric distance between each alternative and the ideal alternative, which is the best score in each criterion

<br>

## How to use this package:

TOPSIS-Saumyaa 101803609 can be run as in the following example:

Usages:
python topsis.py <InputDataFile> <Weights> <Impacts> <ResultFileName>
Example:
python topsis.py inputfile.csv “1,1,1,2” “+,+,-,+” result

### In Command Prompt
```
>> topsis data.csv "1,1,1,1" "+,+,-,+" result
```
<br>

### In Python IDLE:

topsis('data.csv','1,1,2,2','+,+,-,+','result')

<br>

## Sample dataset (.csv)

	Model	Corr	Rseq	RMSE	Accuracy
0	M1	0.79	0.62	1.25	60.89
1	M2	0.66	0.44	2.89	63.07
2	M3	0.56	0.31	1.57	62.87
3	M4	0.82	0.67	2.68	70.19
4	M5	0.75	0.56	1.30	80.39

Information of benefit positive(+) or negative(-) impact criteria should be provided in `I`.

<br>

## Output file (.csv)

  Model  Corr  Rseq  RMSE  Accuracy TOPSIS score  Rank
0    M1  0.79  0.62  1.25     60.89      0.77221   2.0
1    M2  0.66  0.44  2.89     63.07     0.225599   5.0
2    M3  0.56  0.31  1.57     62.87     0.438897   4.0
3    M4  0.82  0.67  2.68     70.19     0.523878   3.0
4    M5  0.75  0.56  1.30     80.39     0.811389   1.0

<br>
