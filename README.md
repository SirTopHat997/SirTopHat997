<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SVG Website</title>
</head>
<body>
    <svg width="400" height="200" xmlns="http://www.w3.org/2000/svg">
        <rect width="100%" height="100%" fill="lightblue" />
        <foreignObject x="50" y="50" width="300" height="100">
            <div xmlns="http://www.w3.org/1999/xhtml" style="text-align:center; color:white; font-size:24px;">Welcome to My SVG Website!</div>
        </foreignObject>
    </svg>

    <h1>About Me</h1>
    <p>This is a simple HTML website with SVG elements included.</p>

    <h2>Some SVG Shapes</h2>
    <svg width="400" height="100" xmlns="http://www.w3.org/2000/svg">
        <foreignObject x="10" y="10" width="80" height="80">
            <div xmlns="http://www.w3.org/1999/xhtml" style="background-color:orange; width:80px; height:80px; border-radius:50%;"></div>
        </foreignObject>
        <foreignObject x="120" y="10" width="80" height="80">
            <div xmlns="http://www.w3.org/1999/xhtml" style="background-color:green; width:80px; height:80px;"></div>
        </foreignObject>
        <foreignObject x="230" y="10" width="80" height="80">
            <div xmlns="http://www.w3.org/1999/xhtml" style="background-color:blue; width:80px; height:80px;"></div>
        </foreignObject>
        <foreignObject x="340" y="10" width="80" height="80">
            <div xmlns="http://www.w3.org/1999/xhtml" style="background-color:red; width:80px; height:80px;"></div>
        </foreignObject>
    </svg>

    <h2>Contact Me</h2>
    <p>You can reach out to me at myemail@example.com</p>
</body>
</html>
