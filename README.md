### Steps for creating a new test and method using TDD

#### test_student.py
1. Create a new test method called test_apply_extension
2. Inside test_apply_extension, store the current end_date for our student instance in a variable called old_end_date
3. Call a method named apply_extension that will take a number of days as an argument on the student instance to update the end_date
4. Assert whether the instance's end_date equals the old end_date plus the days argument that was passed in using timedelta
5. Run the tests to confrim that the new method is failing

#### student.py
1. In the Student class, create a new method called apply_extension that has a parameter called days
2. Use the timedelta method from datetime to update the end_date property
3. Run the tests to confirm they are working


### Mocking Our Method Challenge
- Build a test method called test_course_schedule_failed that:
    1. Creates a request context manager similar to  the text_course_schedule_success method
    2. Mocks an unsuccessful request where the return value indicates a failed request and the value stored in schedule is the expected string when a request fails

#### Reflective Questions
- What should the value of return_value.ok be to mock a failed request?
- Where did we define the string that should be returned for a failed request?