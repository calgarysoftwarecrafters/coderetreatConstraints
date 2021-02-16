

### Summary:

On test failure, revert everything except the test


### Details:

Every time you run your tests, you will either:



1. Commit everything, because **all tests passed**
2. Revert everything (or everything except the test) because **it failed**