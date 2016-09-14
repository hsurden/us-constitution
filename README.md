# us-constitution
United States Constitution in xml and JSON

This is a beta version of the US Constitution in xml and JSON.   A website using a version of this file can be found here http://www.harrysurden.com/projects/visual/USCode_D3/constitution/US_Constitution_Tree.html

(Update: Some time after I released this unofficial version, [Congress released an official version of the U.S. Constitution in xml - located here](https://github.com/usgpo/house-manual/blob/master/114/original-file-names/constitution.xml).  You may prefer that official version to this unofficial one).

For the US Constitution in XML
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
