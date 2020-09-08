# Introduction to markup as a way to structure and interpret text

In order to be able to create links between words and different texts, sort them by date, identify authors and provide additional context, certain sections of each text in need to be highlighted and enriched with meta-information. This process is called text encoding, and the standard procedures used to encode text are markup languages. The most commonly used markup for digital text-based editions in the humanities is XML.

# Writing and editing XML with XML editors

Although XML can be written with any standard plain text editor, special XML editors foster correct syntax and include special features for the parsing and analysis of XML files.

[OXYGEN](https://www.oxygenxml.com/), a very popular and elaborate XML used for many scholarly editions worldwide, requires a paid licence while other editors are open source.

![Oxygen interface](https://www.oxygenxml.com/img/tei_editor_big.jpg)

WIKIPEDIA provides a handy [overview of XML editors](https://en.wikipedia.org/wiki/Comparison_of_XML_editors), detailing their functionality and their compatibility with different operating systems.

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
