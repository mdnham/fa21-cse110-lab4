
1. values added: 20
2. final result: 20
3. values added: 20
4. This will return an error, because the usage of "let" means that _result_ has only been declared in the if-block. Thus, it does not exist outside of the if-block; hence, line 13 would return an error as we're calling a variable that does not exist.
5. values added: 0 (Previous line will return an error due to trying to change a const variable.)
6. Similar to #4, this will return an error, because the usage of "const" also means that _result_ has only been declared in the if-block. And so, line 13 will return an error since we are again calling a variable that does not exist.