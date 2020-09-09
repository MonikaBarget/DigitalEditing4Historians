# XML as a basis for systematic text analysis / distant reading

# Xpath and XQuery

[Anderson, Clifford B., und Joseph C. Wicentowski. XQuery for Humanists. College Station, UNITED STATES: Texas A&M University Press, 2020](http://ebookcentral.proquest.com/lib/senc/detail.action?docID=6177763)

[Lai, Catherine, und Steven Bird. „Querying Linguistic Trees“. Journal of Logic, Language, and Information 19, Nr. 1 (2010): 53–73.](https://www.jstor.org/stable/20685004)

# XML analysis with programming languages such as Python

[Monika Barget, "Doing Digital History with Python I: reading (messy) XML & JSON data," in Digital Humanities Lab, 30/04/2020](https://dhlab.hypotheses.org/1406)

e.g. [ReadXML_titles_withBeautifulSoup.py](https://github.com/MonikaBarget/DigitalHistory/blob/master/ReadXML_titles_withBeautifulSoup.py)

```
#!/usr/bin/env python
# coding: utf-8

from bs4 import BeautifulSoup
import os
from os.path import dirname, join
directory=("C:\\Users\\mbarg\\Documents\\corpus") # location of XML files on local drive

results=[] # create result list
for infile in os.listdir(directory):
    filename=join(directory, infile)
    indata=open(filename,"r", encoding="utf-8", errors="ignore") # UTF-8 encoding errors are ignored
    contents = indata.read()
    soup = BeautifulSoup(contents,'xml')
    titles = soup.find_all('title') # get item titles
    for title in titles:
        print(title.get_text())
        results.append(title.get_text())
print(results) # result list is shown on screen
```
