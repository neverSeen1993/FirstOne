<!DOCTYPE html>
<html>
<head lang="en">
    <meta charset="UTF-8">
    <title>Happy Birthday</title>
    <script src="https://code.jquery.com/jquery-2.1.1.min.js"></script>
</head>
<body align="center">
<div id="header">
    <h1>HAPPY BIR...</h1>

    <h3>Wait a bit, are you real Masha?</h3>
</div>
<div id="final" style="display: none; margin-top: 15%">
    <p style="font-size: 25px">Looks like you are real Masha</p>
    <p>Well, then..</p>
    <p style="font-size: 45px; font-weight: bold">HAPPY BIRTHDAY</p>
    <hr>
    <p style="font-size: 10px">I hope you will never be testing my code ;) </p>
</div>
<br><br><br>
<button id="iam" style="font-size: 80px">YES I AM</button>
<div id="test1" style="display: none">
    <h2>What is the best color?</h2>

    <div id="v1" style="margin-left: 45%; width: 100px; height:100px; background-color: indigo "></div>
    <br>

    <div id="v2" style="margin-left: 45%; width: 100px; height:100px; background-color: darkolivegreen "></div>
    <br>

    <div id="v3" style="margin-left: 45%; width: 100px; height:100px; background-color: saddlebrown"></div>
    <br>
</div>

<div id="test2" style="display: none">
    <h2>Who is this?</h2>
    <img src="http://cs11379.vk.me/u78864207/-6/x_90b00023.jpg"><br><br>
    <button id="a1" style="font-size: 20px">Yavorskii</button>
    <br><br>
    <button id="a2" style="font-size: 20px">Tiger</button>
    <br><br>
    <button id="a3" style="font-size: 20px">Zoshenko</button>
    <br><br>
    <button id="a4" style="font-size: 20px">Suprun</button>
    <br><br>
</div>

<div id="test3" style="display: none">
    <h2>What language is this test written on?</h2>
    <button id="h1" style="font-size: 20px">C,C++,C#</button>
    <br><br>
    <button id="h2" style="font-size: 20px">Lisp, PROLOG</button>
    <br><br>
    <button id="h3" style="font-size: 20px">Fu**ing JAVA</button>
    <br><br>
    <button id="h4" style="font-size: 20px">HTML JavaScript</button>
    <br><br>
    <button id="h5" style="font-size: 20px">None of the above</button>
    <br><br>
</div>

</body>
<script type="text/javascript">
    $("#iam").click(function () {
        if (confirm("Lets check this")) {
        $("#iam").css("display", "none");
        $("#test1").css("display", "block");
        $("#v1").click(function () {
            if (confirm("CORRECT")) {
                $("#test1").css("display", "none");
                $("#test2").css("display", "block");
                $("#a1").click(function () {
                    alert("I'm sorry");
                });
                $("#a2").click(function () {
                    alert("It's definitely not!");
                });
                $("#a3").click(function () {
                    if (confirm("WELL DONE")) {
                        $("#test2").css("display", "none");
                        $("#test3").css("display", "block");
                        $("#h1").click(function () {
                            alert("Saharov would kill you for this answer");
                        });
                        $("#h2").click(function () {
                            alert("Gromova is a bit happier now, but this IS NOT CORRECT");
                        });
                        $("#h3").click(function () {
                            alert("Are you realy QA?");
                        });
                        $("#h4").click(function () {
                            if (confirm("CONGRATULATIONS")) {
                                $("#test3").css("display", "none");
                                $("#header").css("display", "none");
                                $("#final").css("display", "block");
                            }
                        });
                        $("#h5").click(function () {
                            alert("WRONG!");
                        });

                    }
                });
                $("#a4").click(function () {
                    alert("Error");
                })
            }
        });
        $("#v2").click(function () {
            alert("NOPE");
        });
        $("#v3").click(function () {
            alert("WRONG");
        });
        }
    })
</script>
</html>
