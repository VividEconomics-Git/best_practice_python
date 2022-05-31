<h1>Best Practice</h1>
<h2>Coding / Python</h2> 

Short preamble: you should aim to write code that is bug-free and runs reasonably fast. Besides, your code should be easy for a moderately python-literate colleague to understand and make changes to. Remember that like a slide deck or a report, your code is for human consumption – the computer only understands ones and zeros anyway. **Achieving both functionality and understandability is easier when following the below advice.**

<ol>
  <li>
  <b>Single source of truth</b>
  
  - Data / inputs should only be defined at a single location
    - In almost every case this should be done in a separate .csv file in the inputs folder. If this would not be suitable then the inputs must be defined at the top of the scripts and clearly marked
    - Hard-coded parameters should be capitalized, so that code readers know to look them up at the top of the scripts when they come across one
    
  </li>
  <li>
  <b>All variables used inside functions should be given as parameters or be declared within the function</b>
  - No global variables are allowed inside functions!
  </li>
  
  <li>
  <b>Write clean and tidy code</b>
  
  - Use PyCharm tick or equivalent as the gold standard
    - Not good for use if model code contains PyCharm warnings and errors
  - If unsure how to write code refer to the Python style guide [https://peps.python.org/pep-0008/](https://peps.python.org/pep-0008/)
  - Refactoring, avoid nested if statements
    - Nested if statements makes code difficult to understand. There are several strategies for avoiding this. See for example: [https://www.python-engineer.com/posts/python-refactoring-tips/](https://www.python-engineer.com/posts/python-refactoring-tips/)
  </li>
  
  <li>
  <b>Variable names</b>
  
  - Use sensible and simple to understand names
  - Stick to snake\_case naming convention
  </li>
  <li>
  <b>Short and sharp functions</b>
  
  - Each function should only do one thing
  </li>
  <li><b>Within code documentation</b>
  
  - Code commenting
    - <b>How much?</b> Every 1-5 lines of code minimum.
    - <b>When?</b> As soon as you finished the code
    - <b>What?</b>  Explain why
  - Docstrings
    - For all your functions you should write docstrings according to the Pandas/NumPy standard. For more information see [https://numpydoc.readthedocs.io/en/latest/format.html](https://numpydoc.readthedocs.io/en/latest/format.html)
  </li>
  <li><b>Vectorize and avoiding using for loops</b>
  
   - Writing loops is often very inefficient – the main alternative is vectorization. See this post on what it is [https://stackoverflow.com/questions/47755442/what-is-vectorization](https://stackoverflow.com/questions/47755442/what-is-vectorization) and this one on why it is faster,

  </li>
  <li>
  <b>Vectorizing and avoiding using loops</b>
  
   - Writing loops is often very inefficient – the main alternative is vectorization. See this post on what it is https://stackoverflow.com/questions/47755442/what-is-vectorization and this one on why it is faster,
  </li>
  
  <li>
  <b>Write DRY code</b>
  
   - DRY stands for Don't Repeat Yourself. Read more here: [https://www.earthdatascience.org/courses/intro-to-earth-data-science/write-efficient-python-code/intro-to-clean-code/dry-modular-code/](https://www.earthdatascience.org/courses/intro-to-earth-data-science/write-efficient-python-code/intro-to-clean-code/dry-modular-code/)
  </li>
  
  <li>
  <b>Remove legacy code, commented out chunks, TODOs and other unnecessary stuff before pushing your code! </b>
    
   - Use issues log rather than inline comments to keep track of to dos
  </li>
</ol>
