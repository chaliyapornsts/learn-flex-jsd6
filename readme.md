"html"
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="./style.css">
    <title>Learn-Flex</title>
</head>
<body>
    <div class="flex-parent">
        <div class="flex-children child-1">child-1</div>
        <div class="flex-children child-2">child-2</div>
        <!-- <div class="flex-children">child-3</div>
        <div class="flex-children">child-4</div> -->
        <!-- <div class="flex-children">child-5</div>
        <div class="flex-children">child-6</div>
        <div class="flex-children">child-7</div>
        <div class="flex-children">child-8</div> -->
    </div>
</body>
</html>

"css"
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

.flex-parent{
    height: 10vh;
    width: 300px;
    background: wheat;
    display: flex;
    /* flex-direction: column; */
    /* justify-content: space-around; */
    /* align-items: center; */
   /* flex-wrap: nowrap; */
   /* flex-flow: row wrap; */
   /* align-content: space-evenly; */
   gap: 20px;
}

.flex-children{
    background-color: red;
    width: 150px;
    /* height: 100px; */
    /* aspect-ratio: 2; */
    /* สามารถใช้ 4/3 6/10 ได้ */ 
}

.child-1{
    /* flex-grow: 1;
    flex-shrink: 5;
    flex-basis: 200px; */
    /* flex: 1 5 200px; */
    flex: 1;
}

.child-2{
    flex-grow: 1;
    flex-shrink: 1;
}

.child-3{
    height: 200px;
    aspect-ratio: 1;
}

.order-1{
    order: -1;
    background: blue;
}

.self{
    align-self: flex-end;
}





"html login"
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="./style.css">
    <title>Learn-Flex</title>
</head>
<body>
    <div class="app">
        <div class="left">left
            <img src="https://www.govivigo.com/content/upload/images/1b_articles/Top%205%20highest%20mountains-1.jpg"
            alt="Photo">
        </div>
        <div class="right">
            <form class="form">
                <h1>Sign Up</h1>
                <input>
                <input>
                <button>Sign Up</button>
            </form>    
        </div>
    </div>
</body>
</html>

"css login"
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

.app{
    height: 100vh;
    /* background: wheat; */
    display: flex;
}

.left{
    /* background: green; */
    flex: 1;
}

.right{
    /* background: orangered; */
    flex: 1;
    padding: 40px;
    display: flex;
    /* flex-direction: column; */
    align-items: center;
}

.form{
    flex: 1;
    height: 50vh;
    /* background: gray; */
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
}

input{
    padding: 10px;
}

button{
    padding: 10px;
    align-self: flex-start;
    min-width: 200px;
}

img{
    /* width: 100%; */
    height: 100vh;
    object-fit: cover;
}

@media (max-width: 768px){
    .left{
        display: none;
    }
}
