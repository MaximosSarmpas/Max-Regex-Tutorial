# Regex Tutorial Starter Code
Regex Tutorial: Understanding URL Matching
This tutorial will break down a specific regular expression (regex) used for matching URLs. By explaining each component of the regex, you will gain a better understanding of how it functions to accurately match URLs in various formats.

Summary
The regex featured in this tutorial is designed to match URLs:

regex
Copy code
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/
We will examine each component of this regex and explain its role in matching URLs.

Table of Contents
Anchors
Quantifiers
OR Operator
Character Classes
Flags
Grouping and Capturing
Bracket Expressions
Greedy and Lazy Match
Boundaries
Back-references
Look-ahead and Look-behind
Regex Components
Anchors
Anchors are used to assert the position of the regex match. In our regex, ^ asserts the start of the string, while $ asserts the end of the string.

regex
Copy code
^...$
Quantifiers
Quantifiers specify how many instances of a character or group must occur. In our regex, ? indicates that the preceding character or group is optional and can occur 0 or 1 times. {2,6} indicates that the preceding character or group must occur between 2 to 6 times.

regex
Copy code
(https?:\/\/)?
([a-z\.]{2,6})
OR Operator
There is no OR operator in this regex.

Character Classes
Character classes represent a set of characters. In our regex, \d represents any digit (0-9), and \w represents any word character (letters, digits, or underscores).

regex
Copy code
[\da-z\.-]+
[\/\w \.-]*
Flags
There are no flags used in this regex.

Grouping and Capturing
Grouping is done using parentheses. In our regex, we have several groups that help match different parts of the URL:

(https?:\/\/)? - The protocol (http or https) and the :// separator.
([\da-z\.-]+) - The domain name.
([a-z\.]{2,6}) - The top-level domain (e.g., .com, .org).
([\/\w \.-]*)* - The path and any additional URL components.
Bracket Expressions
Bracket expressions define a character set. In our regex, [a-z] represents any lowercase letter, and [\/\w \.-] represents a set of characters including forward slash, word characters, space, period, and hyphen.

regex
Copy code
[a-z]
[\/\w \.-]
Greedy and Lazy Match
There are no greedy or lazy match operators in this regex.

Boundaries
There are no word boundaries in this regex.

Back-references
There are no back-references in this regex.

Look-ahead and Look-behind
There are no look-ahead or look-behind assertions in this regex.

Author
This tutorial was created by Maximos Sarmpas, a student of the Carlton university coding bootcamp.
