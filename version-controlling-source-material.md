(note: "source material" refers to a piece of media that contains information which is used as a basis for the cards of a shared deck)

# Version Controlling of Source Material
Decks based on source material that will change over time will inevitably become out of date. This is especially true of documentation for actively developed software (whether a language such as Python or an application such as Anki). To remedy this, collaborative decks should keep track of the version of each document that is used as source material for the deck. If you're working with multiple sources, then ideally each note of the deck will have a tag containing a URL pointing to a source at a specific version. This serves a few purposes. It allows users to check where a question came from and allows them to study from only a specific source using Anki's filtered deck feature. Additionally it allows deck maintainers to more easily find cards that are affected by an update to the source material. My system utilizes this syntax:

`SV::URL`

The URL points to a public resource at a specific version. If it's a git repo, it should point to a specific tag or commit. For instance (using GitHub as an example):

`SV::https://github.com/ankitects/anki-manual/tree/5a63f208ae84c902bb39df52c22037a897d84b45`

Note that not all git hosting platforms support this, but the major ones do (typically by selecting a commit then clicking a button called "Browse files")

## Git shallow clones
When a collaborative deck is started, you usually you won't need to track the full history of the source material. You probably only need to track changes made to certain documents after a certain commit. Shallow clones can be utilized to save disk space of collaborators while still allowing to track changes.
TODO: demo

## URL's via the internet archive
For non-git based sources you can create a snapshot on the Internet Archive's [Wayback Machine](https://web.archive.org/). You can take the URL of this snapshot and add it to the notes of the deck as well as a `links.txt` file in your `sources` directory (see next section)

## The sources directory
Keep source material inside a directory called `sources/` in the root of your git repo. This will let you and collaborators manage the deck's notes created from the same version of the source material. Git repos can be added as git submodules. 

