### Steps for Creating a new test and method using TDD

1. Create a new test method called test_apply_extension
2. Inside test_apply_extension, store the current end_date for our student instance in a variable called old_end_date
3. Call a method named apply_extension that will take a number of days as an argument on the student instance to update the end_date
4. Assert whether the instance's end_date equals the old end_date plus the days argument that was passed in using timedelta
5. Run the tests to confrim that the new method is failing
6. In the Student class, create a new method called apply_extension that has a parameter called days
7. Use the timedelta method from datetime to update the end_date property
8. Run the tests to confirm they are working