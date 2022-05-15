## CSS Notes
Cascading style sheets used just for the purpose of beautifying HTML and XML files.

#### Inline CSS
This type of CSS styling involving beautifying each html tag.
##### Disadvantage
The same that we will have to style each tag, incase of any changes, remember every tag where the change has to be applied. Need something to apply CSS to whole webpage. ---> Internal CSS

#### Internal CSS
This type of CSS styling involving beautifying each html page. We can apply consistent styling to the whole page using this tag. Can be done by adding *style tag inside head tag.*
```
<head>
  <style>
  body{
    background-color : blue;
  }
  </style>
</head>
```
##### Disadvantage
Incase of 200 webpages need to copy-paste everywhere. --> External CSS
#### Notes
- Every thing on a website is just a box. That box is styled by some default CSS applied by the browser itself. Therefore, if you apply something and don't get it, check the box height and width -> *pesticide extension*.

#### External CSS
This type of CSS styling involving beautifying the tags across all the webpages. Can be done by creating a *css* folder and adding *styles.css* file inside it. the adding all the internal css code there, and then linking the style sheet to each of the page where that kind of styling is required.
Page reads it as *The link to the stylesheet is at href.*
```
<head>
  <link rel="stylesheet" href="css/styles.css" />
</head>
```
#### Debugging CSS
This is can done using chrome developer tools

#### CSS Syntax
- Selector - Who do you wanna change ?
- Key : what do you wanna change ?
- Value : How do you wanna change ?

*For easy debugging keep key1, key2 in alphabetical order.*  
```
selector {
  key1 : value1 ;
  key2 : value2 ;
}
```

#### CSS Selectors
1. Tag Selectors: These are the normal tag styling added to the whole page.
```
body{
  background-color : blue;
}
```
2. Class Selectors: When we want to add custom styling to a specific tag we use classes.
```
.classname{
  font: blue;
}
```
3. Id Selectors: When we want to style an individual tag only.
    - there can only be a unique id in one Page.
    - one tag can have only one id.
```
#idname{
  font: blue;
}
```

| Class Selector                                   |  Id Selector                                            |
| -------------                                    | -------------                                           |
| It represents how a class of tags should look.   | It represents how a individual/unique tag should only.  |
| There can be many tags with one classname.       | There can only be a unique id in one Page.              |
| One tag can have many classnames.                | One tag can have only one id.                           |
