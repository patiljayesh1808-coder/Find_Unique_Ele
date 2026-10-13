# Python List Operations: Unique Elements and Frequency

## 📌 Task Description

This task contains two separate Python programs:

1. Finding unique elements in a list.
2. Finding the frequency of every element in a list using a dictionary.

---

## Program 1: Find Unique Elements

### Code

```python
l = [5, 4, 5, 4, 2, 1, 3, 1, 6, 4, 2, 3, 5, 7, 6]

unique_ele = []

for data in l:
    if data not in unique_ele:
        unique_ele.append(data)

print(unique_ele)
```

### Output

```text
[5, 4, 2, 1, 3, 6, 7]
```

### Explanation

- Create an empty list named `unique_ele`.
- Check each element in the original list.
- Add an element only if it is not already in `unique_ele`.
- Print the list containing each element once.

---

## Program 2: Find the Frequency of Each Element

### Code

```python
l = [5, 4, 5, 4, 2, 1, 3, 1, 6, 4, 2, 3, 5, 7, 6]

freq_list = {}

for data in l:
    if data in freq_list:
        freq_list[data] = freq_list[data] + 1
    else:
        freq_list[data] = 1

print(f"How many times repeated each element: {freq_list}")
```

### Output

```text
How many times repeated each element: {5: 3, 4: 3, 2: 2, 1: 2, 3: 2, 6: 2, 7: 1}
```

### Explanation

- Create an empty dictionary named `freq_list`.
- If the element already exists as a key, increase its count by one.
- Otherwise, add the element to the dictionary with a count of one.
- Print the dictionary showing each element and its frequency.

---

## 🧠 Concepts Used

- Python lists
- `for` loops
- `if-else` conditions
- `append()` method
- Dictionaries
- Frequency counting

## 🎯 Learning Outcome

Practiced finding unique elements and counting the occurrences of each element using two separate Python programs.
