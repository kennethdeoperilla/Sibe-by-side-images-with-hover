# Sibe-by-side-images-with-hover
This is a part my self-learning web development. I tried to make a simple gallery and add hover on the images.


HTML:


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="./css/style.css">
</head>
<body>
        <div class="container">

            <img class="banner-img" src="./images/banner.jpg" alt="banner">
            <div class="centered">Text</div>

     
        <div class="wrapper">
            <div class="column">
                <div class="overlay1">
                <img class="image1" src="./images/1.jpg" alt="1">
                <div class="image-overlay1">
                    <div class="image-title">IMAGE</div>
                        <p class="image-description">
                            Here we have a sample pic
                        </p>
                </div>
                </div>
            </div>



           <div class="column">
                <div class="overlay2">
                <img class="image2" src="./images/2.jpg" alt="2">
                <div class="image-overlay2">
                    <div class="image-title">IMAGE</div>
                        <p class="image-description">
                            Here we have a sample pic
                        </p>
                </div>
                </div>
            </div>

            <div class="column">
                <div class="overlay3">
                <img class="image3" src="./images/3.jpg" alt="3">
                <div class="image-overlay3">
                    <div class="image-title">IMAGE</div>
                        <p class="image-description">
                            Here we have a sample pic
                        </p>
                </div>
                </div>
            </div>

        </div>
        </div>

</body>
</html>




CSS:


.container{
    width: 100vh;
    margin: auto;
    position: relative;
    
}

.banner-img{
    position: relative;
}

.centered {
    position: absolute;
    top: 33%;
    left: 50%;
    transform: translate(-50%, -50%);
    font-family: Arial, Helvetica, sans-serif;
    font-size: 44px;
    font-weight: bold;
    color: white;
  }

.wrapper{

    width: 100vh;
    display: flex;
}

.column{
    flex: 33.3%;
    padding: 5px;

}

/* Image 1 */

.overlay1{
    width: 100%;
    position: relative;
}

.image1{
    display: block;
    width: 100%;
}

.image-overlay1{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.6);
    color: #ffffff;
    font-family: 'Quicksand', sans-serif;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    opacity: 0;
    transition: opacity 0.25s;
}

.image-overlay1:hover{
    opacity: 1;
}

/* Hanggang dito Image 1*/

/* Simula ng image 2*/

.overlay2{
    width: 100%;
    position: relative;
}

.image2{
    display: block;
    width: 100%;
}

.image-overlay2{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.6);
    color: #ffffff;
    font-family: 'Quicksand', sans-serif;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    opacity: 0;
    transition: opacity 0.25s;
}

.image-overlay2:hover{
    opacity: 1;
}

/* Hanggang dito image 2*/


/* Simula ng image 3*/

.overlay3{
    width: 100%;
    position: relative;
}

.image3{
    display: block;
    width: 100%;
}

.image-overlay3{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(0, 0, 0, 0.6);
    color: #ffffff;
    font-family: 'Quicksand', sans-serif;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    opacity: 0;
    transition: opacity 0.25s;
}

.image-overlay3:hover{
    opacity: 1;
}
