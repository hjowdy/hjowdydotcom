---
title: "Hello, friend."
date: "1986-09-17"
author: "Elliot"
cover: "img/cob-sheet.jpg"
draft: false
description: "Hello, friend? That's lame. Maybe I should give you a name?"
---

> Hello, friend? That's lame.
> Maybe I should give you a name.
> But that's a slippery slope.
> You're only in my head.
> We have to remember that...
> Shit.
> It's actually happened.
> I'm talking to an imaginary person.[^1]


This is an example post. You can write about anything, or nothing.

Some advice:

# Be Liberal With Headings
It's vry helpful. But don't be clickbaity. Tell something true. Or something wildy false. 

## Subheadings, too.

Good for seugueing.[^2]

For instance, here is my one-and-only attempt at COBOL. Notice that COBOL makes even the otherwise pleasant-looking code formatting appear *off*:


{{< highlight go "linenos=table,hl_lines=420,linenostart=418"  >}}

       IDENTIFICATION DIVISION. 
       PROGRAM-ID. HELLO.
       PROCEDURE DIVISION.
           DISPLAY "Hello, friend."
           END PROGRAM HELLO.

{{< / highlight >}}

What a mess. But hej, as the famed computer scientist Edsger Dijkstra once said about COBOL: "...you can either fight the disease or pretend it does not exist."[^3]

Here is an example of a modern language ([Golang](https://go.dev/)) with some really cool formatting:

```go "linenos=table,hl_lines=420,linenostart=415" >}}

package database

import "postapi/app/models"

func (d *DB) CreatePost(p *models.Post) error {
	res, err := d.db.Exec(insertPostSchema, p.Title, p.Content, p.Author)
	if err != nil {
		return err
	}

	res.LastInsertId()
	return err
}
```

# Conclusion

End your rambling already.

[^1]: *Mr. Robot* S01E01
[^2]: Should be *segueing*. It's also a great idea to use some kind of spellcheck. 
[^3]: He also said that "the use of COBOL cripples the mind; its teaching should, therefore, be regarded as a criminal offence." Quite harsh.[^4] See: [*How do we tell truths that might hurt?*, Edsger W. Dijkstra](https://www.cs.virginia.edu/~evans/cs655/readings/ewd498.html)

[^4]: Lest you think he was singling out COBOL, he also said: "FORTRAN --'the infantile disorder'--, by now nearly 20 years old, is hopelessly inadequate for whatever computer application you have in mind today: it is now too clumsy, too risky, and too expensive to use."[^5]

[^5]: Do *not*, like me, engage in the pure degeneracy that is the nested footnote.  

