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

It handles multiple characters by adopting utf-8 encoding and Unicode charset by the default.

The files have a simple format and can be edited in any text editor. Lots of editors, code repository and wiki managers transform the files into web pages (parsing).

The format provides most of the structure of a document or web page like:

- Title Hierarchy (H1,H2...)
- Text emphasis (italics, bold...)
- List decorations (dots, numeric lists)
- Links, images and embedded video
- Code blocks


## References

https://www.markdownguide.org/

https://commonmark.org/

https://wordpress.com/support/wordpress-editor/blocks/markdown-block/

https://docs.github.com/en/get-started/writing-on-github

https://docs.gitlab.com/user/markdown/

https://handbook.gitlab.com/docs/markdown-guide/