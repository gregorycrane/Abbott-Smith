This directory contains the Abbott-Smith data from DSaw's digitization of Abbott-Smith, which can be found here:

http://www.biblesupport.com/e-sword-downloads/file/9282-g-abbott-smith-a-manual-greek-lexicon-of-the-new-testament/

Files:

abbott-smith.odt.content.xml   The original content of the RTF file, converted to ODF
abbott-smith.xquery            An XQuery that converts the ODF to a format like our TEI format
abbott-smith.out.xml           Output Abbott-Smith data

The XQuery is not perfect - some things should be improved in the
query, others will need to be done manually.  The first N are partial
entries - this is an artifact of the original data. Instead of
deleting this partial data, I am keeping it so it can be
cherry-picked.

αἷμα is a reasonably good benchmark entry.

The automatic conversion must meet at least these criteria:

* All text is preserved, available in the text editor
* Easy enough to figure out what went wrong
* Any remaining problems are easier to hand edit than to fix in the XQuery

Try to fix these in the XQuery:

* Correct the OSIS references
* More correct tagging (lots of things are falsely labeled
  senses). Some of this may need to be manual.

These things will need to be done manually:

1. Check for missing entries (e.g. α not auto-converted, β etc. does not seem to exist)
2. Cross-references: ἁλιεύς, see ἁλεεύς. => shows up as a sense in the previous entry,
   no Strong's number is available for these, as in the orphans. Searching for the word 'see'
   seems to find these.

