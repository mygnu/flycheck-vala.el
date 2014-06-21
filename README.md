flycheck-vala.el
================

My simple workaround to use flycheck for vala source code.

This code has been taken and modified from https://gist.github.com/DinoChiesa/11154481

Usage
(require 'flycheck-vala)

Valac compiler syntax checker isn’t that great, but it works just fine for me. All you have to do is add following at the top of your source file

// flycheck: valac --pkg gtk+-3.0 %f

where %f is your current buffer
