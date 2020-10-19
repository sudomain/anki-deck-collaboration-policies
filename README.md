# anki-deck-collaboration-policies
Policies and strategies for collaboration on Anki decks. These are the policies I (hopefully) adhere to for decks that I maintain. Inspired by the docs of the [Ultimate Geography deck](https://github.com/axelboc/anki-ultimate-geography). Suggestions are welcome (please open an issue).

## Version Controlling of Source Material
Decks based on a piece of actively developed software (whether a language such as Python or an application such as Anki) will inevitably become out-of-date. To remedy this, collaborative should keep track of the version of each document that is used as source material for a deck. If you're working with multiple sources, then ideally each note of the deck will have a tag containing a URL pointing to a source at a specific version.
TODO: demo the `SV::` tags, getting a GH URL to point at a specific commit. and URL's from the internet archive for sources not managed by git

### Git shallow clones
When a collaborative deck is started, you usually you won't need to track the full history of the source material. You probably only need to track changes made to certain documents after a certain commit. Shallow clones can be utilized to save disk space of collaborators while still allowing to track changes.
TODO: demo

### URL's via the internet archive
For non-git based sources you can create a snapshot on the internet archive.

## Translations
Different git branch for each translation? More research needed
