## TDD in pyhton

t's important to take baby steps when completing unit tests in python. We want to make sure we break down the bigger problems of our projects to small steps that we can implement in tests to stop bugs before they star and give us faster results.

With unit testing in python, we have to create a block of code that can helps the testing enviorment know what it's looking for. Hereis an example below: 

def test_should_return_female_when_the_name_is_from_female_gender():
    detector = GenderDetector()
    expected_gender = detector.run(‘Ana’)
    assert expected_gender == ‘female’

    as you can see, a python function is defined and with a descriptive name to help us test whichever code we wish to.

    Other thing to care about is the structure. A convention widely used is the AAA: Arrange, Act and Assert.
Arrange: you need to organize the data needed to execute that piece of code (input);
Act: here you will execute the code being tested (exercise the behaviour);
Assert: after executing the code, you will check if the result (output) is the same as you were expecting.
Now you can execute the tests. I suggest the lib pytest to do it. But you are free to choose anything you like.