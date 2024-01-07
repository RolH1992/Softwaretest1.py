# Softwaretest1.py
#A basic software test. For example divide 10 by 0 it should show a AssertionError.

import unittest

# The class that contains the tests
class MyTest(unittest.TestCase):
    # The setup method is run before each test method
    def setUp(self):
        # Initialize any resources needed for the tests
        pass
    
    # The teardown method is run after each test method
    def tearDown(self):
        # Clean up any resources used by the tests
        pass
    
    # Test methods should start with the word "test"
    def test_addition(self):
        result = 2 + 2
        self.assertEqual(result, 4)
    
    def test_subtraction(self):
        result = 5 - 3
        self.assertEqual(result, 2)
    
    def test_multiplication(self):
        result = 4 * 3
        self.assertEqual(result, 12)
    
    def test_division(self):
        result = 10 / 2
        self.assertEqual(result, 5)  # Compare with an expected value

# Run the tests
if __name__ == '__main__':
    unittest.main()
