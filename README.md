# libreoffice-thesis

A LibreOffice port of Dominik Menke's [Thesis Template](https://github.com/dmke/thesis-template). It has been extended with sample content and uses styles for chapters, headers, pages, and tables. Enjoy!

## Caution For Thesisers
If you plan on using LibreOffice / MS Word for your thesis, consider this path carefully. It might initially be more work to get into LaTeX but it is probably worth the effort. To achieve the same high-quality appearance (ignoring the relevancy of content) will require a careful eye for when your text editor of choice eats your formatting.

None the less, since yours truly had the constrain of NOT writting it in LaTeX, this template is the least I can do to get you on your way to writting a beautifully layouted thesis. The necessary paragraph, heading, table and page layouts have be created and mostly tested. Most changes have been backported from my current thesis, so happy thesesing (damn I love making up words).

## How-To's

### Add an image, caption it and if necessary place them side by side or above one another or in wierd matrix style:

 * Drag that image into the document
 * Right-Click → 'Insert Caption' → Caption it
 * Select caption frame and in Styles and Formatting double click 'Frame' to apply the style
   * However, if you plan on placing images side by side or above one another, create table (ctrl + F12) to match your image layout.
     * Thereby select AutoFormat and select the style Illustration Container
   * After creating the table, go to Right-Click → 'Table Properties...' → And set the spacing below to 4mm
   * Move the caption frames containing your illustrations into the cells of the table.
   * Select the frames and then set the frame style to the FrameInTable style, a substyle of the Frame style
   * Go to the illustration properties (double-click), copy the image width, go to the individual frame property, paste it into the width 
   * Hopefully nothing screwed up...

### Get a table in there
 * Copy the Coffee Table from the Tables appendix
 * Resize to need
 * The only thing that might require customizing are the following Text Flow settings (in 'Table Properties...'):
    * 'Allow table to split across pages and columns'
    * 'Allow row to break across pages and columns'
    * 'Repeat heading'

### Other Headings and Subheadings
 * Take a note of the existing headings. They consist of paragraph and page styles...

## Rants
There is not style formatting for tables! And even the limited style formatting with AutoFormat does not copy the spacing below a table. This sounds way to calm...
Also, it is not possible to let illustrations, frames and tables float as seen in LaTeX. There exists a realy old bug report: https://bugs.documentfoundation.org/show_bug.cgi?id=40879 but who knows...