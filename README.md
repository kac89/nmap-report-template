# nmap-report-template
A Nmap XSL implementation with Bootstrap.

## How to use

- Add the `nmap-template.xsl` as stylesheet to your Nmap scan. 
- Example: 

```sh
nmap -sS -T4 -A -sC -oA scanme --stylesheet https://raw.githubusercontent.com/kac89/nmap-report-template/master/nmap-template.xsl scanme.nmap.org scanme2.nmap.org
```

- Open the scanme.xml with your Web browser.
- Alternatively you can transform the xml to html with

```sh
xsltproc -o scanme.html nmap-template.xsl scanme.xml
```
- You will need to download the nmap-template.xsl beforehand.

## Old scans

- You can also format old scans with the xsl stylesheet.
- Insert `<?xml-stylesheet href="https://raw.githubusercontent.com/kac89/nmap-report-template/master/nmap-template.xsl" type="text/xsl"?>` after `<!DOCTYPE nmaprun>`.

## Author

All credits go to: https://github.com/honze-net/nmap-bootstrap-xsl
I only modify structure and add anchor links.
