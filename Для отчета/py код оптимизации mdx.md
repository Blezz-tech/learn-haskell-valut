```bash
pip install beautifulsoup4
pip install lxml
```

```python
from bs4 import BeautifulSoup

path_source = './source/MT_Yandex_en-ru_Learn-You-a-Haskell-for-Great-Good.tmx'
path_dist = './dist/out.tmx'

with open(path_source, "r", encoding="utf-8") as xml_file:
  xml_string = xml_file.read()
  print("Файл прочитан")

  soup = BeautifulSoup(xml_string, 'xml')

  translate_count = 0

  for tu in soup.find_all('tu'):
    segments = tu.find_all('seg')
    if (segments[0].get_text() == '' and segments[1].get_text() == ''):
      translate_count = translate_count + 1
      tu.decompose()
  
  print("Строк с пустым переводом:", translate_count)

  with open(path_dist, "w", encoding="utf-8") as fd:
    out = soup.prettify()
    fd.write(out)
    print("Файл записан")
```