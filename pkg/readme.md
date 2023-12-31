## Topsis:-MULTIPLE-CRITERIA DECISION MAKING

# TOPSIS

Submitted By: **BANDHAN SHER SINGH 102003440**.

Date: **23-JAN-2023**.

Description: **Evaluation of alternatives based on multiple criteria using TOPSIS method.**.

---

## What is TOPSIS?

**T**echnique for **O**rder **P**reference by **S**imilarity to **I**deal **S**olution
TOPSIS chooses the alternative of shortest Euclidean distance from the ideal solution,
and greatest distance from the negative-ideal solution.

<br>

## How to install this package:

```
>>pip install Topsis_Bandhan_102003440
```

### In Command Prompt

```
>> topsis data.csv "1,1,1,2,1" "+,+,-,+,-" result.csv
```

## Input file (data.csv)

The decision matrix should be constructed with each row representing a Model alternative, and each column representing a criterion like Attribute, Price or cost, Storage Space ,Camera,Looks.

| Fund Name | P1   | P2   | P3  | P4   | P5    |
| --------- | ---- | ---- | --- | ---- | ----- |
| M1        | 0.67 | 0.45 | 6.4 | 64.2 | 17.93 |
| M2        | 0.78 | 0.61 | 5.1 | 42.5 | 12.25 |
| M3        | 0.66 | 0.44 | 6.7 | 58.5 | 16.58 |
| M4        | 0.68 | 0.46 | 3.6 | 40.7 | 11.36 |
| M5        | 0.83 | 0.69 | 6.8 | 33   | 10.33 |
| M6        | 0.95 | 0.9  | 5.7 | 36.9 | 11.11 |
| M7        | 0.95 | 0.9  | 3.5 | 51.2 | 14.14 |
| M8        | 0.89 | 0.79 | 4.1 | 60.1 | 16.47 |

Weights (`weights`) is not already normalised will be normalised later in the code.

Information of benefit positive(+) or negative(-) impact criteria should be provided in `impacts`.

<br>

## Output file (result.csv)

| Fund Name | P1   | P2   | P3  | P4   | P5    | Topsis Score | Rank |
| --------- | ---- | ---- | --- | ---- | ----- | ------------ | ---- |
| M1        | 0.67 | 0.45 | 6.4 | 64.2 | 17.93 | 0.541        | 3    |
| M2        | 0.78 | 0.61 | 5.1 | 42.5 | 12.25 | 0.401        | 7    |
| M3        | 0.66 | 0.44 | 6.7 | 58.5 | 16.58 | 0.486        | 4    |
| M4        | 0.68 | 0.46 | 3.6 | 40.7 | 11.36 | 0.405        | 6    |
| M5        | 0.83 | 0.69 | 6.8 | 33   | 10.33 | 0.323        | 8    |
| M6        | 0.95 | 0.9  | 5.7 | 36.9 | 11.11 | 0.445        | 5    |
| M7        | 0.95 | 0.9  | 3.5 | 51.2 | 14.14 | 0.679        | 2    |
| M8        | 0.89 | 0.79 | 4.1 | 60.1 | 16.47 | 0.723        | 1    |

<br>
The output file contains columns of input file along with two additional columns having **Topsis_score** and **Rank**
