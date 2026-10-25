<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>BoardQuest 10 | Superhero Edition</title>
<style>
*{box-sizing:border-box}
body{margin:0;font-family:Arial,sans-serif;color:white;background:linear-gradient(145deg,#080d25,#20104a,#700b20);min-height:100vh;text-align:center;padding:18px}
.container{max-width:650px;margin:auto}
header{padding:18px 42px;position:relative}
.logo{font-size:48px}
h1{font-size:32px;margin:8px 0;color:#ffcc33}
.subtitle{color:#d5d9ff}
.panel{background:#111a36;border:2px solid #e63946;border-radius:18px;padding:20px;margin:16px 0;box-shadow:0 0 18px #e6394640}
.stats{display:flex;justify-content:space-around;gap:8px;flex-wrap:wrap}
.stat{background:#202c50;padding:12px;border-radius:12px;flex:1;min-width:90px}
.stat b{display:block;color:#ffcc33;font-size:22px;margin-top:6px}
button,input{border:0;border-radius:12px;padding:14px;font-size:16px;font-weight:bold}
button{background:#e63946;color:white;width:100%;margin-top:10px;cursor:pointer}
button:hover{filter:brightness(1.15)}
button:disabled{cursor:default;opacity:.9}
input{width:100%;margin:6px 0;background:#202c50;color:white;border:1px solid #637bb9}
input::placeholder{color:#c7ccef}
.subjects{display:grid;grid-template-columns:1fr 1fr;gap:10px}
.subjects button{background:#25365f;border:1px solid #637bb9;margin:0}
.option{background:#202c50;text-align:left;border:2px solid #405079}
.option.correct{background:#176b48;border-color:#46e69a}
.option.wrong{background:#8a2333;border-color:#ff7b85}
.small{font-size:13px;color:#c7ccef}
.hidden{display:none!important}
#question{font-size:21px;line-height:1.5}
#feedback{font-weight:bold;margin:15px 0;min-height:24px}
.rank-icon{position:absolute;right:0;top:8px;width:39px;height:39px;padding:0;border-radius:50%;border:2px solid #ffcc33;background:#111a36;font-size:20px}
.record{text-align:left;background:#202c50;padding:12px;border-radius:10px;margin:9px 0;overflow-wrap:anywhere}
footer{color:#b7bddb;font-size:12px;padding:20px}
</style>
</head>
<body>
<div class="container">
<header>
 <button class="rank-icon" onclick="showRank()" aria-label="India Rank">🇮🇳</button>
 <div class="logo">🕷️ 🛡️</div>
 <h1>BOARDQUEST 10</h1>
 <div class="subtitle">SUPERHERO ADVENTURE EDITION</div>
 <p class="small">Maharashtra State Board • Class 10</p>
 <p class="small">Sane Guruji Nutan Madhyamik Vidyalaya</p>
</header>

<div class="panel">
 <div class="stats">
  <div class="stat">⭐ Score<b id="score">0</b></div>
  <div class="stat">⚡ Level<b id="level">1</b></div>
  <div class="stat">📝 Question<b id="progress">0/5</b></div>
 </div>
</div>

<div class="panel" id="login">
 <h2>🦸 Player Login</h2>
 <p>Enter your Player ID and name.</p>
 <input id="playerId" placeholder="Create your Player ID">
 <input id="playerName" placeholder="Enter your name">
 <button onclick="login()">START ADVENTURE</button>
 <p class="small">Demo login. Google sign-in requires Firebase setup.</p>
</div>

<div class="panel hidden" id="home">
 <h2>🦸 Choose Your Mission</h2>
 <p>Welcome, <b id="welcome"></b>!</p>
 <p class="small">Player ID: <span id="playerLabel"></span></p>
 <div class="stats">
  <div class="stat">🏆 Total Score<b id="totalScore">0</b></div>
  <div class="stat">🎯 Rounds<b id="totalRounds">0</b></div>
 </div>
 <h3>Select Subject</h3>
 <div class="subjects">
  <button onclick="selectSubject('Science')">🔬 Science</button>
  <button onclick="selectSubject('Maths')">➗ Maths</button>
  <button onclick="selectSubject('English')">📘 English</button>
  <button onclick="selectSubject('History')">🏛️ History</button>
  <button onclick="selectSubject('Geography')">🌍 Geography</button>
  <button onclick="selectSubject('Marathi')">📚 Marathi</button>
 </div>
 <p id="selectedLabel">Selected: Science</p>
 <button onclick="startRound()">START ROUND ⚡</button>
 <p class="small">5 questions per round • 10 points per correct answer</p>
</div>

<div class="panel hidden" id="game">
 <h2 id="mission">🕷️ Your Mission</h2>
 <p id="subjectName"></p>
 <p id="roundLabel" class="small"></p>
 <h3 id="question"></h3>
 <div id="options" class="subjects"></div>
 <div id="feedback"></div>
 <button id="next" class="hidden" onclick="nextQuestion()">Next Question ➜</button>
 <button onclick="goHome()" style="background:#405079">🏠 Main Menu</button>
</div>

<div class="panel hidden" id="result">
 <div style="font-size:48px">🏆</div>
 <h2>MISSION COMPLETE!</h2>
 <p id="resultText"></p>
 <h3>Answer Sheet</h3>
 <div id="answerSheet"></div>
 <button onclick="retryRound()">🔄 Retry Same Round</button>
 <button onclick="nextRound()">⚡ Next Round</button>
 <button onclick="goHome()" style="background:#405079">Choose Another Subject</button>
</div>

<div class="panel hidden" id="rank">
 <h2>🇮🇳 Hero Rank</h2>
 <p class="small">Rank is based on scores saved in this browser. All-India live ranking needs an online database.</p>
 <div id="rankList"></div>
 <button onclick="closeRank()" style="background:#405079">Back</button>
</div>

<footer>Made for Class 10 learners ❤️<br>Spider-Man + Avengers inspired fan theme</footer>
</div>

<script>
const bank={
Science:[
{q:"What is the SI unit of electric current?",o:["Volt","Ampere","Ohm","Watt"],a:1},
{q:"Which gas do green plants absorb during photosynthesis?",o:["Oxygen","Nitrogen","Carbon dioxide","Hydrogen"],a:2},
{q:"What is the pH of a neutral solution at 25°C?",o:["0","5","7","14"],a:2},
{q:"Which lens is used to correct myopia?",o:["Convex","Concave","Cylindrical only","Plane"],a:1},
{q:"What is the SI unit of force?",o:["Joule","Pascal","Newton","Watt"],a:2}
],
Maths:[
{q:"What is the value of 2³?",o:["6","8","9","12"],a:1},
{q:"Degree of 4x² + 3x + 1?",o:["1","2","3","4"],a:1},
{q:"What is sin 30°?",o:["0","1","1/2","√3/2"],a:2},
{q:"Sum of roots of x² - 5x + 6 = 0?",o:["6","-5","5","-6"],a:2},
{q:"Probability of heads on a fair coin?",o:["0","1/4","1/2","1"],a:2}
],
English:[
{q:"Past tense of 'go'?",o:["Goed","Gone","Went","Going"],a:2},
{q:"Synonym of 'happy'?",o:["Joyful","Angry","Tired","Sad"],a:0},
{q:"Which is a noun?",o:["Quickly","Beautiful","Honesty","Run"],a:2},
{q:"Choose the correct article: ___ apple.",o:["A","An","The only","No article"],a:1},
{q:"Plural of 'child'?",o:["Childs","Childes","Children","Childrens"],a:2}
],
History:[
{q:"Who founded the Maratha kingdom?",o:["Shivaji Maharaj","Akbar","Ashoka","Tipu Sultan"],a:0},
{q:"India became independent in:",o:["1942","1945","1947","1950"],a:2},
{q:"Who chaired the Constitution Drafting Committee?",o:["Mahatma Gandhi","Dr. B. R. Ambedkar","Jawaharlal Nehru","Sardar Patel"],a:1},
{q:"Quit India Movement began in:",o:["1920","1930","1942","1947"],a:2},
{q:"First Prime Minister of independent India?",o:["Dr. Rajendra Prasad","Sardar Patel","Jawaharlal Nehru","Lal Bahadur Shastri"],a:2}
],
Geography:[
{q:"Largest ocean on Earth?",o:["Atlantic","Indian","Arctic","Pacific"],a:3},
{q:"Line dividing Earth's Northern and Southern Hemispheres?",o:["Tropic of Cancer","Equator","Prime Meridian","Tropic of Capricorn"],a:1},
{q:"Which instrument records earthquakes?",o:["Barometer","Thermometer","Seismograph","Anemometer"],a:2},
{q:"Capital of Maharashtra?",o:["Pune","Nagpur","Mumbai","Nashik"],a:2},
{q:"Which is a renewable energy source?",o:["Coal","Petroleum","Solar energy","Natural gas"],a:2}
],
Marathi:[
{q:"'आई' हा शब्द कोणत्या प्रकारचा आहे?",o:["नाम","क्रियापद","विशेषण","अव्यय"],a:0},
{q:"'मोठा' या शब्दाचा विरुद्धार्थी शब्द?",o:["लहान","उंच","जाड","सुंदर"],a:0},
{q:"'आकाश' या शब्दाचा समानार्थी शब्द?",o:["नभ","जल","वारा","भूमी"],a:0},
{q:"'तो शाळेत जातो.' या वाक्यातील क्रियापद?",o:["तो","शाळेत","जातो","वाक्य"],a:2},
{q:"मराठी भाषेची लिपी कोणती?",o:["रोमन","देवनागरी","गुरुमुखी","तमिळ"],a:1}
]
};

let player=null,currentSubject="Science",round=1,questions=[],index=0,score=0,answered=false,roundAnswers=[];

const $=id=>document.getElementById(id);
const sections=["login","home","game","result","rank"];
function showOnly(id){sections.forEach(s=>$(s).classList.toggle("hidden",s!==id))}
function getRecords(){try{return JSON.parse(localStorage.getItem("bq10_records")||"[]")}catch(e){return []}}
function saveRecords(r){localStorage.setItem("bq10_records",JSON.stringify(r))}
function escapeHTML(s){return String(s).replace(/[&<>"']/g,c=>({"&":"&amp;","<":"&lt;",">":"&gt;",'"':"&quot;","'":"&#39;"}[c]))}

function login(){
 const id=$("playerId").value.trim(),name=$("playerName").value.trim();
 if(!id||!name){alert("Enter both Player ID and name.");return}
 player={id,name};
 let r=getRecords(),p=r.find(x=>x.id===id);
 if(!p)r.push({id,name,score:0,rounds:0});
 else p.name=name;
 saveRecords(r);
 $("welcome").textContent=name;
 $("playerLabel").textContent=id;
 updateStats();
 showOnly("home");
}
function selectSubject(s){
 currentSubject=s;
 $("selectedLabel").textContent="Selected: "+s;
}
function updateStats(){
 const p=getRecords().find(x=>x.id===player.id);
 $("totalScore").textContent=p?p.score:0;
 $("totalRounds").textContent=p?p.rounds:0;
 $("score").textContent=p?p.score:0;
}
function startRound(){
 const source=bank[currentSubject];
 const start=((round-1)*5)%source.length;
 questions=Array.from({length:5},(_,i)=>source[(start+i)%source.length]);
 index=0;score=0;roundAnswers=[];
 $("mission").textContent="🕷️ "+currentSubject+" Challenge";
 $("subjectName").textContent="Mission: "+currentSubject;
 $("roundLabel").textContent="Round "+round;
 showOnly("game");showQuestion();
}
function showQuestion(){
 answered=false;
 const item=questions[index];
 $("score").textContent=score;
 $("level").textContent=round;
 $("progress").textContent=(index+1)+"/"+questions.length;
 $("question").textContent=item.q;
 $("feedback").textContent="";
 $("next").classList.add("hidden");
 $("options").innerHTML="";
 item.o.forEach((option,i)=>{
  const btn=document.createElement("button");
  btn.className="option";
  btn.textContent=String.fromCharCode(65+i)+". "+option;
  btn.onclick=()=>chooseAnswer(i,btn);
  $("options").appendChild(btn);
 });
}
function chooseAnswer(choice,btn){
 if(answered)return;
 answered=true;
 const item=questions[index],buttons=[...$("options").children];
 buttons.forEach((b,i)=>{
  b.disabled=true;
  if(i===item.a)b.classList.add("correct");
 });
 if(choice===item.a){
  score+=10;
  $("feedback").textContent="✅ Correct! +10 points, Hero!";
 }else{
  btn.classList.add("wrong");
  $("feedback").textContent="❌ Not quite! Green shows the correct answer.";
 }
 roundAnswers.push({q:item.q,o:item.o,choice,correct:item.a});
 $("score").textContent=score;
 $("next").textContent=index===questions.length-1?"🏆 See Results":"Next Question ➜";
 $("next").classList.remove("hidden");
}
function nextQuestion(){
 if(!answered)return;
 if(index<questions.length-1){index++;showQuestion()}
 else finishRound();
}
function finishRound(){
 let r=getRecords(),p=r.find(x=>x.id===player.id);
 if(!p){p={id:player.id,name:player.name,score:0,rounds:0};r.push(p)}
 p.score+=score;p.rounds++;
 saveRecords(r);updateStats();
 $("resultText").textContent="You scored "+score+" out of 50 in "+currentSubject+" Round "+round+"!";
 $("answerSheet").innerHTML="";
 roundAnswers.forEach((a,i)=>{
  const d=document.createElement("div");d.className="record";
  d.innerHTML="<b>Q"+(i+1)+". "+escapeHTML(a.q)+"</b>"+
  "<p>Your answer: "+escapeHTML(a.o[a.choice])+"</p>"+
  "<p>Correct answer: "+escapeHTML(a.o[a.correct])+"</p>"+
  "<p>"+(a.choice===a.correct?"✅ Correct":"❌ Incorrect")+"</p>";
  $("answerSheet").appendChild(d);
 });
 showOnly("result");
}
function retryRound(){startRound()}
function nextRound(){round++;startRound()}
function goHome(){updateStats();showOnly("home")}
function showRank(){
 const r=getRecords().sort((a,b)=>b.score-a.score);
 $("rankList").innerHTML="";
 if(!r.length)$("rankList").innerHTML="<p>No scores recorded yet. Play a round first!</p>";
 r.forEach((p,i)=>{
  const d=document.createElement("div");d.className="record";
  d.innerHTML="<b>#"+(i+1)+" "+(i===0?"🕷️ Spider-Man":i===1?"🛡️ Avengers Hero":"🦸 Superhero")+"</b>"+
  "<p>"+escapeHTML(p.name)+" • "+escapeHTML(p.id)+"</p>"+
  "<p>⭐ Score: "+p.score+" | Rounds: "+p.rounds+"</p>";
  $("rankList").appendChild(d);
 });
 showOnly("rank");
}
function closeRank(){showOnly(player?"home":"login")}
</script>
</body>
</html>
