Sometimes the same information is relevant in several places and we are tempted to connect the dots by copying the data around.

This approach has a big failure: When you need to update the information it's hard to find all occurrencies!

So to keep our documents as minimal as possible we should use 3 technics: references, links and embeds.

## References

This is the first form of deduplication on documents. Instead of copying some part of a document you only say where you should look for more information.

Ex.:
```
For more information on this topic look for the **Onboarding Documentation** on page 6.
``` 

Although this is the way of connecting information in books and articles you need to search for the other content and sometimes its not easy to find them.

## Links

Links are the digital way of reference, not only the link tells you where to find the information but also get you instantaneosly to the information.

Links can be used in conjunction with references so the description of the link describes the reference and link gets you there.

Ex.:

Markdown: 
```markdown
  [Reference in scholarship context - Article on Wikipedia](https://en.wikipedia.org/wiki/Reference#Scholarship)
```
Result: 

  [Reference in scholarship context - Article on Wikipedia](https://en.wikipedia.org/wiki/Reference#Scholarship)
  
## Embeds

Embeds are a special type of link that is used to bring the content form other pages instead of redirecting the user to other page.

Ex.:

Markdown:
```
[![Watch the video](https://img.youtube.com/vi/G3Cytlicv8Y/maxresdefault.jpg)](https://www.youtube.com/watch?v=G3Cytlicv8Y)
```
Result:

[![Watch the video](https://img.youtube.com/vi/G3Cytlicv8Y/maxresdefault.jpg)](https://www.youtube.com/watch?v=G3Cytlicv8Y)
