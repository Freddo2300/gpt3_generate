---
jupyter:
  jupytext:
    formats: ipynb,md
    text_representation:
      extension: .md
      format_name: markdown
      format_version: '1.3'
      jupytext_version: 1.13.1
  kernelspec:
    display_name: Python 3
    language: python
    name: python3
---

```python
import openai
import os
from dotenv import load_dotenv
```

```python
load_dotenv()
```

```python
openai.api_key = os.getenv("OPENAI_API_KEY")
```

```python
import pandas as pd
import numpy as np

df=pd.read_csv('articles1.csv', sep=',', nrows=100)

df=df.drop(columns=['Unnamed: 0','publication','author','date','year','month','url'])

df['content'][0]

df['review']=df.content.str[:500]

df.drop(columns='content')
```
