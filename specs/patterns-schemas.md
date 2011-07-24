## Patterns: schema.

It would be in line with modern web standards to ensure that the
patterns published on the website conform to web standards. Some of
these are mentioned below:

 * Search Schema support (see [[schema.org|http://schema.org/Thing]])
 Patterns published on the website **SHOULD** follow microformat
specifications 
 Probably a custom subset of *Thing::Article* would be something we
could look at. 

 * RSS/Atom feeds of new patterns
 Eventually it would be a good idea to expose feeds for patterns by
topics and/or category. 

 * Template for writing patterns
 We should decide on a underlying pattern template which can be used to
write new patterns. This might evolve over time.

## Hyde variables

We use the following hyde variables in a pattern to supply metadata to our pre-processor.

{%hyde _metadata blocks must begin with this_

Title: Title of the pattern

Type: pattern _values allowed: pattern, principle, page_

Desc: This short description is a 1-2 line abstract to appear on the homepage and other shortened forms.

Categories: location, notice, smartphone, ui _tags that classify the subject matter, the purpose of the pattern, and the applicable audience_

Status: draft _values allowed: stub, draft, published_ 

Address: http://npdoty.name, @m0hit _comma-separated list of authors, or more importantly, the people to contact or blame about the content, to be displayed in an &lt;address&gt; HTML element on the page. in future, URLs may be de-referenced and hCard identities extracted; Twitter/github handles and email addresses also possible._

%} _end the metadata block with this_