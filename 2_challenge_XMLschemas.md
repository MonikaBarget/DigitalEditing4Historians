# Overall purpose of XML schemas

XML schemas are a way to define XML elements specifally for one edition project or a series of related projects, e.g. editions of historical letters. Parsing XML files against the project schema ensures that the syntax and hierarchies of the files are correct and that the files will eventually display correctly on the web or in print.

# Challenges of XML schemas for historical sources

However, defining a schema also comes with many pitfalls, one of them being the premature limitation of options to describe certain textual features. The challenge especially affects editions of historical sources as pre-modern texts often use inconsistent spelling, quotes from foreign languages such as Greek and Latin, or may contain many sections that are no longer legible.

# Case study: the Letters 1916-1923 schema for early 20th-century correspondence

a) history of the collection and its infrastructure 

b) focus in Letters 1916-1923 is on encoding metadata

show frontend, backend and exported XML file

c) elements of the Letters 1916 schema are both adaptable to other collections of letters and project-specific:

https://raw.githubusercontent.com/bleierr/Letters-1916-sample-files/master/plain%20corresp%20templates/template.rng

d) PROs & CONs of specifying person and places names in the XML/TEI schema

!["persName" and values in the original Letters 1916 schema](https://github.com/MonikaBarget/DigitalEditing4Historians/blob/master/PersName_Letters1916_Schema.png)

Solution in the new infrastructure: "consecutive disambiguation"
