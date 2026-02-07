# project 1
## BG COLOR CHANGER

``` html css & javascript
console.log("jatin");

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Styled Page</title>
    <style>
        /* Navigation Bar */

        body {
            margin: auto;
            text-align: center;
            transition: background-color 0.3s ease;
            text-transform: capitalize;
        }

        .nav {
            background-color: gray;
            color: white;
            display: flex;
            align-items: center;
            height: 60px;
            justify-content: center;
            width: 100%;
            gap: 30px;
        }

        .nav a {
            text-decoration: none;
            color: white;
            background-color: black;
            padding: 10px 15px;
            border-radius: 5px;
            transition: 0.3s;
        }

        .nav a:hover {
            background-color: transparent;
            border: 1px solid white;
        }

        /* Box Container */
        .boxes {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
            margin-top: 20px;
        }

        /* Individual Box */
        .box {
            background-color: lightgray;
            width: 150px;
            height: 120px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: bold;
            border: 1px solid black;
            border-radius: 10px;
            cursor: pointer;
            transition: 0.3s;
        }

        .box:hover {
            transform: scale(1.1);
        }
    </style>
</head>

<body>
    <div class="nav">
        <a href="#">Home</a>
        <a href="#">YouTube Channel</a>
    </div>

    <h2>Color Scheme Changer</h2>
    <div class="boxes">
        <div class="box" id="green">click me </div>
        <div class="box" id="red">click me</div>
        <div class="box" id="blue">click me</div>
        <div class="box" id="yellow">click me</div>
        <div class="box" id="skyblue">click me</div>
    </div>

    <script>
        let buttons = document.querySelectorAll(".box");
        let bodyselect = document.querySelector("body");

        buttons.forEach(function (button) {
            button.addEventListener("click", function (e) {
                console.log(e.target); // Debugging: Log clicked element

                // with if else 

                if (e.target.id === "green") {
                    bodyselect.style.backgroundColor = e.target.id;
                }

                if (e.target.id === "blue") {
                    bodyselect.style.backgroundColor = e.target.id;
                }

                if (e.target.id === "yellow") {
                    bodyselect.style.backgroundColor = e.target.id;
                }

                if (e.target.id === "red") {
                    bodyselect.style.backgroundColor = e.target.id;
                }

                if (e.target.id === "skyblue") {
                    bodyselect.style.backgroundColor = e.target.id;
                }


// here is switch case alternative
                // switch (e.target.id) {
                //     case "green":
                //     case "red":
                //     case "blue":
                //     case "yellow":
                //     case "skyblue":
                //         bodyselect.style.backgroundColor = e.target.id;
                //         break;
                //     default:
                //         console.log("No color matched!");
                // }
            });
        });
    </script>
</body>

</html>

 ```
