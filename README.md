
# TOPSIS-ShivamPundir-101803158
Submitted By: Shivam Pundir(101803158)

## What is TOPSIS?
Technique for Order Preference by Similarity to Ideal Solution (TOPSIS) originated in the 1980s as a multi-criteria decision making method. TOPSIS chooses the alternative of shortest Euclidean distance from the ideal solution, and greatest distance from the negative-ideal solution.
## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install **TOPSIS**.
Dependencies and devDependencies will be installed automatically.

```bash
pip install TOPSIS-ShivamPundir-101803158
```

## Usage
##### 1) As a Library:
Import in your python File:
```python
from TOPSIS import topsis
topsis()
```
Run the python file by typing in terminal/cmd:
```sh
python nameOfFile.py nameOfDataFile.csv "weights" "impacts" nameOfOutputFile.csv
```
##### 2) Using Command Promt:

Command line args:
- name of input File(csv format)
- weights(as a string)
- impacts(as a string)
- name of output file(csv format)
Eg. 
```bash
topsis data.csv "1,1,1,1" "+,+,-,+" output.csv
```

# Input file (data.csv)
The decision matrix should be constructed with each row representing a Model alternative, and each column representing a criterion like Accuracy, R2, Root Mean Squared Error, Correlation, and many more.
|Model|Corr|Rseq|RMSE|Accuracy|
|-----|----|----|----|--------|
|M1   |0.79|0.62|1.25|60.89   |
|M2   |0.66|0.44|2.89|63.07   |
|M3   |0.56|0.31|1.57|62.87   |
|M4   |0.82|0.67|2.68|70.19   |
|M5   |0.75|0.56|1.3 |80.39   |
Weights (`weights`) is not already normalised will be normalised later in the code.

Information of benefit positive(+) or negative(-) impact criteria should be provided in impacts.
# Output file (output.csv)
|Model|Corr|Rseq|RMSE|Accuracy|Topsis_score       |Rank|
|-----|----|----|----|--------|-------------------|----|
|M1   |0.79|0.62|1.25|60.89   |0.7722097345612788 |2   |
|M2   |0.66|0.44|2.89|63.07   |0.22559875426413367|5   |
|M3   |0.56|0.31|1.57|62.87   |0.43889731728018605|4   |
|M4   |0.82|0.67|2.68|70.19   |0.5238778712729114 |3   |
|M5   |0.75|0.56|1.3 |80.39   |0.8113887082429979 |1   |
The output file contains columns of input file along with two additional columns having **Topsis_score** and **Rank**
## License
[MIT](https://choosealicense.com/licenses/mit/)


  


