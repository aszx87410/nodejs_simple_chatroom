<!doctype html>
<html>
  <head>
    <title>Socket.IO chat</title>
    <style>
      * { margin: 0; padding: 0; box-sizing: border-box; }
      body { font: 13px Helvetica, Arial; }

      #m{ 
        border: 2px solid black; 
        padding: 10px; 
        width: 90%; 
        margin: .5%; 
        position: fixed; 
        bottom: 0;

      }
      #send{ 
        width: 8%; 
        margin: .5%; 
        background: rgb(121,2,2);
        color:white; 
        
        padding: 10px; 
        position: fixed; 
        bottom: 0;
        right:5px;
      }
      #message_block{
        width:100%;
        position: absolute;
        top:0;
        bottom:5%;
        margin-bottom:10px;
        border: solid 2px black; 
        overflow:auto;
      }
      #messages { 
        list-style-type: none; 
        margin: 10px; 
        
        padding: 0; 
      }
      #messages li { 
        padding: 5px 10px; 
        font-size:16pt;
      }
      #messages li:nth-child(odd) { 
        background: #eee; 
      }
    </style>

    <script src="https://cdn.socket.io/socket.io-1.2.0.js"></script>
    <script src="http://code.jquery.com/jquery-1.11.1.js"></script>
    <script>



      var socket = io();
      $(document).ready(function(){

        var name = prompt("請輸入暱稱","guest");

        if(name=="" || name==null){
          name = "guest";
        }

        //tell server
        socket.emit("add user",name);

        //監聽新訊息事件
        socket.on('chat message', function(data){
          appendMessage(data.username+":"+data.msg);
        });

        socket.on('add user',function(data){
          appendMessage(data.username+"已加入");
        });

        socket.on('user left',function(data){
          appendMessage(data.username+"已離開");
        });

        $('#send').click(function(){
          var text = $('#m').val();
          socket.emit('chat message', text);
          $('#m').val('');
          return false;
        });

        $("#m").keydown(function(event){
          if ( event.which == 13 ){
            $('#send').click();
          }
        });

        function appendMessage(msg){
          $('#messages').append($('<li>').text(msg));
          var message = document.getElementById("message_block");
          message.scrollTop = message.scrollHeight;

        }
      });
      
    </script>
  </head>
  <body>
  <div id="message_block">
    <ul id="messages"></ul>
  <div>
    <input id="m" autocomplete="off" /><button id="send">Send</button>
  </body>
</html>