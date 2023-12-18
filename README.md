# Patika.dev_Python
Python Basics with Patika.dev
## Python Basics

 

<br>

 

1-) 
```
 
def flatten_list(lst):
    flattened = []
    for item in lst:
        if isinstance(item, list):
            flattened.extend(flatten_list(item))
        else:
            flattened.append(item)
    return flattened

# Örnek kullanım
input_list = [['Bilge', 'GIS', ['25'], 18.3], [[['Lila']], 'cat'], '08012023', 5]
output_list = flatten_list(input_list)
print(output_list)
 
```

<br>

2-)
```

def reverse_nested_list(lst):
    reversed_list = []
    for item in reversed(lst):
        if isinstance(item, list):
            reversed_list.append(reverse_nested_list(item))
        else:
            reversed_list.append(item)
    return reversed_list

# Örnek kullanım
input_list = [[100, 200], [300, 400], [500, 600, 700], [800, 900, 1000]]
output_list = reverse_nested_list(input_list)
print(output_list)

```

<br>
