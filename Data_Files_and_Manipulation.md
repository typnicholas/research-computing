Data Files and Manipulation
========================================================
author: Brian High
date: 2014-12-23
transition: fade

Research Computing and Data Management
-------------------------------------------------------
[http://github.com/brianhigh/research-computing](http://github.com/brianhigh/research-computing)

<small style="font-size:.5em">
This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.<br />
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a>
</small>

Data File Types
========================================================

Two main categories of files:
- Binary
- Plain Text

Important considerations:
- layout
- filename extensions

Binary Files
========================================================

- May be efficient (compressed)
- Often proprietary format ("opaque")

Plain Text Files
========================================================

Character [Encodings](http://en.wikipedia.org/wiki/Character_encoding#Common_character_encodings):
- ASCII
- UTF-8 (Unicode)

ASCII formatted files are ...
- Usually open, standard, and "transparent"

Unicode formatted files are ...
- Like ASCII, but support many more character sets

Example: XML
========================================================

- Plain Text
- Self-describing
- Structured
- Standard
- Easy to parse
- Example: xlsx

Delimited Text Files
========================================================

A delimiter is used to separate the fields (columns).

Delimiter may be ...
- Comma (CSV)
- Tab (TSV) 

Sometimes the data records span multiple lines (rows).

- Example: Genomics file formats:
  * [FASTA](http://en.wikipedia.org/wiki/FASTA_format)
  * [FASTQ](http://en.wikipedia.org/wiki/FASTQ_format)

Data File Considerations
========================================================

- Layout:
  * Structure data files as simple "columns and rows"
- Filename extensions: 
  * The letters after the (last) dot (period)
- File type associations: 
  * Determines which application opens a file


Data File Manipulation
========================================================

Conversion and Pipelines:

- ETL: extract, transform, and load
- Data cleanup is 90% of the work
- Pipelines: link utilities together to transform data streams

Command Line Interface (CLI) Pipes
========================================================

- Use special character (e.g., "pipe", |) to separate commands
- Data output from one command streams into next
- Example utilities: cut, rt, sed, "one-liners", scripts

File Conversion Utilities
========================================================

- Domain-Specific Utilities
 * Genomics
 * markup-conversion
- Conversion utilities: 
  * Csvkit, Rio
  * See : http://goo.gl/H6PhfS
