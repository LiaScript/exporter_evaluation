<!--
author:   Your Name

email:    your@mail.org

version:  0.0.1

language: en

narrator: US English Female

comment:  Try to write a short comment about
          your course, multiline is also okay.
-->

# Main Title

This examplary LiaScript document adresses basic Markdown formats.

## Basic Markdown

Lists and numbers
-----------------

* alpha
+ **beta**
- gamma
  and delta

  new Paragraph

  - and another
  - important list

- epsilon

Block quotes
-----------------

> This was said some time ago ...
>
>> This was said even longer ago,
> > I guess ...
>
> * aleph
> * beth

Citations
-----------------
> “Live as if you were to die tomorrow.
> Learn as if you were to live forever.”
>
> -- Mahatma Gandhi

References
-----------------

[Project Website](https://liascript.github.io/)

## Tables and Images

Images referencing external content
-----------------

`![OER Logo](https://upload.wikimedia.org/wikipedia/commons/thumb/2/20/Global_Open_Educational_Resources_Logo.svg/800px-Global_Open_Educational_Resources_Logo.svg.png)`

> External image references generate an error for pdf generation. This has to be evaluated!

Images referencing project internal content
-----------------

![OER Logo](./images/OER_Logo.png)

Table
-----------------

| Tables               |      Are      |  Cool |
| -------------------- |:-------------:| -----:|
| *** columns 3 is *** | right-aligned | $1600 |
| ** column 2 is **    |   centered    |   $12 |
| * zebra stripes *    |   are neat    |    $1 |


## Code Snippets

``` python
import time
# Quick, count to ten!
for i in range(10):
    # (but not *too* quick)
    time.sleep(0.5)
    print(i)
```
