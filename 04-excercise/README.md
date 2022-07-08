# `04` Exercise

**Create a program that asks the user for a number and then prints out a list of all the divisors of that number. (If you don’t know what a divisor is, it is a number that divides evenly into another number. For example, 13 is a divisor of 26 because 26 / 13 has no remainder.)**

```python
def main():
    input_number = int(input('enter a number to display all its divisors: '))

    list_divisors = []

    for i in range(1, input_number + 1):
        if input_number % i == 0:
            list_divisors.append(i)

    print('list of all divisors of {}: {}'.format(input_number, list_divisors))


if __name__ == "__main__":
    main()
```