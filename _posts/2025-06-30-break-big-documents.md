Large documents are hard to maintain, slow to read, and difficult to navigate. Instead of creating monolithic files, split content into smaller, focused documents.

Why Smaller Docs Are Better

- Improved Readability: Shorter documents reduce cognitive load.
- Faster to Find: Readers open only what they need.
- Easier to Update: Changes affect only one section, not an entire file.
- Better Collaboration: Multiple people can edit different parts without conflicts.

## How to Split Effectively

### By Topic or Function

Divide content based on its purpose: A single file "Project-Guide.md" with 50 pages covering several topics can be turned into a list of documents:

- `Setup.md`
- `Backend.md`
- `Frontend.md`
- `Depployment-Guide.md`

### By Audience

Tailor docs to specific readers:

- End Users: `User-Manual.md`
- Developers: `Setup.md`, `Backend.md`, `Frontend.md`
- Admins: `Deployment-Guide.md`,
- ...

### Use Links, Not Duplication

Instead of repeating details, link to dedicated docs:

``` markdown

## Deployment  
For cloud setup, see [Cloud-Configuration.md](./Cloud-Configuration.md).  
For on-premise, see [On-Premise-Guide.md](./On-Premise-Guide.md).  
```

### Keep a Logical Flow

Ensure smaller docs still connect:

- Throughout the document add links to other especialized documents.  
- Add a section to Related Documents.
- Connect all documents to the [single starting point](https://edumco.github.io/mini-docs/single-starting-point/)

## Set Size Limits

- Around 500 words: Gives about 3min reading (attentions decreases around 10 min)¹
- Printable: 2...3 pages (front and back)
- Correct media: Sometimes a video, a gif or a print is a better way of describing setups and other processes.  

## Combining all

### Before (Monolithic)

A single document with several goals, publics and editors: `Project-Overview.md`

### After (Modular)

Multiple documents and each one of them has a single and clear goal, public and editor:

- `User-Manual.md`
- `Quickstart.md`
- `Setup.md`
- `Backend.md`
- `Frontend.md`
- `Deployment-Guide.md`
- `Reporting-Bugs.md`
- `Collecting-Bug-Evidences.md`
- `Frontend-Test-Automation.md`
- `Backend-Test-Automation.md`
- `Performance-Tests.md`

## References

1 - [Attention span during lectures: 8 seconds, 10 minutes, or more? - journals.physiology.org/doi/pdf/10.1152/advan.00109.2016](https://journals.physiology.org/doi/pdf/10.1152/advan.00109.2016)
