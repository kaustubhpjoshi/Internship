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
