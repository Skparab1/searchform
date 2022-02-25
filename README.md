# Searchform
- HTML form for skparab1 search
- also testing html forms
- use at https://skparab1.github.io/searchform

# What it does
- Creates a simple ui for skparab1 search query
<img width="1024" alt="Screen Shot 2022-02-24 at 10 01 28 AM" src="https://user-images.githubusercontent.com/71990977/155581217-74be6774-b401-4618-a0e6-3329839f68fb.png">
- When 'submit' is clicked, makes string query of selected options

- However, HTML default string query format isn't the same as the one used used by skparab1 search
  - since skparab1 search defaults to true, and makes the parameters = to false
  - while html string query will default to false, and make parameters = to true
- For example, The following two are equivilant in value

````
https://skparab1.github.io/search/?game&js=true&webpage=true
````

````
https://skparab1.github.io/search/game&py=falsehtml=falsepas=falsemd=falsesv=falsesoftware=false&article=false
````

- However, the first one is generated by html form and the second one is generated by skparab1 search, so only the second woks as an input
- to solve this, /searchform will redirect to /pack, which will translate the parameters and format them to be compatible with skparab1 search
