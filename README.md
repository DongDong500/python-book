# python-book

## for personal use (python cook-book)

### Asterisk(*) 

<https://treyhunner.com/2018/10/asterisks-in-python-what-they-are-and-how-to-use-them/>

<https://mingrammer.com/understanding-the-asterisk-of-python/>

1. multiplication and power operations.

2. repeatedly extending the list-type containers.

3. variadic arguments. “packing”

 Positional arguments and other is keyword arguments, the former are specified according to their position and latter are the arguments with keyword which is the name of the argument.

4. unpacking the containers.

The * can also be used for unpacking the containers. Its principles is similar to “For using the variadic arguments” in above. The easiest example is that we have data in the form of a list, tuple or dict, and a function take variable

```
>>> fruits = ['lemon', 'pear', 'watermelon', 'tomato']
>>> print(fruits[0], fruits[1], fruits[2], fruits[3])
lemon pear watermelon tomato
>>> print(*fruits)
lemon pear watermelon tomato

def transpose_list(list_of_lists):
    return [
        list(row) for row in zip(*list_of_lists)
    ]
>>> transpose_list([[1, 4, 7], [2, 5, 8], [3, 6, 9]])
[[1, 2, 3], [4, 5, 6], [7, 8, 9]]
```