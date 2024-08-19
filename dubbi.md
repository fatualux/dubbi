## Punti critici

### 16/08/2024
- try/except - In quali situazioni devo utilizzare la pratica di gestione degli errori?
https://fatualux.github.io/python-notes/chapters/principles/error_handling.html

- creazione ed esecuzione di test/CI-CD "best practises"
https://fatualux.github.io/python-notes/chapters/principles/testing.html

- COMPREHENSION
    - Nested list/dictionaries comprehension - flattening a list of lists
     - https://fatualux.github.io/python-notes/chapters/lists/comprehensions.html
     - https://fatualux.github.io/python-notes/chapters/dictionaries/comprehensions.html
As far as it regards dictionaries I understood the code snippets provided as examples, but I am not sure I master these concepts.

- Module initialization
  - ```if __name__ == "__main__":``` construct (https://fatualux.github.io/python-notes/chapters/modules.html)
  - I understood that it's a method used to initialized modules only when they're executed directly (not after being imported), but I cannot figure th use cases.

### 19/08/2024

- Variable-Length Arguments: Python functions can accept an arbitrary number of arguments using *args (for non-keyword arguments) and **kwargs (for keyword arguments).
(https://fatualux.github.io/python-notes/chapters/functions.html)

Ho compreso in linea di massima le funzioni lambda, ma non ho capito questo esempio, nonostante mi sia guardato il metodo *sorted*:

```python
points = [(2, 3), (1, 2), (4, 1)]
sorted_points = sorted(points, key=lambda point: point[1])
print(sorted_points)  # Output: [(4, 1), (1, 2), (2, 3)]
```


- Funzioni di alto livello e concetti programmazione funzionale.
Degli esempi che ho messo [qui](https://fatualux.github.io/python-notes/chapters/functions/higher_order.html) non ho capito questo:

```python
def make_multiplier(factor):
    return lambda x: x * factor

double = make_multiplier(2)
print(double(5))  # Output: 10
```

e questo:

```python
def add(x, y):
    return x + y

numbers = [1, 2, 3, 4]
total = reduce(add, numbers)
print(total)  # Output: 10
```

Ho capito il metodo *reduce()* ma non ho capito come mai qui riesco ad effettuare la somma di ogni elemento e non solo di due, dal momento che il numero di parametri di *add()* è 2 (sommo a + b).

- Class methods:

*Class methods are methods that operate on the class itself rather than on instances of the class. They are defined using the @classmethod decorator and take cls as the first parameter, which represents the class.*

Casi d'uso? non ne comprendo l'utilità.
