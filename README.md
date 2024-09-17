# heart-animation
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <title>I Love You</title>
    <style>
      body, html {
        margin: 0;
        padding: 0;
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: white;
        font-family: Arial, sans-serif;
      }
      .heart {
        position: relative;
        width: 300px;
        height: 300px;
      }
      .heart::before,
      .heart::after {
        content: "";
        position: absolute;
        top: 0;
        width: 150px;
        height: 240px;
        background: pink;
        border-radius: 150px 150px 0 0;
      }
      .heart::before {
        left: 150px;
        transform: rotate(-45deg);
        transform-origin: 0 100%;
      }
      .heart::after {
        left: 0;
        transform: rotate(45deg);
        transform-origin: 100% 100%;
      }
      .heart-text {
        position: absolute;
        width: 100%;
        text-align: center;
        top: 40%;
        font-size: 2em;
        z-index: 1;
        color: white;
      }
    </style>
  </head>
  <body>
    <div class="heart">
      <div class="heart-text">I love you</div>
    </div>
  </body>
</html>
