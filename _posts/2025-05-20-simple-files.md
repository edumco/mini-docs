While rich text editors can create visual pleasing documents, they impose their own file formats that in most of the case aren't 100% compatible with other editors. This causes inconsistent formatting and even file corruption not mentioning the vendor lock in situations.

To avoid all these issues we can use plain text file formats (files that contain only text characters formatted in a human readble manner).

## .txt

The simplest format of all. Can be used with different character sets via encodings, but the file itself doesn’t declare its encoding—the program reading it must know (or guess) the correct one. UTF-8 is the modern standard for maximum compatibility.

This causes some problems when teams using different text editors or working across regions and languages.

## .html

More versatile than txt. Has several forma options allowing to create more organized documents.

Can be read with a browser or edited with any text editor. Some document systems accept them as a valid input format and some editors help with the tags.

The support for multiple characters is more robust cause the file can have a dedicated tag to the used charset.

## .md

The markdown format is a good balance between the simplicity of txt and the flexibility of html.
