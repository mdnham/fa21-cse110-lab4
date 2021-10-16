
1. values added: 20
2. final result: 20
3. values added: 20
4. This will return an error, because the usage of "let" means that _result_ has only been declared in the if-block. Thus, it does not exist outside of the if-block; hence, line 13 would return an error as we're calling a variable that does not exist.
5. The code will return an error due to line 7, since it is trying to alter _result_ when _result_ has been declared with "const" so it cannot be altered. So, it does not even reach line 9.
6. Similar to #5, line 13 will not be reached due to the same error.