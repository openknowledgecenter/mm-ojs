# README

## Requirements

`pandoc` - Install following [these instructions](https://pandoc.org/installing.html).

## Process overview

1. Fix Word doc so that the styles applied are appopriate to the HTML that will be generated. The title of the article should be a header 1, section titles should be header 2, etc.
2. Generate HTML from the Word doc using the appropriate command below.
3. Create a new copy of the `standard-template.html`.
4. Update document title in the `<title>` tag.
5. Update issue number in `<header>` tag.
6. Copy the HTML in the `<body>` generated by pandoc into the `<main>` tag of the copied template.
7. Copy the logo HTML from `icon-snippet.html` and replace the broken HTML for the logo generated by `pandoc`.

**[Step by step process instructions are available here](https://github.com/openknowledgecenter/mm-ojs/blob/main/step_by_step.md).**

## Figures/Images and Videos

Copy the HTML from the appropriate template file into the correct place in the article or document HTML after it's been placed in the `standard-template`. Fill in the appropriate information then:

- for a video, copy the Youtube embed code into the template section
- for an image, input the correct `src`, alt text, and caption.

## Pandoc commands

`pandoc` should be run from your terminal or command prompt. You can find getting started instructions [here](https://pandoc.org/getting-started.html).

To generate a HTML file:

`pandoc filename.docx -f docx -t html -s -o outputfilename.html`

To generate a markdown file, which is _sometimes_ helpful for seeing structure and content:

`pandoc filename.docx -f docx -t markdown -o outputfilename.md`
