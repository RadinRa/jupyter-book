---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# title

here some title ciao

(section-label)=
## my section title

## sajedeh 

Here im referincing [this title](section-label). Try a reference [](section-label).

```{tip}
some text that gives a usefull tip to your reades!
```

ciao 

```{code-cell} ipython3
:tags: [remove-input]

print("A python cell")
```

## A section

And some more Markdown...


```{code-cell} ipython3

%matplotlib inline 
from ipywidgets import interactive
import matplotlib.pyplot as plt
import numpy as np

def f(m, b):
    plt.figure()
    x = np.linspace(-10, 10, num=1000)
    plt.plot(x, m * x + b)
    plt.ylim(-5, 5)
    plt.show()

interactive_plot = interactive(f, m=(-2.0, 2.0), b=(-3, 3, 0.5))
interactive_plot
f((-2.0),(-3))
print("A python cell")
```