Tabs are generally used in code to indent lines. So it is really important to draw them the way they will be shown in any other text editor. On the other hand sometimes things got added to the original line, like line number for example, and that shouldn't change the original tab sizes.

So how it's done?
First of all, for each tab in the line it's width in chars got calculated before anything else is done.
If nothing else would be done later as, for example, visualizing of white spaces, then tabs stays in the line untouched, mainly to make it possible for the user to see them.

If on the other hand we going to change original line, tabs got replaced by spaces. If white spaces are visible then there are no drawbacks at all, code stays indent and user could see where tabs chars are inside the code.
However, if line numbers is enabled and visible white spaces are turned off, code stays indent but user wouldn't be able to distinguish between plain spaces and tabs chars. But that's the only way to preserve the original indentation with line numbers in front of each line.