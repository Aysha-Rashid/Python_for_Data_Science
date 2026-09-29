# Python for Data Science
A collection of Python exercises completed as part of the **42 Abu Dhabi Python for Data Science** curriculum.

The project focuses on building a strong foundation in Python while gradually introducing **NumPy, image processing, Pandas, data visualization, object-oriented programming, decorators, closures, and statistical analysis**.

---

## Project Structure

The project is divided into five modules:

```text
Python_for_Data_Science/
│
├── python_00/    # Python fundamentals
├── python_01/    # NumPy & image processing
├── python_02/    # Pandas & data visualization
├── python_03/    # Object-oriented programming
└── python_04/    # Functional programming & statistics
```

---

## Python 00 — Python Fundamentals

The first module focuses on core Python concepts and command-line programming.

Topics covered:
* Variables and basic types
* Functions
* Type checking
* Strings and character processing
* Lists, tuples, sets and dictionaries
* Command-line arguments
* Iterators and generators
* Lambda functions
* Custom implementations of Python functionality
* Morse code conversion
* Progress bars
* Python package creation

### Notable exercises

**`ft_filter` - ex06**

A custom implementation of Python's `filter()` behavior using a generator.

**`Morse Code` - ex07**

Converts alphanumeric strings into Morse code.

**`ft_tqdm` - ex08**

Implements a simplified progress-bar iterator inspired by `tqdm`.

**`ft_package` - ex09**

Creates and packages a small Python package using `setuptools` and `pyproject.toml`.

---

## Python 01 — NumPy & Image Processing

This module introduces numerical computing and image manipulation using **NumPy** and **Matplotlib**.

Topics covered:
* NumPy arrays
* Array shapes and slicing
* Vectorized calculations
* BMI calculations
* Image loading
* Image dimensions and pixel data
* Grayscale conversion
* Image cropping
* Image transposition
* RGB channel manipulation
* Color inversion

### Examples

The image-processing exercises implement operations such as:

```text
Original Image
      │
      ├── Crop / Zoom
      ├── Grayscale
      ├── Transpose
      ├── Invert
      ├── Red filter
      ├── Green filter
      └── Blue filter
```

The exercises demonstrate how images can be represented and manipulated as multidimensional NumPy arrays.

---

## Python 02 — Pandas & Data Visualization

This module introduces working with real datasets using **Pandas** and **Matplotlib**.

Datasets include:
* Life expectancy
* Total population
* GDP per capita adjusted for inflation

### Topics covered
* Loading CSV datasets
* Pandas DataFrames
* Indexing and filtering
* Sorting data
* Extracting country-specific data
* Converting human-readable numerical values
* Data visualization
* Line charts
* Scatter plots
* Logarithmic scales
* Axis formatting

### Data visualizations
The exercises explore relationships such as:

**Life expectancy over time**

A line chart is generated from historical life expectancy data for the United Arab Emirates.

**Population comparison**

Population projections for the United Arab Emirates and France are visualized over time.

**GDP vs Life Expectancy**

A scatter plot compares GDP per capita with life expectancy across countries.

---

## Python 03 — Object-Oriented Programming

This module focuses on Python's object-oriented programming features.

Topics covered:

* Classes and objects
* Inheritance
* Abstract base classes
* Abstract methods
* Class methods
* Multiple inheritance
* Method overriding
* Properties and setters
* Operator overloading

### Example hierarchy

```text
Character
   │
   ├── Stark
   │
   ├── Baratheon
   │
   └── Lannister
          │
          └── King
```

The exercises use a Game of Thrones-inspired class hierarchy to demonstrate inheritance and multiple inheritance.

The module also implements vector operations through operator overloading:

```python
calculator + scalar
calculator - scalar
calculator * scalar
calculator / scalar
```

and vector operations such as:

```python
dotproduct(V1, V2)
add_vec(V1, V2)
sous_vec(V1, V2)
```

---

## Python 04 — Statistics & Functional Programming

The final module combines statistical calculations with more advanced Python programming techniques.

### Statistics

A custom statistical toolkit implements:

* Mean
* Median
* First and third quartiles
* Variance
* Standard deviation

Example:

```python
ft_statistics(
    1, 2, 3, 4, 5,
    mean="mean",
    median="median",
    quartile="quartile",
    variance="var",
    standard_deviation="std"
)
```

### Closures

The `outer()` function demonstrates closures and the `nonlocal` keyword by maintaining state between function calls.

### Decorators

`callLimit()` implements a decorator factory that limits how many times a function can be executed.

```text
callLimit(limit)
      │
      ▼
  decorator
      │
      ▼
 wrapped function
      │
      ├── allowed calls
      └── limit exceeded
```

### Dataclasses

The `Student` class demonstrates Python dataclasses with automatically generated attributes such as:

* Login
* Student ID
* Active status

---

## Technologies

* **Python 3.10+**
* **NumPy**
* **Pandas**
* **Matplotlib**
* **Setuptools**
* **Git**

---

## Installation

Clone the repository:

```bash
git clone https://github.com/Aysha-Rashid/Python_for_Data_Science.git
cd Python_for_Data_Science
```

Create a virtual environment:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

Install the main dependencies:

```bash
pip install numpy pandas matplotlib
```

---

## Running the Exercises

Each exercise is designed to be executed independently.

For example:

```bash
cd python_02/ex01
python3 aff_life.py
```

or:

```bash
cd python_02/ex03
python3 projection_life.py
```

Some exercises expect their datasets or image files to be located in the same directory.

---

## 42 Abu Dhabi

This repository contains exercises completed as part of the **42 Abu Dhabi** curriculum.

The project emphasizes implementing concepts directly rather than relying entirely on high-level abstractions, providing hands-on experience with Python's underlying behavior and commonly used data-science tools.
