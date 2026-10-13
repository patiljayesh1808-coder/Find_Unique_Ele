# Python List Operations: Unique Elements and Frequency

## 📌 Task Description

This task demonstrates two basic Python list operations:

1. Finding unique elements in a list without printing repeated elements more than once.
2. Counting how many times each element appears in a list using a dictionary.

## 💻 Code

```python
l = [5, 4, 5, 4, 2, 1, 3, 1, 6, 4, 2, 3, 5, 7, 6]

# Find unique elements
unique_ele = []

for data in l:
    if data not in unique_ele:
        unique_ele.append(data)

print("Unique Elements:", unique_ele)

# Find the frequency of each element
freq_list = {}

for data in l:
    if data in freq_list:
        freq_list[data] = freq_list[data] + 1
    else:
        freq_list[data] = 1

print("How many times each element appears:", freq_list)
```

## 🖥️ Output

```text
Unique Elements: [5, 4, 2, 1, 3, 6, 7]
How many times each element appears: {5: 3, 4: 3, 2: 2, 1: 2, 3: 2, 6: 2, 7: 1}
```

## 🧠 Concepts Used

- Python lists
- `for` loops
- `if-else` conditions
- `append()` method
- Dictionaries
- Frequency counting

## 🎯 Learning Outcome

Learned how to remove duplicate entries while preserving the original order and how to count the frequency of each element using a dictionary.

---

**Submitted to:** Atul Sir  
**Institute:** Kiran Academy
