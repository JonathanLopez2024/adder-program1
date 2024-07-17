# adder-program1

def add_two_numbers(a, b):
    return a + b

# add_numbers.py

def add_two_numbers(a, b):
    return a + b

if __name__ == "__main__":
    num1 = float(input("Enter the first number: "))
    num2 = float(input("Enter the second number: "))
    result = add_two_numbers(num1, num2)
    print(f"The result of adding {num1} and {num2} is {result}")


# Unit Test - Create Different File

# test_add_numbers.py

import unittest
from add_numbers import add_two_numbers

class TestAddTwoNumbers(unittest.TestCase):
    def test_addition(self):
        self.assertEqual(add_two_numbers(2, 3), 5)
        self.assertEqual(add_two_numbers(-1, 1), 0)
        self.assertEqual(add_two_numbers(0, 0), 0)
        self.assertEqual(add_two_numbers(-1, -1), -2)

if __name__ == '__main__':
    unittest.main()
