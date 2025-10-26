<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Welcome to Raza Game - Tic Tac Toe</title>
  <style>
    :root{
      --bg1:#1a2a6c;
      --bg2:#b21f1f;
      --bg3:#fdbb2d;
      --accent:#06b6d4;
      --win:#10b981;
      --draw:#facc15;
      --text:#e6eef8;
      font-family: Poppins, sans-serif;
    }
    body{
      margin:0;
      height:100vh;
      display:flex;
      align-items:center;
      justify-content:center;
      background:linear-gradient(135deg,var(--bg1),var(--bg2),var(--bg3));
      background-size:400% 400%;
      animation:gradientShift 10s ease infinite;
      color:var(--text);
    }
    @keyframes gradientShift{
      0%{background-position:0% 50%;}
      50%{background-position:100% 50%;}
      100%{background-position:0% 50%;}
    }
    .container{
      width:90%;
      max-width:400px;
      background:rgba(0,0,0,0.4);
      border-radius:16px;
      padding:20px;
      text-align:center;
      box-shadow:0 8px 30px rgba(0,0,0,0.4);
      position: relative;
    }

    h1{margin:10px 0;font-size:24px;color:#fff;}
    #board{
      display:grid;
      grid-template-columns:repeat(3,1fr);
      gap:10px;
      margin:20px 0;
    }
    .cell{
      width:100%;
      aspect-ratio:1;
      font-size:40px;
      font-weight:bold;
      color:#fff;
      background:rgba(255,255,255,0.1);
      border:none;
      border-radius:10px;
      cursor:pointer;
      transition:transform .2s,background .3s;
    }
    .cell:hover{transform:scale(1.05);background:rgba(255,255,255,0.2);}

    #messageScreen{
      position:fixed;
      inset:0;
      background:rgba(0,0,0,0.8);
      display:flex;
      flex-direction:column;
      align-items:center;
      justify-content:center;
      color:#fff;
      font-size:28px;
      z-index:10;
      visibility:hidden;
      opacity:0;
      transition:opacity .5s,visibility .5s;
    }
    #messageScreen.show{visibility:visible;opacity:1;}

    #newGameBtn, #exitGameBtn, #persistentExitBtn{
      margin-top:20px;
      padding:10px 20px;
      font-size:18px;
      border:none;
      border-radius:8px;
      background:linear-gradient(90deg,#06b6d4,#3b82f6);
      color:#fff;
      cursor:pointer;
    }
    #exitGameBtn, #persistentExitBtn{background:linear-gradient(90deg,#ef4444,#f43f5e);}

    #persistentExitBtn{
      position:fixed;
      top:20px;
      right:20px;
      z-index:5;
      padding:8px 16px;
      font-size:16px;
    }
  </style>
</head>
<body>
  <button id="persistentExitBtn">Exit Game</button>
  <div class="container" id="gameContainer">
    <h1 id="welcomeText">Welcome to Raza Game</h1>
    <div id="board"></div>
    <h2 id="status">Player QR's turn</h2>
  </div>

  <div id="messageScreen">
    <div id="resultMessage"></div>
    <button id="newGameBtn">New Game</button>
    <button id="exitGameBtn">Exit Game</button>
  </div>

  <script>
    const boardEl=document.getElementById('board');
    const statusEl=document.getElementById('status');
    const messageScreen=document.getElementById('messageScreen');
    const resultMessage=document.getElementById('resultMessage');
    const newGameBtn=document.getElementById('newGameBtn');
    const exitGameBtn=document.getElementById('exitGameBtn');
    const persistentExitBtn=document.getElementById('persistentExitBtn');

    let board=['','','','','','','','',''];
    let currentPlayer='QR';
    let running=true;

    const winPatterns=[
      [0,1,2],[3,4,5],[6,7,8],
      [0,3,6],[1,4,7],[2,5,8],
      [0,4,8],[2,4,6]
    ];

    function startGame(){
      boardEl.innerHTML='';
      for(let i=0;i<9;i++){
        const cell=document.createElement('button');
        cell.className='cell';
        cell.dataset.index=i;
        cell.addEventListener('click',cellClick);
        boardEl.appendChild(cell);
      }
      statusEl.textContent=`Player ${currentPlayer}'s turn`;
      running=true;
    }

    function cellClick(e){
      const i=e.target.dataset.index;
      if(!running||board[i]!=='')return;
      board[i]=currentPlayer;
      e.target.textContent=currentPlayer;
      checkWinner();
      currentPlayer=currentPlayer==='QR'?'AR':'QR';
      if(running)statusEl.textContent=`Player ${currentPlayer}'s turn`;
    }

    function checkWinner(){
      for(const [a,b,c] of winPatterns){
        if(board[a]&&board[a]===board[b]&&board[a]===board[c]){
          const winner=board[a];
          const loser=winner==='QR'?'AR':'QR';
          showResult(`${winner} Wins! ${loser} Lost!`,true);
          return;
        }
      }
      if(!board.includes('')){
        showResult(`It's a Draw!`,false,true);
      }
    }

    function showResult(message,isWin=false,isDraw=false){
      running=false;
      resultMessage.textContent=message;
      if(isWin){resultMessage.style.color='var(--win)';}
      else if(isDraw){resultMessage.style.color='var(--draw)';}
      messageScreen.classList.add('show');
    }

    function exitGame(){
      messageScreen.classList.remove('show');
      document.getElementById('gameContainer').innerHTML='<h1>Thanks for playing Raza Game!</h1>';
      persistentExitBtn.style.display='none';
    }

    newGameBtn.addEventListener('click',()=>{
      messageScreen.classList.remove('show');
      board=['','','','','','','','',''];
      currentPlayer='QR';
      startGame();
    });

    exitGameBtn.addEventListener('click',exitGame);
    persistentExitBtn.addEventListener('click',exitGame);

    startGame();
  </script>
</body>
</html>