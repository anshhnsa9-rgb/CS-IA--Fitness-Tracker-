<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Fitness Challenge App</title>
<link href="https://fonts.googleapis.com/css?family=Inter:400,600&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css">
<style>
body{font-family:'Inter',Arial,sans-serif;background:#f7f9fb;margin:0;}
.container{background:#fff;padding:32px 24px;border-radius:16px;max-width:480px;margin:48px auto 80px auto;box-shadow:0 4px 24px rgba(0,0,0,0.07);}
h1{color:#1a3e8a;font-size:2rem;font-weight:600;text-align:center;margin-bottom:8px;}
h2{color:#1a3e8a;font-size:1.2rem;font-weight:600;margin-bottom:8px;}
.section{margin-bottom:32px;}
input,button{margin:6px 0;padding:12px;width:100%;border-radius:8px;border:1px solid #e3e7ee;font-size:1rem;box-sizing:border-box;}
button{background:#2563eb;color:#fff;border:none;font-weight:600;cursor:pointer;transition:background 0.2s;}
button:hover{background:#1e40af;}
.leaderboard,.history{margin-top:10px;padding-left:0;}
.leaderboard li,.history li{margin-bottom:8px;list-style:none;background:#f1f5fa;padding:8px 12px;border-radius:6px;}
.icon{color:#2563eb;font-size:2.5rem;display:block;margin:0 auto 12px auto;}
.empty-state{text-align:center;color:#94a3b8;margin:40px 0;}
.empty-state .icon{font-size:3rem;margin-bottom:12px;}
.bottom-nav{position:fixed;bottom:0;left:0;right:0;background:#fff;border-top:1px solid #e3e7ee;display:flex;justify-content:space-around;align-items:center;height:64px;z-index:10;}
.nav-item{text-align:center;color:#2563eb;font-size:1.1rem;flex:1;cursor:pointer;transition:color 0.2s;}
.nav-item.inactive{color:#94a3b8;}
.nav-item i{display:block;font-size:1.5rem;margin-bottom:2px;}
.section{display:none;}
.section.active{display:block;}
#loginContainer,#signUpContainer{display:none;}
.error-msg{color:red;text-align:center;margin-top:8px;}
.link{color:#2563eb;cursor:pointer;text-decoration:underline;}
#signOutBtn{background:#ef4444;margin-top:16px;}
#signOutBtn:hover{background:#dc2626;}
</style>
</head>
<body>
<div id="loginContainer">
<div class="container" style="margin-top:100px;">
<i class="fa-solid fa-trophy icon"></i>
<h1>Fitness Challenge</h1>
<div style="text-align:center;color:#64748b;margin-bottom:24px;">Track your progress, compete with friends</div>
<input type="text" id="loginEmail" placeholder="Email">
<input type="password" id="loginPassword" placeholder="Password">
<button onclick="login()">Sign In</button>
<div style="text-align:center;margin-top:12px;">
<span>Don't have an account? <span class="link" onclick="showSignUp()">Sign Up</span></span>
</div>
<div id="loginError" class="error-msg"></div>
</div>
</div>
<div id="signUpContainer">
<div class="container" style="margin-top:100px;">
<i class="fa-solid fa-trophy icon"></i>
<h1>Sign Up</h1>
<input type="text" id="signUpEmail" placeholder="Email">
<input type="password" id="signUpPassword" placeholder="Password">
<button onclick="signUp()">Create Account</button>
<div style="text-align:center;margin-top:12px;">
<span>Already have an account? <span class="link" onclick="showLogin()">Sign In</span></span>
</div>
<div id="signUpError" class="error-msg"></div>
</div>
</div>
<div id="mainApp" style="display:none;">
<div class="container">
<div id="challengesSection" class="section active">
<i class="fa-solid fa-trophy icon"></i>
<h1>Challenges</h1>
<div style="text-align:center;color:#64748b;margin-bottom:24px;">Join and compete with friends</div>
<div id="challengeList"></div>
<div class="empty-state" id="noChallenges">
<i class="fa-solid fa-trophy icon"></i>
<div>No challenges yet</div>
<div style="font-size:0.95rem;">Create one to get started!</div>
</div>
<h2>Create Challenge</h2>
<input type="text" id="challengeName" placeholder="Challenge name">
<input type="text" id="challengeGoal" placeholder="Challenge goal (e.g. 10000 steps)">
<button onclick="createChallenge()">Create Challenge</button>
<div id="createChallengeResult"></div>
<h2>Join Challenge</h2>
<input type="number" id="joinChallengeId" placeholder="Challenge ID">
<button onclick="joinChallenge()">Join Challenge</button>
<div id="joinChallengeResult"></div>
</div>
<div id="leaderboardSection" class="section">
<i class="fa-solid fa-chart-line icon"></i>
<h1>Leaderboard</h1>
<input type="number" id="leaderboardChallengeId" placeholder="Challenge ID">
<button onclick="getLeaderboard()">Show Leaderboard</button>
<ul id="leaderboardList" class="leaderboard"></ul>
</div>
<div id="profileSection" class="section">
<i class="fa-solid fa-user-circle icon"></i>
<h1>Profile</h1>
<div style="text-align:center;color:#64748b;margin-bottom:24px;">Your fitness journey</div>
<div style="display:flex;justify-content:space-between;margin-bottom:24px;">
<div style="text-align:center;flex:1;">
<i class="fa-solid fa-trophy" style="color:#2563eb;"></i>
<div id="profileChallenges" style="font-size:1.3rem;font-weight:600;">0</div>
<div style="font-size:0.95rem;">Challenges Joined</div>
</div>
<div style="text-align:center;flex:1;">
<i class="fa-solid fa-heart-pulse" style="color:#22c55e;"></i>
<div id="profileActive" style="font-size:1.3rem;font-weight:600;">0</div>
<div style="font-size:0.95rem;">Active</div>
</div>
<div style="text-align:center;flex:1;">
<i class="fa-solid fa-calendar-days" style="color:#a855f7;"></i>
<div id="profileHistory" style="font-size:1.3rem;font-weight:600;">0</div>
<div style="font-size:0.95rem;">Logs</div>
</div>
</div>
<button onclick="getHistory()">Show My History</button>
<ul id="historyList" class="history"></ul>
<button id="signOutBtn">Sign Out</button>
</div>
</div>
<div class="bottom-nav">
<div class="nav-item active" onclick="showSection('challengesSection',this)">
<i class="fa-solid fa-trophy"></i>
Challenges
</div>
<div class="nav-item inactive" onclick="showSection('leaderboardSection',this)">
<i class="fa-solid fa-chart-line"></i>
Leaderboard
</div>
<div class="nav-item inactive" onclick="showSection('profileSection',this)">
<i class="fa-solid fa-user-circle"></i>
Profile
</div>
</div>
</div>
<script>
let users=JSON.parse(localStorage.getItem('users')||'[]');
let userId=localStorage.getItem('userId');
let challenges=JSON.parse(localStorage.getItem('challenges')||'[]');
let logs=JSON.parse(localStorage.getItem('logs')||'[]');
let joinedChallenges=JSON.parse(localStorage.getItem('joinedChallenges')||'[]');
function saveData(){
localStorage.setItem('users',JSON.stringify(users));
localStorage.setItem('challenges',JSON.stringify(challenges));
localStorage.setItem('logs',JSON.stringify(logs));
localStorage.setItem('joinedChallenges',JSON.stringify(joinedChallenges));
}
function showSection(sectionId,navItem){
document.querySelectorAll('.section').forEach(sec=>sec.classList.remove('active'));
document.getElementById(sectionId).classList.add('active');
document.querySelectorAll('.nav-item').forEach(item=>item.classList.remove('active'));
document.querySelectorAll('.nav-item').forEach(item=>item.classList.add('inactive'));
navItem.classList.add('active');
navItem.classList.remove('inactive');
}
function showLogin(){
document.getElementById('loginContainer').style.display='block';
document.getElementById('signUpContainer').style.display='none';
document.getElementById('mainApp').style.display='none';
}
function showSignUp(){
document.getElementById('loginContainer').style.display='none';
document.getElementById('signUpContainer').style.display='block';
document.getElementById('mainApp').style.display='none';
}
function showApp(){
document.getElementById('loginContainer').style.display='none';
document.getElementById('signUpContainer').style.display='none';
document.getElementById('mainApp').style.display='block';
}
function login(){
const email=document.getElementById('loginEmail').value.trim();
const password=document.getElementById('loginPassword').value;
const user=users.find(u=>u.email===email&&u.password===password);
if(user){
userId=user.id;
localStorage.setItem('userId',userId);
joinedChallenges=user.joinedChallenges||[];
localStorage.setItem('joinedChallenges',JSON.stringify(joinedChallenges));
document.getElementById('loginError').innerText='';
showApp();
showChallenges();
updateProfile();
}else{
document.getElementById('loginError').innerText='Invalid email or password!';
}
}
function signUp(){
const email=document.getElementById('signUpEmail').value.trim();
const password=document.getElementById('signUpPassword').value;
if(!email||!password){
document.getElementById('signUpError').innerText='Please enter email and password!';
return;
}
if(users.find(u=>u.email===email)){
document.getElementById('signUpError').innerText='Email already registered!';
return;
}
userId=Date.now().toString();
users.push({id:userId,email,password,joinedChallenges:[]});
localStorage.setItem('userId',userId);
joinedChallenges=[];
saveData();
document.getElementById('signUpError').innerText='';
showApp();
showChallenges();
updateProfile();
}
function signOut(){
localStorage.removeItem('userId');
localStorage.removeItem('joinedChallenges');
userId=null;
joinedChallenges=[];
showLogin();
}
document.getElementById('signOutBtn').onclick=signOut;
function createChallenge(){
const name=document.getElementById('challengeName').value.trim();
const goal=document.getElementById('challengeGoal').value.trim();
if(!name||!goal){
document.getElementById('createChallengeResult').innerText='Please enter name and goal!';
return;
}
const challengeId=challenges.length?challenges[challenges.length-1].id+1:1;
challenges.push({id:challengeId,name,goal,creatorId:userId,members:[userId]});
joinedChallenges.push(challengeId);
const user=users.find(u=>u.id===userId);
if(user)user.joinedChallenges=joinedChallenges;
document.getElementById('createChallengeResult').innerText=`Challenge created (ID: ${challengeId})`;
saveData();
showChallenges();
updateProfile();
}
function joinChallenge(){
const challengeId=Number(document.getElementById('joinChallengeId').value);
const challenge=challenges.find(c=>c.id===challengeId);
if(!challenge){
document.getElementById('joinChallengeResult').innerText='Challenge not found!';
return;
}
if(!challenge.members.includes(userId)){
challenge.members.push(userId);
if(!joinedChallenges.includes(challengeId)){
joinedChallenges.push(challengeId);
}
const user=users.find(u=>u.id===userId);
if(user)user.joinedChallenges=joinedChallenges;
document.getElementById('joinChallengeResult').innerText='Joined challenge!';
saveData();
showChallenges();
updateProfile();
}else{
document.getElementById('joinChallengeResult').innerText='Already joined!';
}
}
function getLeaderboard(){
const challengeId=Number(document.getElementById('leaderboardChallengeId').value);
const challenge=challenges.find(c=>c.id===challengeId);
const list=document.getElementById('leaderboardList');
list.innerHTML='';
if(!challenge){
list.innerHTML='<li>Challenge not found.</li>';
return;
}
const challengeLogs=logs.filter(l=>l.challengeId===challengeId);
const leaderboard={};
challengeLogs.forEach(log=>{
leaderboard[log.userId]=(leaderboard[log.userId]||0)+log.progress;
});
const sorted=Object.entries(leaderboard)
.map(([userId,total])=>{
const user=users.find(u=>u.id===userId);
return{userId,username:user?(user.email||user.username):'User',total};
})
.sort((a,b)=>b.total-a.total);
if(sorted.length===0){
list.innerHTML='<li>No progress yet.</li>';
}
sorted.forEach((entry,idx)=>{
const li=document.createElement('li');
li.innerHTML=`<strong>#${idx+1}</strong> ${entry.username}: <span style="color:#2563eb;">${entry.total}</span>`;
list.appendChild(li);
});
}
function getHistory(){
const list=document.getElementById('historyList');
const userLogs=logs.filter(l=>l.userId===userId);
list.innerHTML='';
if(userLogs.length===0){
list.innerHTML='<li>No logs yet.</li>';
}
userLogs.forEach(log=>{
const challenge=challenges.find(c=>c.id===log.challengeId);
const challengeName=challenge?challenge.name:`Challenge ${log.challengeId}`;
const li=document.createElement('li');
li.innerText=`${challengeName}: ${log.progress} on ${new Date(log.date).toLocaleDateString()}`;
list.appendChild(li);
});
updateProfile();
}
function showChallenges(){
const list=document.getElementById('challengeList');
if(joinedChallenges.length===0){
document.getElementById('noChallenges').style.display='block';
list.innerHTML='';
}else{
document.getElementById('noChallenges').style.display='none';
list.innerHTML='';
joinedChallenges.forEach(id=>{
const challenge=challenges.find(c=>c.id===id);
if(challenge){
const div=document.createElement('div');
div.style="background:#f1f5fa;padding:12px;border-radius:8px;margin-bottom:8px;";
div.innerHTML=`<strong>${challenge.name}</strong> <br><span style="color:#64748b;">Goal: ${challenge.goal}</span> <br>ID: ${challenge.id}`;
list.appendChild(div);
}
});
}
}
function updateProfile(){
document.getElementById('profileChallenges').innerText=joinedChallenges.length;
document.getElementById('profileActive').innerText=joinedChallenges.length;
document.getElementById('profileHistory').innerText=logs.filter(l=>l.userId===userId).length;
}
function logProgress(){
if(joinedChallenges.length===0){
alert('Join a challenge first!');
return;
}
const challengeId=Number(prompt("Enter Challenge ID to log progress:"));
if(!joinedChallenges.includes(challengeId)){
alert('You have not joined this challenge!');
return;
}
const progress=Number(prompt("Enter your progress (e.g. steps):"));
if(isNaN(progress)||progress<=0){
alert('Please enter a valid number!');
return;
}
logs.push({userId,challengeId,progress,date:new Date().toISOString()});
saveData();
alert('Progress logged!');
getHistory();
}
const logBtn=document.createElement('button');
logBtn.innerText="Log Progress";
logBtn.onclick=logProgress;
setTimeout(()=>{
document.getElementById('profileSection').insertBefore(logBtn,document.getElementById('historyList'));
},0);
if(!userId){
showLogin();
}else{
showApp();
showChallenges();
updateProfile();
}
</script>
</body>
</html>
