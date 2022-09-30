# Pandas : For Data Analysis

<a class="anchor" id="0.1"></a>
**TOC:**
1. [Importing pandas](#1)
2. [Reading the data](#2)
3. [Analyze the data](#3)
4. [Pandas - Data Correlations](#4)
5. [Type Casting in Python](#5)
6. [Indexing and Slicing](#6)
7. [Plotting](#7)

Pandas is a Python library used for working with data sets. It has functions for analyzing, cleaning, exploring, and manipulating data.

- Pandas allows us to analyze big data and make conclusions based on statistical theories.
- Pandas can clean messy data sets, and make them readable and relevant.

## **1. Importing Pandas** <a class="anchor" id="1"></a>
[Table of Contents](#0.1)

Pandas can be imported in Jupyer notebook using Python programming language.

    import pandas as pd
    
## **2. How to read data?** <a class="anchor" id="2"></a>
[Table of Contents](#0.1)

Data can be read in various formats. You can read textual, tabular or pictorial data with the use of **pandas**

    data = pd.read_csv("data.csv")
 
## **3. Analyze the data** <a class="anchor" id="3"></a>
[Table of Contents](#0.1)

Data can be analyzed using various methods in pandas. 
    
- **Check null values** - `df.isnull()` methods will give me the null values

        df.isnull()sum()
   
- **Drop duplicates** - `drop_duplicates()` returns DataFrame with duplicate rows removed.
    
- **Indexing** - 

## **4. Pandas - Data Correlations** <a class="anchor" id="4"></a>
[Table of Contents](#0.1)

The `corr()` method calculates the relationship between each column in your data set.

        df.corr()
        
### Result Explained

The Result of the corr() method is a table with a lot of numbers that represents how well the relationship is between two columns.

The number varies from -1 to 1.

- 1 means that there is a 1 to 1 relationship (a perfect correlation), and for this data set, each time a value went up in the first column, the other one went up as well.
- 0.9 is also a good relationship, and if you increase one value, the other will probably increase as well.
- -0.9 would be just as good relationship as 0.9, but if you increase one value, the other will probably go down.
- 0.2 means NOT a good relationship, meaning that if one value goes up does not mean that the other will.

## **5. Type casting**<a class="anchor" id="5"></a>
[Table of Contents](#0.1)

**Type Casting** is the method to convert the variable data type into a certain data type in order to the operation required to be performed by users. In this article, we will see the various technique for typecasting.

There can be two types of Type Casting in Python –

- Implicit Type Casting
- Explicit Type Casting

## **6. Indexing and Slicing**<a class="anchor" id="6"></a>
[Table of Contents](#0.1)

- `.iloc()` and `.iloc()` function are used 
- `.loc` is primarily label based, but may also be used with a boolean array. `.loc` will raise KeyError when the items are not found. 
- `.iloc` is primarily integer position based (from **0** to **length-1** of the axis), but may also be used with a boolean array. `.iloc` will raise IndexError

## **7. Plotting**<a class="anchor" id="7"></a>
[Table of Contents](#0.1)

- Pandas uses the `plot()` method to create diagrams

        import matplotlib.pyplot as plt
        df.plot()
        plt.show()
   
![image](https://user-images.githubusercontent.com/35486320/193227923-fac41eb5-fd63-4adf-9ef9-d049e3875450.png)

