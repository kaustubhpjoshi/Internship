!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        body{
            background :silver;
            display: flex;
            align-items: center;
            justify-content: center;
            padding-top: 10rem;
        }
        .calculator{
            display:flex;
            align-items: center;
            flex-direction: column;
            justify-content: center;
            width: 290px;
            backdrop-filter: blur(16px) saturate(180%);
            border-radius: 20px;
            border:4px solid black;
            padding: 20px;
            box-shadow: 1px 3px 4px 5px rgb(8, 53, 58);
        }
        .screen{
            background-color: #033630;
            font-size: 45px;
            border-radius: 20px;
            text-align: end;
            width: 100%; 
            outline: none;
            backdrop-filter: blur(16px) saturate(180%);
            background: linear-gradient(45deg rgb(114, 114, 114)#494949);
            border-radius: 20px;
        }
        button{
            height: 40px;
            width: 70px;
            border-radius:20px;
            border:3px solid black;
            margin-top: 10px;
            background-color: black;
            color: white;
            box-shadow: 1px 1px 1px 1px white;
        }
    </style>
     </style>
</head>
<body>
       <div class="calculator">
        <div class="circle"></div>
            <div class="circle"></div>
            <input type="text" class="screen" placeholder="0" id="screen">
         <table>
            <tr>
                <td>
                    <button style="color:orange" onclick="clr()">AC</button>
                </td>
                <td>
                    <button style="color:deepskyblue" onclick="dis('%')">%</button>
                </td>
                <td>
                    <button style="color:deepskyblue" onclick="dis('/')">/</button>
                </td>
                <td>
                    <button style="color:cornflowerblue" onclick="backspace()">C</button>
                    <i class="fas fa-backspace"></i>
                </td>
            </tr>
            <tr>
                <td>
                    <button onclick="dis('7')">7</button>
                </td>
                <td>
                    <button onclick="dis('8')">8</button>
                </td>
                <td>
                    <button onclick="dis('9')">9</button>
                </td>
                <td>
                    <button style="color:deepskyblue" onclick="dis('*')">x</button>
                </td>
            </tr>
            <tr>
                <td>
                    <button onclick="dis('4')">4</button>
                </td>
                <td>
                    <button onclick="dis('5')">5</button>
                </td>
                <td>
                    <button onclick="dis('6')">6</button>
                </td>
                <td>
                    <button style="color:deepskyblue" onclick="dis('-')">-</button>
                </td>
            </tr>
            <tr>
                <td>
                    <button onclick="dis('1')">1</button>
                </td>
                <td>
                    <button onclick="dis('2')">2</button>
                </td>
                <td>
                    <button onclick="dis('3')">3</button>
                </td>
                <td>
                    <button style="color:deepskyblue" onclick="dis('+')">+</button>
                </td>
            </tr>
            <tr>
                <td>
                    <button onclick="dis('.')">.</button>
                </td>
                <td>
                    <button onclick="dis('0')">0</button>
                </td>
                <td>
                    <button class="equalToBtn" style="color:orange" onclick="solve()">=</button>
                </td>
            </tr>
        </table>
    </div>
        
<script>
    function dis(value) {
        document.getElementById("screen").value+=value;
    }
    function solve() {
       let x = document.getElementById("screen").value;
       let y=eval(x);
       document.getElementById("screen").value=y;
    }
    function clr() {
        document.getElementById("screen"). value=""
    }
    function backspace() {
       let screen = document.getElementById("screen").value;
       document.getElementById("screen").value=screen,substring(0,screen.length-1);
    }
</script>
</body>
</html>
