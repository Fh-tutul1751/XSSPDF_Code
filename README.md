Abstract

PDF documents and PDF generators are ubiquitous on the web, and so are injection vulnerabilities. Did you know that controlling a measly HTTP hyperlink can provide a foothold into the inner workings of a PDF? In this paper, you will learn how to use a single link to compromise the contents of a PDF and exfiltrate it to a remote server, just like a blind XSS attack.

I'll show how you can inject PDF code to escape objects, hijack links, and even execute arbitrary JavaScript - basically XSS within the bounds of a PDF document. I evaluate several popular PDF libraries for injection attacks, as well as the most common readers: Acrobat and Chrome's PDFium. You'll learn how to create the "alert(1)" of PDF injection and how to improve it to inject JavaScript that can steal the contents of a PDF on both readers.

I'll share how I was able to use a custom JavaScript enumerator on the various PDF objects to discover functions that make external requests, enabling me to to exfiltrate data from the PDF. Even PDFs loaded from the filesystem in Acrobat, which have more rigorous protection, can still be made to make external requests. 
