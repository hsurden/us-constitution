# us-constitution
US Constitution in XML and JSON

This is a beta version of the U.S. Constitution in xml and JSON.   A website using a version of this file can be found here http://www.harrysurden.com/projects/visual/USCode_D3/constitution/US_Constitution_Tree.html

For XML
The individual articles, amendments, and contents are labeled in xml format.

The different levels of the xml hierarchy are:
'document
  part
    article (or amendment)
      section (optional)
         paragraph
            content

 The text of the Constitution parts are located in the <content> elements.

 The JSON file is hierarchical, with each sub-part located in the "children" element.

For instance, you might have something like (some parts omitted):
  {"name":"part"
   "children":[
      {"name":"section 1"}
      {"name":"section 2"}
   ]
   }
