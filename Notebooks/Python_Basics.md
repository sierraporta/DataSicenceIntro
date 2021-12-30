## Python Basics
Most of these notes are built in Jupyter Notebook. So let's do a quick review of how to install Jupyter Notebook first. 

Jupyter Notebook is an open source web application that allows us to create and share code and documents. It is an interactive computing environment, which allows users to experiment with code and share it.

![jupyter](https://miro.medium.com/max/756/0*AqFDoe9TNQQLmrl1.png)

Tka a look from their web page: https://jupyter.org/

Jupyter is the acronym for Julia, Python and R, the three programming languages Jupyter started with, although today it supports a large number of languages.
It is widely used to create and share documents containing code. This is very useful in teaching, since we can show with examples how a script, a language works or ask students to propose and validate their own code.

To install Jupyter Notebook, please keep forward the next link: https://docs.jupyter.org/en/latest/install/notebook-classic.html


```python
import numpy as np
import matplotlib.pyplot as plt
```


```python
x=np.arange(1,10,1)
```


```python
y=np.random.randint(13,50,len(x))
```


```python
plt.figure(figsize=(8,6))
plt.plot(x,y,marker='o')
plt.show()
```


![png](Python_Basics_files/Python_Basics_5_0.png)



```python

```


```python

```
