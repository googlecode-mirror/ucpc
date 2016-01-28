uCpC (for lack of a better name) is a framework for rendering web objects in PHP programaticaly.  The desire to create such a framework was born out of my frustration of spending time writing HTML, making sure it worked in varying browsers, and repeating the same Javascript over and over again for similar
reasons.  uCpC in its infancy back in 2004 was simply a classic ASP set of functions that on the server side created an onclick="..." Javascript function that basically instantiated an XMLHTTP request, which then returned some HTML
to a specified target div.

While the spirit of what I had started back in the beginning of the AJAX craze has not changed, the functionality has matured a bit.  I started creating custom classes for repetitive HTML layouts, such as panels with titles which
basically were pseudo-windows, or 2-3 column layouts, which were always the same lines of HTML.  This allowed me to begin passing properties to the object itself and making it reusable.  This extended into about a dozen classes and
now is quickly turning into the entire DOM, from HTML all the way to SPAN, along with more complex items such as Window, Tabstrip, etc.

Why?  The purpose is to define the composition of your web application, instead of being bogged down with the presentation code.  Do not mistake this for loss
of control.  You can still change HTML attributes as easily as you would in Javascript.  You can still modify things like inline STYLE, CLASS, ID, etc as you would when writing out the tags manually. Anything that you want to tweak
you can, but why bother writing the code if you don't have to?  At its core, this framework has 2 distinct goals.

1) Focus on application functionality while reducing time spent on presentation.

2) Provide a lightweight and easy to use AJAX framework to achieve a richer end-user experience.

The watermark of these goals rises as we meet them, while not losing vision of its original purpose.  The goal is not to end up with a daunting or bloated API, but to make it easier to program.