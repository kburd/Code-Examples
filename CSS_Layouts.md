```css


/* Desktop Display */
@media screen and (min-width: 1250px){
    .leftCol{
        width:25%;
        float: left;
    }
    .centerCol{
        width: 50%;
        float: left;
    }
    .rightCol{
        width: 25%;
        float: left;
    }
    .footer{
        clear: both;
    }
}

/* Mobile Display */
@media screen and (max-width: 1250px){
    .centerCol{
        padding: 0% 5%;
    }
}

@keyframes colorChange {
    0%   {color:red; text-align: left;}
    33%  {color:yellow; text-align: center;}
    50%  {color:green; text-align: right;}
    66%  {color:yellow; text-align: center;}
    100% {color:red; text-align: left;}
}

.coolHeader {
    animation-name: colorChange;
    animation-duration: 6s;
    animation-iteration-count: infinite;
    color: red;
}

div {
    text-align: center;
}

.header{
    /* background-color: purple; */
}

.leftCol{
    background-color: red;
    animation-name: colorChange;
    animation-duration: 6s;
    animation-iteration-count: infinite;
}

.centerCol{
    background-color: green;
}

.rightCol{
    background-color: blue;
    animation-name: colorChange;
    animation-duration: 6s;
    animation-iteration-count: infinite;
}

.footer{
    background-color: yellow;
}
```

```html
<!DOCTYPE html>
<html>
    <head>
        <link rel="stylesheet" href="index.css">
    </head>
    <body>
        <div class="header">
            Header
        </div>
        <div class="leftCol">
            <img src="The_Eminem_Show.jpg">
        </div>
        <div class="centerCol coolHeader">
            <h1 class="coolHeader">Center Column</h1>
            <p>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut hendrerit mi ut orci ultrices tempus. Vestibulum et velit et lectus tempus aliquet vitae et risus. Integer luctus lobortis libero, nec eleifend lacus. Aliquam faucibus aliquam purus, et mattis lorem tempus in. Nulla facilisi. Nam a mattis risus. Praesent blandit posuere augue, vitae aliquam nibh molestie id. Nulla vitae dapibus tellus. In pharetra diam id dictum euismod. Morbi id nisi et elit accumsan blandit vel vitae enim.

Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Mauris ipsum purus, efficitur sit amet nunc vel, vulputate posuere mi. Aliquam at nisl id orci mollis sodales quis id velit. Curabitur ornare mauris eu nisi blandit condimentum. Donec iaculis pulvinar nulla, id interdum purus gravida id. Quisque tincidunt odio venenatis, hendrerit justo eget, dapibus sem. Duis lacinia ligula nec diam accumsan tristique. Aliquam ac diam at augue tincidunt pretium a vel turpis. Mauris dui mauris, cursus et sodales eu, faucibus quis nulla. Curabitur odio tortor, aliquet vitae placerat vitae, dignissim id diam. Mauris magna arcu, blandit pulvinar ante eget, congue lacinia mi.

Maecenas eu scelerisque metus. Phasellus non vestibulum tellus, ac vestibulum nibh. Sed vel tortor et nisl rhoncus dignissim. Nam quis nisl in velit hendrerit sagittis in sed ex. Sed fermentum nec orci nec rhoncus. Etiam pretium lacus sed diam viverra rutrum. Duis rutrum molestie ligula, non elementum urna tempus quis. Nam a euismod tortor. Donec porta quis dolor a venenatis.
            </p>
        </div>
        <div class="rightCol">
            <img src="The_Eminem_Show.jpg">
        </div>
        <div class="footer">
            Footer
        </div>
    </body>
</html>
```
