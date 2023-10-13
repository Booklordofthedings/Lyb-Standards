# Lyb-Standards
There is no official standard for beef code and projects yet, outside of a simply doing it mostly how c# does it.  
I wanted to make my own unofficical standards for beef projects, for both code, and files.  
No one needs to follow these, but I think they make for a good baseline and readable code.  
There are reasons even someone who wants to follow these standards cant do that and thats fine.

## Index
[Formatting Conventions](#Formatting-Conventions)
[Gitignore](#Gitignore)
[Keywords](#Keywords)

## Formatting Conventions
__Tabs vs Spaces:__
Tabs are used, as its the default setting in alot of ide's aswell as in beef-ide.  

__Curly Braces Positioning:__
Curly braces go onto a new line. C# does it that way and it allows seeing the scope of braces better. There may be valid reasons where this is not the case, like having a ton of oneliner functions. Here a different formatting may be used to save space.  

## Gitignore
The common gitignore file for beef projects, includes some additional files for better coverage of common usecases
```
build/
recovery/
packages/
dist/
BeefSpace_User.toml
```

## Keywords
This lists some of the common names for specific variables and operations.

| Name | Meaning | Explanation |
| --- | --- | --- |
| i, j, k, l, m, n | *Index* | Used in indexable loops. If its multiple loops deep use the next character |
| err | *Error* | Variable containing an error. May be the result of getting the error of a Result<T, TErr> operation or an error code/enum |
| e, o | *Entry, Object* | Represents the current object/entry in a loop or something similar. Used in foreach loops |
| res | *Result* | The result of an operation. Commonly a Result<T> or a boolean |
| rhs, lhs | *Left hand side, Right hand side* | For operator overloads, where these variables are the side of the operation |
| toReturn | *toReturn* | Variable that is to be assigned during the function and will be returned at the end |
