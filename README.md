# Core Python Data Structures: Dictionaries, Sets, and Tuples

## Overview

This project demonstrates fundamental Python data structures beyond lists, focusing on:

* Dictionaries (key-value mappings)
* Sets (unordered unique collections)
* Tuples (immutable sequences)

The notebook illustrates creation, access, modification, and inspection of these structures in a Python 3 environment.

---

## 1. Dictionaries

### Definition

A dictionary is a key-value data structure that maps unique keys to associated values.

Example:

```python
Notas = {'João': 6.0, 'Maria': 8.0, 'Pedro': 6.5}
```

Keys must be unique and immutable. Values can be of any type.

---

### Accessing Values

Values are accessed using their keys:

```python
print(Notas['João'])
```

---

### Retrieving Keys and Values

```python
Notas.keys()
Notas.values()
```

* `keys()` returns all dictionary keys
* `values()` returns all stored values

---

### Membership Testing

```python
'João' in Notas
```

Checks whether a key exists in the dictionary.

---

### Removing and Adding Elements

Remove an entry:

```python
del Notas['João']
```

Add or update an entry:

```python
Notas['Ana'] = 9
```

---

### Safe Value Retrieval

Use `get()` to avoid runtime errors when a key does not exist:

```python
Notas.get('Geraldo', "Not found.")
```

The second argument is a default value returned if the key is missing.

---

### Dictionaries with Tuple Keys

Tuples can be used as dictionary keys because they are immutable:

```python
dic2 = {(0, 1): 0, (1, 2): 1}
```

This demonstrates how composite keys can represent structured relationships.

---

## 2. Sets

### Definition

A set is an unordered collection of unique elements.

Example:

```python
bigdata = {'Spark', 'Hive', 'Sqop'}
```

Properties:

* No duplicate values
* No guaranteed order

---

### Membership Check

```python
'Spark' in bigdata
```

---

### Adding Elements

```python
bigdata.add('Hadoop')
```

---

### Set Size

```python
len(bigdata)
```

Returns the number of unique elements.

---

## 3. Tuples

### Definition

A tuple is an immutable ordered sequence.

Example:

```python
tupla = (1, 2, 3, 4, 5, 6, 7)
```

Key difference from lists:

* Tuples cannot be modified after creation.

---

### Accessing Tuple Elements

```python
tupla[4]
```

Tuples use zero-based indexing, just like lists.

---

## 4. Type Inspection

The `type()` function identifies the data structure:

```python
type(Notas)   # dict
type(bigdata) # set
type(tupla)   # tuple
```

Understanding object types is essential for debugging and system design.

---

## Environment

* Python 3.12.4
* Jupyter Notebook
* Conda base environment

---

## Learning Objectives

This notebook builds foundational understanding of:

* Key-value mapping
* Immutable vs mutable structures
* Unique-value collections
* Membership testing
* Safe data access patterns

These data structures form the backbone of real-world Python applications, including:

* Data processing
* API handling
* Configuration management
* Performance optimization
* Algorithm design
