# THHCalculator

## Background
Thailand 30 year historical lottery data was downloaded from the internet. Extracted the winning numbers by digit place and put them into individual columns.

## Data
<p>Following are file names and a brief description.</p>

### 30Y_preproc.csv
<p>The file contains Day, Month, Year, and the winning numbers in separate columns. Each winning numbers was extracted according to its digit location and put into separate columns. For example, the number '123' in column '3ตัวบน' was extracted as:</p>
<ul>
  <li>'1' in column '3ตัวบน_100'</li>
  <li>'2' in column '3ตัวบน_10'</li>
  <li>'3' in column '3ตัวบน_1'</li>
</ul> 
<p><b>NOTE!!!</b> '2ตัวบน' and '2ตัวล่าง' also has the '_100' columns with '0' in them. PLEASE IGNORE '_100' columns from '2ตัวบน' and '2ตัวล่าง'.</p>

### 30Y_preproc_training.csv
<p>This is 90% of randomly selected rows from "30Y_preproc.csv". This file is intended to be used as a training file for the ML model. Note the unnamed first column can cross-reference to the first column rows of "30Y_preproc.csv" file.</p>

### 30Y_preproc_eval.csv
<p>This is 10% of remaining rows. Note the unnamed first column can cross-reference to the first column row of "30Y_preproc.csv" file.</p>

### 30Y_preproc.json
<p>This is the json format of the 30Y_preproc.csv.</p>

    
