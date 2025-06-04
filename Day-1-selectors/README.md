# Selectors in CSS

**1. Tagname/Element/Type Selectors**

     ``` css

     p{
        color: green;
     }

     ```

**2. Universal selectors**

     ``` css

     *{
        margin: 0;
        padding: 0;
        box-sizing: border-box;
     }

     ```

**3. className selectors**

   ```html

    <p class='brand'> Sole Shoe Company </p>

   ```

   ```css
   
   .brand{
      font-size: 3rem;
   }

   ```

**4. ID selectors**

``` html

   <h1 id='large-title'> Hello world </h1>

```
**5. Group & Combinators**

- Group selector: h1, p, a { ... }
- Descendant: div p
- Child: div > p
- Adjacent sibling: h1 + p
- General sibling: h1 ~ p

**6. Attribute selectors**

``` html

   <img src = '/img/seasons/cold/winter.jpg'>
   <img src = '/img/seasons/warm/summer.jpg'>

```

``` css

    img[src*= 'winter'] /* will look for src attribute with string containing as 'winter' and apply the ruleset */
    {
      height: 50px;
    }

    img[src*= 'summer'] /* will look for src attribute with string containing as 'summer' and apply the ruleset */
    {
      height: 100px;
    }

```

**7. CSS pseudo classes**
- :focus
- :visited
- :disabled
- :active 

``` css syntax

    element_name : pseudo_class_name
    {
      #css property
    }

```

**CSS Specificity Rules**

Id selectors > class selectors > tagName selectors