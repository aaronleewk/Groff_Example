
# CV in "Groff"

Before there was "Word", there was "Groff"...

## What am I looking at?

"sample_CV.ms" is a CV template. Using the "Groff" program, you can turn it into a PDF file.

In this example, "sample_CV.pdf" is the resultant file.

## Sounds good! How do I do it?

First download "sample_CV.ms". Then open up your terminal and navigate to the directory containing the file. Proceed to run this command:
```
groff -ms -t -Tpdf sample_CV.ms > sample_CV.pdf
```

## Okay... but what exactly is going on?

"Groff" is a word processor*. It provides you with tools to make your text pretty. Think margins, fonts, sizing etc, the stuff that improves your reading experience. The technical term for this is "typesetting".

"sample_CV.ms" contains plain text interspersed with formatting commands. "Groff" reads the file, and when it comes across commands it recognises, it renders subsequent text in the associated formatting.

## Sounds complicated. Why "Groff"?

I like "Groff" because it makes it easy to understand formatting.

When I used "Word" to create CVs, I wanted to fit everything onto a single page. To achieve this, I adjusted the formatting quite extensively to trim my content to size.

Afterwards when I added or deleted text, these changes would not sit well with the old formatting. Alignments would go out of sync, text dimensions would look weird and once again I had to trim my content to size.

Updating the formatting was not easy. To re-format my content to the same layout as before, I had to right click, select "Paragraphs" and go through multiple property panels and tweak dimensions until, once again, everything was in its place. I hated spending time doing such investigations.

With "Groff", formatting decisions are clearly defined. I can know everything about the document's layout just from reading the commands in the source file. No more detective work! I can also recreate a document exactly from scratch, as long as I know the original document's "Groff" properties. Try recreating a Word document that has different "before text" and "after text" line spacing and paragraph spacing for each section! 
___

\* Well not exactly. A word processor presents an entire toolchain for document creation, from text editing and formatting, to spell checking, to printing. Microsoft's "Word" or Apple's "Pages" are two examples. "Groff" does not do printing or editing. It is focused on formatting. "Document preparation system" is probably a better description - see [GNU Troff Manual - What is groff?](https://www.gnu.org/software/groff/manual/html_node/What-Is-groff_003f.html)





