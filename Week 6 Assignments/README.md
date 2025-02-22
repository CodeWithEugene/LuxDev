# Question 1. Difference Between Loading (JSON) and Reading (CSV)

### Loading (JSON)

JSON (JavaScript Object Notation) is a hierarchical data format that supports nested structures like dictionaries and lists. 
When you load a JSON file in Python using `json.load()`, it reads the file and converts the JSON data into a Python object eg. a dictionary or a list. 
This allows you to access the data using keys or indices.


### Reading (CSV)

CSV (Comma-Separated Values) is a format where data is organized into rows and columns which are separated by commas. 
When you read a CSV file using `csv.reader()` or `pandas.read_csv()`, it treats the file as a table and allows you to access the data row by row or as a DataFrame.


# Question 2. Difference Between Writing (CSV) and Dumping (JSON)

### Writing (CSV)

Writing to a CSV file means to format data into a tabular structure with rows and columns. 
I tried to use `csv.writer()` to write lists or tuples as rows in the CSV file and it worked.

**Example:**

```python
import csv  

data = [['Name', 'Age'], ['Alice', 25], ['Bob', 30]]  

with open('output.csv', 'w', newline='') as file:  
    writer = csv.writer(file)  
    writer.writerows(data)  
```

### Dumping (JSON)

Dumping to JSON involves converting a Python object (like a dictionary or list) into a JSON-formatted string and saving it to a file. 
One can use `json.dump()` to serialize the Python object into JSON format.

**Example:**

```python
import json  

data = {"name": "Alice", "age": 25}  

with open('output.json', 'w') as file:  
    json.dump(data, file, indent=4)  
```

# Question 3. Loading a Personal Image in Python

To load and display an image in Python, you can use libraries like Pillow (PIL) or OpenCV. Below are examples for both:

### Using Pillow (PIL):

```python
from PIL import Image
with open("eugene.jpg", "rb") as src:
    data = Image.open(src)
    data.show()

from PIL import Image
from IPython.display import display

with open("william f65 pic.jpg", "rb") as src:
    data = Image.open(src)
    display(data) 
```

### Displaying in Jupyter Notebook (using matplotlib):

```python
import matplotlib.pyplot as plt  
import matplotlib.image as mpimg  
  
img = mpimg.imread("my_photo.jpg")  
plt.imshow(img)  
plt.axis("off")  
plt.show()
```

# Question 4. Write on hypothesis testing, why we use it, and when we use it


Kindly access my article [here](https://medium.com/@eugenegabriel.ke/hypothesis-testing-why-we-use-it-and-when-we-use-it-e2877c2d486c)
