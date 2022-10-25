# srcML v1.0.0

This is a major release with changes from previous alphas and betas. The following
is now versioned at 1.0.0

* The srcML tag set
* The srcML library C API, libsrcml
* The command-line client, srcml

Minor changes include:
* Options to the client, srcml
* The interface for transformations in libsrcml

Major changes are primarily markup:
* The if-stmt has been redesigned to handle nested and non-nested if
  statements in a similar manner. This includes a new &lt;if-stmt&gt; element,
  and the removal of the &lt;then&gt; element.
* The &lt;block&gt; now has a &lt;block_content&gt; inside of the block delimiters
  (e.g., '{' and '}'). This makes it easy to grab the contents of a block and not have
  to strip the '{' and '}'.
* Going back a few releases, for compound statements (e.g., if, while, for, etc.) without
  a block, a pseudo-block is added. This is a block with a type attribute &lt;pseudo&gt;.
