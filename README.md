# linuxcnc29-Docs-drafts
**Documentation: Drafts for proposals, revisions and improvements.**

Inspired by https://github.com/jnavila/git-manpages-l10n

Based on po4a at https://github.com/mquinson/po4a

How to write good documentation?
Well, this is another story. It is a matter for developers. 
This repository is focused on another aspect .... internationalization and localization; in other words, translations of good documentation. 

**Fact:** untranslated free software is useless for non-English speakers.

**Fact:** the actual translations represent a huge effort of many individuals, crippled by small technical difficulties.

Traditionally, the gettext toolsuite is used to extract the strings to be translated from a program in a standardized format (PO files or catalogs). Other tools help translators to translate these PO files. Then gettext uses the result at runtime to display the translated messages to end users. The user interface translation seems to be well resolved. 

Regarding documentation, however, the situation still somewhat disappointing. When the original documentation is modified, keeping track of the modifications quickly turns unpleasant and error prone.

Outdated translations are often worse than no translation at all: 
- End-users can be tricked by documentation describing an old behavior of the program.
- They cannot interact directly with the maintainers since they don't speak English. 
- The maintainer cannot fix the problem as they don't know every language.

po4a is a framework for translating documentation and other materials that makes it easy to maintain documentation translation using classic gettext tools and decouples content translation from its document structure. The goal of the po4a project is makes documentation translations maintainable, reusing and adapting the gettext approach to this field.
 
As with gettext, texts are extracted from their original locations and presented to translators as PO translation catalogs. 
The translators can leverage the classical gettext tools to monitor the work to do, collaborate and organize as teams. po4a then injects the
translations directly into the documentation structure to produce translated source files that can be processed and distributed just like the English files. 
Any paragraph that is not translated is left in English in the resulting document, ensuring that the end users never see an outdated translation in the documentation.

Discovering the paragraphs needing an update becomes very easy, and the process is completely automated when elements are reordered without further modification. 
Specific verification can also be used to reduce the chance of formatting errors that would result in a broken document.

**...to be continued**
