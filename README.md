Formatting that works with Markdown and reST / sphinx
=====================================================

Code blocks
===========

* for Markdown we can use indents
* for reST we can use `::` 

**Good:** Combination of both (notice the double-colon at end of this line)::

    <f:if condition="{something} == 'other'">
   
    </f:if>
   
   
**Bad:** This will work for Markdown but not reST:   

    <f:if condition="{something} == 'other'">
   
    </f:if>


Headers
=======

**Good**

* Use headers with underline.
* Use headers sparingly, do not create complicated hierarchies
* For reST sphinx the hierarchy is determined by what underline style is used
  first, next etc. 


1. Header with underline
------------------------

**Bad**

We cannot use the usual header formatting used by Markdown with `#` with reST:

# this should be a header


Inline code
===========

Using single backticks should be ok `code();`. 

In the documenation we often use backticks with a textrole, e.g. :php:`code();`. 

Since we want to use a minimal subset here, we should stick with single backticks!


Notes, hints etc.
=================

Do not use them, e.g. 

.. hint:: 

   This is a hint
