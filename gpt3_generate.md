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

```
