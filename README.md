# Lesson-01
### 1. Unittest - Unit Testing Framework
The unittest unit testing framework was originally inspired by JUnit and has a similar flavor as major unit testing frameworks in other languages. It supports test automation, sharing of setup and shutdown code for tests, aggregation of tests into collections, and independence of the tests from the reporting framework.

### 2. Concepts
test fixture  
A test fixture represents the preparation needed to perform one or more tests, and any associated cleanup actions. This may involve, for example, creating temporary or proxy databases, directories, or starting a server process.

test case  
A test case is the individual unit of testing. It checks for a specific response to a particular set of inputs. unittest provides a base class, TestCase, which may be used to create new test cases.

test suite  
A test suite is a collection of test cases, test suites, or both. It is used to aggregate tests that should be executed together.

test runner  
A test runner is a component which orchestrates the execution of tests and provides the outcome to the user. The runner may use a graphical interface, a textual interface, or return a special value to indicate the results of executing the tests.

### 3. Basic Example
```
def add(a, b):
    return a + b
```
Now we are going to create a testcase to test the method 'add(a, b)'.   
```
class Calculate(unittest.TestCase):
    def test_add(self):
        self.assertEqual(add(5, 10), 15)
```

### 4. Exercise
1.Fill in the blanks in 'test_person_01.py' and pass the tests.  
2.Find the errors in 'test_person_02.py' and correct them.  
3.Complete 'test_person_03.py' and pass the tests.  