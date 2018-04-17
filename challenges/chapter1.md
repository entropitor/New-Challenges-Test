---
title: "python_basics"
output: html_document

--- type:MultipleChoiceChallenge key:107L8j1H95f231l1SC9vIYGfLFcAy7xCikn difficulty:1
## Choose the right answer

*** =assignment1
Which symbol marks the beginning of a comment in Python?

*** =options1
- `%`
- `%*`
- [`#`]
- `@`
- `$`
- `*`
- `/*`

*** =assignment2
Which function is used to determine the data type of an object?

*** =options2
- `class()`
- `data.type()`
- [`type()`]
- `object.type()`
- `typeof()`

--- type:MultipleChoiceChallenge key:211tSzjdCihQf difficulty:1
## Other mcq
*** =assignment1
Which data type(s) can a list hold?

*** =options1
- Only strings
- Only integers
- Only booleans
- Only integers and booleans
- Only floats
- Only floats and integers
- [Any object]

*** =assignment2
Which of the following is the recommended method of assigning a value to a variable?

*** =options2
- [`x = 5`]
- `x <- 5`
- `x is 5`
- `x == 5`
- `x -> 5`
- `x assign 5`

--- type:OutputChallenge key:107H5LslS6zeRElpelPPwFGdZPrkiVVtNHm difficulty:1
## Basic math operations - 1

*** =code
```{python}
p = {{$var1}}
q = {{$var2}}
print(p {{fun1}} q)
```

*** =pre_challenge_code
```{python}
import dccpu.generators as g
```

*** =variables
var1:
  - '4'
  - '6'
  - '8'
var2:
  - '1'
  - '2'
  - '4'
fun1:
  - '+'
  - '-'
  - '*'

--- type:OutputChallenge key:107m7CS9a8GhB
## Basic math operations - 2

*** =code
```{python}
x = {{var1}}
y = {{var2}}
print(x {{fun1}} y)
```

*** =pre_challenge_code
```{python}
import dccpu.generators as g
```

*** =variables
var1:
  - '4'
  - '6'
  - '8'
  - '12'
var2:
  - '1'
  - '2'
  - '4'
fun1:
  - '%'
  - '**'
  - '/'


--- type:OutputChallenge key:107QfXOqEPbWEqN5oDhqgQTteZJOF1nrBCp difficulty:1
## Type of a variable

*** =code
```{python}
p = {{var1}}
print(type(p))
```

*** =variables
var1:
  - 'True'
  - 'False'
  - '"True"'
  - '"False"'
  - '"str"'
  - '23'
  - '6.5'
  - '"7.2"'
  - '"23"'
  - 'None'
  - '"None"'

--- type:BlanksChallenge key:107GYNS5El5prfnHk30oE5VLFZEf1EAFdbM
## Convert data types - 1

*** =code1
```{python}
x = {{var1}}
print({{_fun1}}(x))
```

*** =code2
```{python}
x = {{var2}}
print({{_fun2}}(x))
```

*** =code3
```{python}
x = {{var3}}
print({{_fun3}}(x))
```

*** =pre_challenge_code
```{python}
import dccpu.generators as g
```

*** =variables
var1:
  - '!expr g.rand_bool()'
  - '!expr g.stringify(g.rand_int, hi=20)'
var2:
  - '!expr g.rand_bool()'
  - '!expr g.stringify(g.rand_float, hi=20)'
var3:
  - '!expr g.rand_int(hi=2)'
fun1:
  - 'int'
fun2:
  - 'float'
fun3:
  - 'bool'

*** =distractors
fun1:
  - '{{fun2}}'
  - '{[fun3}}'
  - 'num'
fun2:
  - '{{fun1}}'
  - '{{fun3}}'
  - 'num'
fun3:
  - '{{fun1}}'
  - '{{fun2}}'
  - 'log'
  
--- type:BlanksChallenge key:107gi81JxnH1FSMu6cTBiWBWdR1HMgeoFJz
## Convert data types - 2

*** =code1
```{python}
p = {{var1}}
q = {{var2}}
print(q + {{_fun2}}(p))
```

*** =code2
```{python}
p = {{var1}}
q = {{var2}}
print({{_var3}} + str(p))
```

*** =code3
```{python}
p = {{var1}}
q = {{var2}}
print(q + str({{_var4}}))
```

*** =code4
```{python}
p = {{var1}}
q = {{var2}}
print(q {{_fun1}} str(p))
```

*** =pre_challenge_code
```{python}
import dccpu.generators as g
```

*** =variables
var1:
  - '!expr g.rand_int()'
  - '!expr g.rand_float()'
var2:
  - '"The value of p is: "'
  - '"p is: "'
var3:
  - 'q'
var4:
  - 'p'
fun1:
  - '+'
fun2:
  - 'str'

*** =distractors
var3:
  - "q"
var4:
  - "p"
fun1:
  - "-"
  - "*"
  - "&"
fun2:
  - "string"
  - "char"
  
--- type:BlanksChallenge key:107DB51jGEmsn
## Convert data types - 3

*** =code1
```{python}
p = {{var1}}
q = {{var2}}
print(q {{_fun1}} p)
```

*** =pre_challenge_code
```{python}
import dccpu.generators as g
```

*** =variables
var1:
  - '!expr g.rand_int(hi=5)'
var2:
  - '"Hello! "'
  - '"Python "'
  - '"DataCamp "'
var3:
  - 'q'
fun1:
  - '*'

*** =distractors
fun1:
  - "+"
  - "**"
