```bash
pip install pandas
pip install openpyxl
pip install xlrd
```

```python
# pip install pandas
# pip install openpyxl
# pip install xlrd

import pandas as pd

path_input =  './Learn-You-a-Haskell-for-Great-Good.txt'
path_output = './Learn-You-a-Haskell-for-Great-Good.xlsx'
path_tmp =    './tmp.csv'

# Создание правильного csv файла
file_input = open(path_input,'r')
file_tmp   = open(path_tmp,'w')

file_string = file_input.read()
file_string = file_string.replace('\n\n', '\n')
file_string = file_string.replace('"', '""')
file_string = '"' + file_string.replace('\n', '"\n"') + '"'
file_tmp.write(file_string)

file_input.close()
file_tmp.close()

# Создание Excel файла
df = pd.read_csv(path_tmp, sep=',')
df.to_excel(path_output, 'Ave Maria! Deus Vult!', index = None, header=True)
```
