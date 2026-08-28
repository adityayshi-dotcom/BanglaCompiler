\# Bangla Compiler - Lexer



This repository contains the lexical analysis component of a simple compiler for a Bangla-based programming language.



\## Implemented By



Lexer module implemented in Java.



\## Supported Bangla Keywords



| Bangla Keyword | Meaning |

|---|---|

| সংখ্যা | Integer datatype |

| লেখা | String datatype |

| যদি | If |

| নাহলে | Else |

| যতক্ষণ | While |



\## Supported Tokens



The lexer recognizes:



\- Bangla and English identifiers

\- Integer numbers

\- String literals

\- Arithmetic operators:

&#x20; - `+`

&#x20; - `-`

&#x20; - `\*`

&#x20; - `/`

\- Assignment operator:

&#x20; - `=`

\- Comparison operators:

&#x20; - `==`

&#x20; - `!=`

&#x20; - `<`

&#x20; - `<=`

&#x20; - `>`

&#x20; - `>=`

\- Parentheses:

&#x20; - `(`

&#x20; - `)`

\- Braces:

&#x20; - `{`

&#x20; - `}`

\- Semicolon:

&#x20; - `;`

\- EOF token

\- Invalid-character errors

\- Unterminated-string errors



\## Lexer Components



\### TokenType.java



Defines all token categories recognized by the lexer.



\### Token.java



Represents an individual token and stores:



\- Token type

\- Lexeme

\- Line number

\- Column number



\### Lexer.java



Performs lexical analysis and converts Bangla source code into a list of tokens.



\### LexerError.java



Stores lexical errors with line and column information.



\## Example Program



```text

সংখ্যা বয়স = 20;



যদি (বয়স >= 18) {

&#x20;   লেখা অবস্থা = "প্রাপ্তবয়স্ক";

}

নাহলে {

&#x20;   লেখা অবস্থা = "শিশু";

}



যতক্ষণ (বয়স < 25) {

&#x20;   বয়স = বয়স + 1;

}

