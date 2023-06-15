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
import sys

path_input     = './Learn-You-a-Haskell-for-Great-Good!.txt'
path_normalize = './爱normalize.txt'
path_csv       = './爱csv.csv'


def generate():
  # Создание правильного csv файла

  file_input     = open(path_input,'r')
  file_normalize = open(path_normalize,'w')
  file_csv       = open(path_csv, 'w')


  file_string = file_input.read()
  file_string = file_string.replace('\n\n', '\n')

  file_normalize.write(file_string)

  file_string = file_string.replace('"', '""')
  file_string = '"' + file_string.replace('\n', '"\n"') + '"'

  file_csv.write(file_string)


  # Закрытие файлов

  file_input.close()
  file_normalize.close()
  file_csv.close()

// Разбиение файла на ровные отрезки по x, причем последний может быть неполным
def generate_parts_excel():
  csvfile = open(path_csv, 'r').readlines()
  rows = 2500
  filename = 1
  for i in range(len(csvfile)):
    if i % rows == 0:
      csv_number = str(filename)
      
      file = open(f"./csv-{csv_number}.csv", 'w+')
      file.writelines(csvfile[i:i+rows])
      file.close()

      file_csv = open(f"./csv-{csv_number}.csv", 'r')

      # Создание частей Excel файла
      df = pd.read_csv(file_csv, sep=',')
      df.to_excel(f"./xlsx-{csv_number}.xlsx", 'Ave Maria! Deus Vult!', index = None, header=True)

      file_csv.close()

      filename += 1


def generate_excel():
  csvfile = open(path_csv, 'r')

  # Создание полного Excel файла
  df = pd.read_csv(csvfile, sep=',')
  df.to_excel(f"./full.xlsx", 'Ave Maria! Deus Vult!', index = None, header=True)

  csvfile.close()


generate()
generate_excel()
```
