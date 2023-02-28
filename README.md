# Apriori-Algorithm

Given a input DB, mining strong association rules from the input DB with user-defined min_supp and min_conf.

- [x] User-defined min_supp
- [x] User-defined min_conf
[Click to read the code]([Apriori_Algorithm.ipynb](https://github.com/podo47/Apriori-Algorithm/blob/11725ce7104d60b86da8c05899c463a850309b93/Apriori_Algorithm.ipynb))

## 1.Import library
``` python
from itertools import combinations
import csv
from collections import Counter
import pandas as pd
```

## 2.Run Apriori Algorithm

**Part 1 : Function**
- [x] Calculate support
- [x] Calculate confidence
- [x] Answer form
- [x] Main : Apriori algorithm

**Part 2 : Apriori Algorithm**
* Input file preprocessing
  * Read input
  * Modify input format and store in list
* Output 
## 3. Output:"output.csv"
| Rule:left       | → | Rule:right | Confidence           |
|-----------------|---|------------|----------------------|
| 32              | → | 38         | 0.18678710358014108  |
| 32              | → | 39         | 0.5574602755983386   |
| 32              | → | 41         | 0.2107206435023406   |
| 32              | → | 48         | 0.5297026438979363   |
| ...             | → | ...        | ... |
| "{48, 41, 38}"  | → | 39         | 0.8386689132266217   |
| "{48, 170, 38}" | → | 39         | 0.7756827048114434   |
| "{48, 110, 38}" | → | 39         | 0.7575312270389419   |
| "{48, 41, 39}"  | → | 32         | 0.22345913657344557  |
| "{48, 41, 39}"  | → | 38         | 0.2702959543850122   |
| "{48, 170, 39}" | → | 38         | 0.9892205638474295   |
| "{48, 110, 39}" | → | 38         | 0.9942140790742526   |

