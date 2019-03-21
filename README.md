# Haberman’s Cancer Survival: Visual Exploratory Data Analysis using Python
Exploratory Data Analysis (EDA) is the series of asking questions and applying statistics and visualization techniques to answer those questions and to uncover the hidden insights from the data. A case study on the cancer survival data set is done to explore the most common EDA techniques in this blog.
<br>
<h1>Data Description</h1>
The Haberman’s survival data set contains cases from a study that was conducted between 1958 and 1970 at the University of Chicago’s Billings Hospital on the survival of patients who had undergone surgery for breast cancer.
<br>
<h2>Attribute Information:</h2>
<pre>
1.Age of patient at time of operation (numerical)
2.Patient’s year of operation (year — 1900, numerical)
3.Number of positive auxillary nodes detected (numerical)
4.Survival status (class attribute) 1 = the patient survived 5 years or longer 2 = the patient died within 5 years
</pre>
Setting the objective is the key in EDA which will structure your thoughts in the entire analysis. Here the objective is to predict whether the patient will survive after 5 years or not based upon the patient’s age, year of treatment and the number of positive lymph nodes.
<h2>
1. Environment Configuration
Import the required packages and load the data set.</h2>

```
import seaborn as sns
import numpy as np
import matplotlib.pyplot as plt
import pandas as pd
import warnings
warnings.filterwarnings("ignore")
```
<p>Density Plot</p>

```
sns.jointplot(data=df, x="Age",y="Year of Operations", kind="kde")
plt.ylabel("Cancer")
plt.show()
```
