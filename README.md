# Convert-Text-File-to-PDF-using-Python
How to Convert Text File to PDF using Python

n this article i will show you How to Convert Text File to PDF using Python. FPDF is a Python Module that allows generating PDF files with Python code. It is free to use and it does not require any API keys. FPDF stands for Free PDF. It means that any kind of modification can be done in PDF files.

To install the fpdf module type the belwo command in the terminal.
```python
pip install fpdf
```
Then use the code below to change text file to pdf file

```python
from fpdf import FPDF

#save FPDF() class into a variable pdf
pdf = FPDF()

#add a page
pdf.add_page()

#set style and size of the font you want
pdf.set_forn("Arial", size=15)

#open the text file in read mode
f = open("techcvr.txt", "r")

#insert the text in pdf
for x in f:
    pdf.cell(200, 10, txt = x, ln = 1, align = 'C')

#save the pdf with name .pdf
pdf.output("techcvr.pdf")
```
Enjoy : )
