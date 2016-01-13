# Language Analysis

For JavaScript files, Codeanywhere provides analysis using a combination of our own analysis tools, as well as JSHint (specifically for Javascript code). Our language analysis can't detect if your program is correct, fast, nor has memory leaks, but it can save you time by spotting things like undeclared variables, syntax errors, or other preventable typos.
When Codeanywhere detects an issue with your code, an icon appears in the gutter (located left from the editor) for the offending lines of code. There are three types of identifiers available for your code:
●	Informational: these are non-critical, non-dangerous updates about your code
●	Warnings: these are potentially incorrect pieces of code
●	Errors: these are incorrect lines of code that will almost certainly throw a runtime error when you try to run your script
	
If you hover over any of these icons in the gutter, you'll get a pop-up that presents some information as to what, exactly, the problem is. For example, suppose we have an argument font-weight in CSS, and we spell „normal“ wrong.
