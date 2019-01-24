---
layout: post
title:      "Inline Styling ~ REACT"
date:       2019-01-24 19:34:23 +0000
permalink:  inline_styling_react
---

Although I recommend conducting the majority of your styling for your React project  in your App.css file, there are time when inline styling is more convenient. For instance, if there is just one dimension or small feature you wish to change and make clear in the component. 

Inline styling goes within our opening tag. For instance, if I were styling a ‘p’ tag:

< p style={{ width: '75%'}}>Hello, World!</p>

As you can see, “style=” is followed by two sets of curly brackets that hold your specifications. If you need to include more than one specifications, separate with commas. 


< p style={{ width: '75%', margin= ‘auto’}}>Hello, World!</p>

Remember that the dimensions need to be in quotation marks and cannot stand alone as they would in your .css file. 

Another thing to make note of:

If your specification is more than one word, use must use camel case. For instance, “padding-top” would become “paddingTop.”

