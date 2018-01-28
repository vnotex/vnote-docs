# Frequently Asked Questions
## How to specify custom MathJax script?
VNote supports a configuration `[web]/mathjax_javascript` which specifies the location of the MathJax and its configuration to use. The default value may look like this:

```ini
[web]
; Location and configuration for Mathjax
mathjax_javascript=https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.2/MathJax.js?config=TeX-MML-AM_CHTML
```

You could download the MathJax ([howto](http://docs.mathjax.org/en/latest/installation.html)) and specify a local copy of the MathJax to use, like `mathjax_javascript="/home/tamlok/Downloads/MathJax-2.7.2/MathJax.js?config=TeX-MML-AM_CHTML"`.