## Note

1. Memilih bagian mana yang mau CSS selector pilih atau rapihkan (Contoh paragraf):
```css
    p{
        color: red;
    }
```

2. Memilih bagian secara spesifik dengan CSS selector dan html class(Contoh paragraf dan div):
```html
    <!--html code-->
    <p class="class_name"> </p>

    <div class="error">I am an error</div>
```
```css
    /* css code access class, start with dot */
    .class_name{
        color: red;
    }
```

3. Memilih lebih spesifik yang mau di style dengan CSS selector dan html class:
```html
    <!--html code-->
    <p class="class_name"> </p>

    <div class="error">I am an error</div>
```
```css
    /* css code access class, maka yang warnanya merah hanya paragraf saja */
    p.class_name{
        color: red;
    }
```

4. Memilih spesifik yang mau di style dengan CSS selector dan dua html class:
```html
    <p class="name_class1 name_class2">test</p>
```
```css
    p.name_class1.name_class2{
        border: 1px dashed green;
    }
```

5. Memilih bagian mana yang mau CSS selector pilih dengan ID tetapi ID biasa digunakan untuk *JavaScript*:
```html
    <p id="id_name">test</p>
```
```css
    #id_name{
        border: 2px dashed green;
    }
    
    div#id_name{
        border: 2px dashed blue;
    }
```

6. Menampilkan secara inheritance:
```html
    <div>
        <p>test1</p>
    </div>
    <p>test2</p>
```
```css
    /* maka warna merah yang ada di dalam div */
    div p{
        color: red;
    }
```
7. Memilih dengan syarat attribut secara spesifik:
```html
    <a href="www.google.com">link</a>
    <a href="www.twitter.com">twitter</a>
```
```css
    a[href*="google"]{
        background-color:green;
    }
```

8. Memilih dengan syarat attribut yang value belakangnya .com. Hal ini berguna untuk menandakan PDF download atau PDF Icon:
```html
    <a href="www.google.com">link</a>
    <a href="www.twitter.com">twitter</a>
```
```css
    a[href$=".com"]{
        background-color:green;
    }
```

9. Inherit beberapa atributt:
```html
    <div>
        test1
        <p>test2</p>
        <p>test3</p>
    </div>

```

```css
div{
    color: lightcoral;
    border: 1px solid grey;
    margin: 40px;
    font-weight: bold;
}
p{
    border: inherit;
    margin: inherit;
    color: crimson;
}
```
