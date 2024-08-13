<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Running Text</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="marquee">
        <p>I LOVE U</p>
    </div>
</body>
</html>

body {
    margin: 0;
    padding: 0;
    font-family: Arial, sans-serif;
    background-color: #000;
    color: #fff;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    overflow: hidden;
}

.marquee {
    white-space: nowrap;
    overflow: hidden;
    box-sizing: border-box;
}

.marquee p {
    display: inline-block;
    padding-left: 100%;
    animation: marquee 10s linear infinite;
    font-size: 2em;
}

@keyframes marquee {
    0% { transform: translateX(100%); }
    100% { transform: translateX(-100%); }
}
