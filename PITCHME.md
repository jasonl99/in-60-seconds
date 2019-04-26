---
## Basic Sorting

Most languages have a 
simple method of sorting 
a list of data.

In ruby, for exampe, 

```ruby
values = [1,6,2,9,0]
values.sort

=> [0,1,2,6,9]
```

---
We can sort just about anything:

```ruby
values = ["Cat", "Dog", "Apple"]
values.sort

=> ["Apple", "Cat", "Dog"]
```


---

### XBRL, my Fuckle Friend

(that's a typo, I swear)

XBRL can have multiple values for the exact same thing.

---

For example, a note may reference a bank balance at the end
of a period of "$1.2 million" 
but in a statement it's shown as $1,235,600.

---

The data in the xbrl would look 
like this (underscores work like commas in ruby)

```ruby
[1_200_000, 1_235_600]
```

---

So maybe it will sort with the most precise
first (1_235_600 is more precise if it wasn't obvs)

```
 values = [1_200_000, 1_235_600]
 values.sort

 =>  [1200000, 1235600]
 ```

 Crap.

---

## Add Some Slide Candy

![](assets/img/presentation.png)

---
@title[Customize Slide Layout]

@snap[west span-50]
## Customize Slide Content Layout
@snapend

@snap[east span-50]
![](assets/img/presentation.png)
@snapend

---?color=#E58537
@title[Add A Little Imagination]

@snap[north-west]
#### Add a splash of @color[cyan](**color**) and you are ready to start presenting...
@snapend

@snap[west span-55]
@ul[spaced text-white]
- You will be amazed
- What you can achieve
- *With a little imagination...*
- And **GitPitch Markdown**
@ulend
@snapend

@snap[east span-45]
@img[shadow](assets/img/conference.png)
@snapend

---?image=assets/img/presenter.jpg

@snap[north span-100 headline]
## Now It's Your Turn
@snapend

@snap[south span-100 text-06]
[Click here to jump straight into the interactive feature guides in the GitPitch Docs @fa[external-link]](https://gitpitch.com/docs/getting-started/tutorial/)
@snapend
