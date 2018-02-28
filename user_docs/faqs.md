# Frequently Asked Questions
## How to specify custom MathJax script?
VNote supports a configuration `[web]/mathjax_javascript` which specifies the location of the MathJax and its configuration to use. The default value may look like this:

```ini
[web]
; Location and configuration for Mathjax
mathjax_javascript=https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.2/MathJax.js?config=TeX-MML-AM_CHTML
```

You could download the MathJax ([howto](http://docs.mathjax.org/en/latest/installation.html)) and specify a local copy of the MathJax to use, like `mathjax_javascript="/home/tamlok/Downloads/MathJax-2.7.2/MathJax.js?config=TeX-MML-AM_CHTML"`.

## How to make VNote more "portable"?
VNote will read and store configuration files in the common directory of the operating system to store application data. If you prefer to put these configuration files along with the VNote executable, you coulud copy or create the `vnote.ini` file in the directory containing VNote executable. VNote will first try to read `vnote.ini` from where the executable exists.

However, please notice that VNote will store the notebook's path in the configuration file, so it may read a wrong path and complain about errors if you copy VNote to another computer.