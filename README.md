# Lex Iterata - Markdown files

[Lex Iterata](https://refli.be/fr/lex) is a project to collect and transform
the content of the Belgian Official Journal web site. It presents that content
in an enhanced format for human comprehension, while also providing structured
data tailored for machine consumption. In this Git repository, the same content
is presented as a collection of files written using the Markdown format.

The specific Markdown markup elements chosen to represent the structural
features of the legislative texts are loosely modeled on the choices made by
`OpenJustice.be` in [their work](https://github.com/openjusticebe/be_laws_fr).
For instance a Chapter is a level-3 heading, and an Article is represented in
**bold**.

## Content

The repository contains texts obtained from the Belgian Official Journal web
site, more specifically from Justel (the consolidated texts). Currently we only
generate the French version of the texts.

[Here is a link to one example
text](https://github.com/hypered/iterata-md/blob/main/texts/2016/00/2016000032.md).
You can use the "Go to file" button visible in the GitHub interface to navigate
to a specific document using its document number (e.g. 2016000032 in the
previous example). The corresponding file on Lex Iterata itself can be found by
using its number after `https://refli.be/fr/lex/`, e.g.
https://refli.be/fr/lex/2016000032.

## Updates

We have two types of updates to this repository:

- Sync, where we add new documents that appeared on Justel since the last sync.
- Full sync, where we also regenerate everything using freshly downloaded
  source documents from Justel. Those full syncs are normally created with two
  commits: one for the changes, and one for the new files.

Note: the date associated with a full sync is the date when we create the
commit in this repository. But the download time of the source documents can be
older (e.g. two days) because we download files from Justel with a 1 second
delay between each, and because manual intervention might be needed in some
cases, causing additional delay.

This repository contains 208304 legislative texts.

Last updated: 2025-12-22.
