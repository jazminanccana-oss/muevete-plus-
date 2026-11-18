[index (1).html](https://github.com/user-attachments/files/35009012/index.1.html)
<!doctype html>
<html lang="es">
<head>
<meta charset="utf-8"><meta name="viewport" content="width=device-width,initial-scale=1">
<title>Muévete+ | Bienestar digital</title>
<style>
:root{--pink:#f4b8d0;--pale:#fff0f6;--paler:#fffafd;--rose:#a94370;--ink:#493744;--muted:#806d79;--line:#f0d4e0;--green:#e4f4e9;--yellow:#fff4d9}
*{box-sizing:border-box}body{margin:0;background:linear-gradient(145deg,#fff1f7,#fffafd);font-family:system-ui,Arial,sans-serif;color:var(--ink)}
header{padding:26px 16px 20px;text-align:center;background:var(--pale);border-bottom:1px solid var(--line)}
header h1{margin:0;color:var(--rose);font-size:2rem}header p{margin:7px 0 0}
main{max-width:1000px;margin:20px auto;padding:0 14px 30px}
.top{display:flex;gap:10px;justify-content:center;flex-wrap:wrap;margin-bottom:12px}
.pill{background:#fff;border:1px solid var(--line);border-radius:999px;padding:10px 15px;color:var(--rose);font-weight:700}
nav{display:flex;gap:8px;flex-wrap:wrap;justify-content:center;margin:16px 0}
button,.btn{border:0;border-radius:22px;padding:10px 15px;background:#ffe1ed;color:var(--rose);font-weight:700;cursor:pointer}
button.active,.primary{background:var(--rose);color:#fff}
.panel{background:#fff;border:1px solid var(--line);border-radius:20px;padding:20px;box-shadow:0 5px 18px #9e567012}
section.hidden{display:none}h2{margin:0 0 12px;color:var(--rose)}h3{color:var(--rose);margin:8px 0}
.grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(210px,1fr));gap:12px}
.tile{background:var(--paler);border:1px solid #f6e2eb;border-radius:15px;padding:14px}
label{display:block;font-weight:650;margin:10px 0 5px}
input,select,textarea{width:100%;padding:10px;border:1px solid #e7c5d4;border-radius:10px;background:#fffafd;color:var(--ink);font:inherit}
input[type=checkbox]{width:auto}
.row{display:flex;gap:8px;align-items:center;flex-wrap:wrap}.row>*{flex:1}
.actions{display:flex;gap:8px;flex-wrap:wrap;margin-top:12px}
.small{font-size:.88rem;color:var(--muted)}.big{font-size:1.8rem;font-weight:800;color:var(--rose)}
ul{padding-left:20px}li{margin:7px 0}.taskline{display:flex;align-items:center;gap:9px}.taskline input{width:auto}
table{width:100%;border-collapse:collapse;margin-top:12px}th,td{border-bottom:1px solid var(--line);padding:8px;text-align:left;font-size:.9rem}th{color:var(--rose)}
.bar{height:10px;background:#f8e3ec;border-radius:20px;overflow:hidden}.bar span{display:block;height:100%;background:#d875a0;width:0}
a{color:var(--rose);font-weight:650}footer{text-align:center;color:#987d8d;padding:20px;font-size:.85rem}
@media(max-width:550px){header h1{font-size:1.7rem}.panel{padding:15px}nav button{font-size:.84rem;padding:9px 11px}}
</style></head>
<body>
<header><h1>🌸 Muévete+</h1><p>Organiza tu tiempo, cuida tu bienestar y ¡suma logros!</p></header>
<main>
<div class="top"><div class="pill">⭐ Puntos: <span id="points">0</span></div><div class="pill">🏅 Racha de hábitos: <span id="streak">0</span> días registrados</div></div>
<nav>
<button class="active" data-tab="home">Inicio</button><button data-tab="schedule">📚 Horarios</button><button data-tab="tasks">📝 Tareas</button><button data-tab="screen">📱 Pantallas</button><button data-tab="breaks">🧘 Pausas</button><button data-tab="activity">🏃 Actividad</button><button data-tab="music">🎧 Música</button><button data-tab="stats">📊 Estadísticas</button><button data-tab="challenge">🏆 Desafío</button>
</nav>
<section id="home" class="panel">
<h2>¡Hola! Este es tu espacio saludable 💗</h2>
<p>Planifica tu semana, organiza tus tareas, registra el uso de pantallas y encuentra momentos para moverte.</p>
<div class="grid">
<div class="tile"><h3>🌙 Planifica por la noche</h3><p>Antes de terminar el día, revisa tus clases de mañana, agrega tareas y elige cuándo harás una pausa o actividad física.</p></div>
<div class="tile"><h3>📵 Bienestar digital</h3><p>Registra tu tiempo de pantalla y consulta las herramientas de bienestar digital de tu celular para revisar el uso real.</p></div>
<div class="tile"><h3>🌳 Tiempo de concentración</h3><p>Usa un bloque de estudio sin distracciones. Puedes probar una dinámica tipo árbol virtual para mantener el enfoque.</p></div>
<div class="tile"><h3>💚 Muévete a tu ritmo</h3><p>Registra caminatas, deportes, baile o cualquier actividad que disfrutes. Cada pequeño avance cuenta.</p></div>
</div>
<p class="small">Tus datos se guardan en este navegador y dispositivo. Esta versión no se sincroniza entre celulares.</p>
</section>

<section id="schedule" class="panel hidden">
<h2>📚 Mi horario escolar y planificación</h2>
<p>Este horario parte de la jornada de referencia de Fe y Alegría 05 Calasanz. Puedes editarlo para adaptarlo a tus clases. ¡También puedes organizar tu tarde y noche!</p>
<div class="row"><div><label for="weekday">Día</label><select id="weekday"><option>Lunes</option><option>Martes</option><option>Miércoles</option><option>Jueves</option><option>Viernes</option><option>Sábado</option><option>Domingo</option></select></div><div><label for="schoolstart">Entrada</label><input id="schoolstart" type="time" value="07:40"></div><div><label for="schoolend">Salida</label><input id="schoolend" type="time" value="13:35"></div></div>
<label for="classnotes">Clases, cursos o indicaciones</label><textarea id="classnotes" rows="2" placeholder="Ej. Matemática, Comunicación, Educación Física..."></textarea>
<h3>Mi planificación después de clases</h3>
<div class="row"><div><label for="planstart">Hora</label><input id="planstart" type="time" value="16:00"></div><div><label for="planitem">Actividad</label><input id="planitem" placeholder="Ej. hacer tarea, deporte, descanso"></div></div>
<div class="actions"><button class="primary" id="saveplan">Guardar horario y actividad</button></div>
<div id="schedulelist"></div>
<p class="small">Sugerencia: cada noche puedes cambiar el día y preparar el horario del día siguiente.</p>
</section>

<section id="tasks" class="panel hidden">
<h2>📝 Organizador de tareas</h2><div class="row"><div><label for="tasktext">Tarea o actividad escolar</label><input id="tasktext" placeholder="Ej. terminar informe de Ciencia"></div><div><label for="taskdate">Fecha</label><input id="taskdate" type="date"></div></div>
<div class="actions"><button class="primary" id="addtask">Agregar tarea</button></div><ul id="tasklist"></ul>
<div class="tile"><b>🌳 Modo concentración</b><p>Elige una tarea, deja el celular a un lado y trabaja durante un bloque de enfoque. Al terminar, marca tu tarea como completada.</p><label for="focusmins">Duración del enfoque (minutos)</label><input id="focusmins" type="number" min="5" max="90" value="25"><div class="actions"><button id="focusstart">Iniciar enfoque</button><button id="focusreset">Reiniciar</button></div><div class="big" id="focustimer">25:00</div><p class="small" id="focusstatus">El temporizador funciona mientras esta página permanezca abierta.</p></div>
</section>

<section id="screen" class="panel hidden">
<h2>📱 Control del tiempo de pantalla</h2><p>Registra el tiempo diario que ves en los ajustes de tu celular. El registro manual no mide automáticamente el uso del dispositivo.</p>
<label for="screenhours">Horas de pantalla de hoy</label><input id="screenhours" type="number" min="0" max="24" step=".25" placeholder="Ej. 3.5">
<div class="actions"><button class="primary" id="savescreen">Guardar registro</button></div><p id="screenmsg"></p>
<div class="grid"><div class="tile"><h3>Android</h3><p>Busca en Ajustes la opción <b>Bienestar digital y controles parentales</b> para revisar el tiempo de uso y configurar límites o modos de concentración.</p></div><div class="tile"><h3>iPhone</h3><p>Busca en Ajustes la opción <b>Tiempo en pantalla</b> para consultar la actividad y establecer descansos o límites.</p></div></div>
<p class="small">Meta sugerida: observar tus hábitos y equilibrar el tiempo de pantalla con el estudio, el descanso y el movimiento; no se trata de competir por usar el celular menos que otras personas.</p>
</section>

<section id="breaks" class="panel hidden">
<h2>🧘 Recordatorios de pausas activas</h2><p>Programa una pausa para levantarte, caminar un poco y estirar suavemente. Evita hacer movimientos que te causen molestias.</p>
<div class="row"><div><label for="breakevery">Recordarme cada (minutos)</label><input id="breakevery" type="number" min="10" max="180" value="45"></div><div><label for="breakduration">Duración de la pausa (minutos)</label><input id="breakduration" type="number" min="1" max="15" value="3"></div></div>
<div class="actions"><button class="primary" id="breakon">Activar recordatorio</button><button id="breakoff">Pausar recordatorio</button><button id="breakdone">Ya hice una pausa (+5 puntos)</button></div><p id="breakmsg" aria-live="polite">Los avisos funcionan mientras esta página esté abierta.</p>
<div class="tile"><b>Ideas para una pausa:</b><ul><li>Caminar por la habitación o el patio.</li><li>Mirar a lo lejos y descansar la vista.</li><li>Estirar suavemente brazos y hombros.</li><li>Tomar agua.</li></ul></div>
</section>

<section id="activity" class="panel hidden">
<h2>🏃 Registro de actividad física</h2><label for="actname">Actividad</label><input id="actname" placeholder="Ej. caminar, bailar, vóley, bicicleta">
<div class="row"><div><label for="actmins">Duración (minutos)</label><input id="actmins" type="number" min="1" placeholder="20"></div><div><label for="actdate">Fecha</label><input id="actdate" type="date"></div></div>
<div class="actions"><button class="primary" id="saveact">Guardar actividad (+10 puntos)</button></div><ul id="actlist"></ul>
<div class="tile"><h3>Conecta tus hábitos con otras herramientas</h3><p><b>Google Fit / Health Connect:</b> puedes revisar actividad y pasos en las aplicaciones compatibles de tu teléfono. Esta página no se conecta directamente a esas cuentas.</p><p><b>Desafío personal:</b> elige actividades que disfrutes y registra tus avances sin compararte con los demás.</p></div>
</section>

<section id="music" class="panel hidden">
<h2>🎧 Música para estudiar y relajarte</h2><p>Escuchar música tranquila puede acompañar una sesión de estudio o un momento de descanso. Elige música que no te distraiga y mantén un volumen cómodo.</p>
<div class="grid">
<div class="tile"><h3>🎹 Música instrumental</h3><p>Para acompañar la concentración.</p><a target="_blank" rel="noopener" href="https://www.youtube.com/results?search_query=musica+instrumental+para+estudiar">Buscar en YouTube</a></div>
<div class="tile"><h3>🌧️ Sonidos de lluvia</h3><p>Para crear un ambiente tranquilo.</p><a target="_blank" rel="noopener" href="https://www.youtube.com/results?search_query=sonido+de+lluvia+para+estudiar">Buscar sonidos</a></div>
<div class="tile"><h3>🎼 Lo-fi para estudiar</h3><p>Para una sesión de tareas.</p><a target="_blank" rel="noopener" href="https://www.youtube.com/results?search_query=lofi+study+music">Escuchar lo-fi</a></div>
</div><p class="small">Los enlaces abren resultados de búsqueda; la reproducción depende de la plataforma y conexión a internet.</p>
</section>

<section id="stats" class="panel hidden">
<h2>📊 Mis estadísticas</h2><div class="grid">
<div class="tile"><p class="small">Tiempo de pantalla registrado hoy</p><div class="big" id="todayScreen">—</div></div>
<div class="tile"><p class="small">Minutos de actividad registrados hoy</p><div class="big" id="todayMove">0</div></div>
<div class="tile"><p class="small">Tareas completadas</p><div class="big" id="tasksDone">0</div></div>
<div class="tile"><p class="small">Puntos acumulados</p><div class="big" id="statPoints">0</div></div>
</div><h3>Actividad de los últimos registros</h3><ul id="history"></ul><p class="small">Las estadísticas reflejan únicamente los datos que tú registras en Muévete+.</p>
</section>

<section id="challenge" class="panel hidden">
<h2>🏆 Desafío de hábitos saludables</h2><p>Completa tus propios objetivos diarios y observa tu progreso. Puedes proponer este desafío en tu salón, cada estudiante registra sus logros en su propio dispositivo.</p>
<div class="grid"><div class="tile"><h3>🚶 Muévete</h3><p>Registra una caminata, deporte o baile que disfrutes.</p></div><div class="tile"><h3>📚 Concéntrate</h3><p>Completa una tarea durante un bloque sin distracciones.</p></div><div class="tile"><h3>🧘 Haz una pausa</h3><p>Interrumpe un periodo largo sentado con movimiento suave.</p></div><div class="tile"><h3>🌙 Organiza tu descanso</h3><p>Prepara tus actividades de mañana y respeta tu hora de dormir.</p></div></div>
<h3>Recompensas simbólicas</h3><p>🌸 10 puntos: Semilla saludable · 🌷 30 puntos: Brote activo · 🌳 60 puntos: Árbol en crecimiento · 🏵️ 100 puntos: Embajador/a del bienestar</p>
<p class="small">Los puntos son motivacionales, no premios por restringir necesidades básicas ni por competir con otros.</p>
</section>
</main><footer>Muévete+ · Tu bienestar también cuenta 🌷</footer>
<script>
const $=id=>document.getElementById(id), today=()=>new Date().toISOString().slice(0,10);
$('taskdate').value=today();$('actdate').value=today();
let data=JSON.parse(localStorage.getItem('mplus_data')||'{}');
data.points=data.points||0;data.tasks=data.tasks||[];data.activities=data.activities||[];data.screens=data.screens||{};data.schedules=data.schedules||{};
function save(){localStorage.setItem('mplus_data',JSON.stringify(data));render()}
function award(n){data.points+=n;save()}
function render(){ $('points').textContent=data.points;$('statPoints').textContent=data.points;
$('streak').textContent=new Set([...Object.keys(data.screens),...data.activities.map(a=>a.date)]).size;
let sc=data.screens[today()];$('todayScreen').textContent=sc==null?'—':sc+' h';
$('todayMove').textContent=data.activities.filter(a=>a.date===today()).reduce((s,a)=>s+a.minutes,0);
$('tasksDone').textContent=data.tasks.filter(t=>t.done).length;
$('tasklist').innerHTML='';data.tasks.forEach((t,i)=>{let li=document.createElement('li'),lab=document.createElement('label'),cb=document.createElement('input'),span=document.createElement('span');lab.className='taskline';cb.type='checkbox';cb.checked=t.done;cb.onchange=()=>{if(cb.checked&&!t.done)data.points+=2;t.done=cb.checked;save()};span.textContent=t.name+(t.date?' · '+t.date:'');if(t.done)span.style.textDecoration='line-through';lab.append(cb,span);li.append(lab);$('tasklist').append(li)});
$('actlist').innerHTML='';data.activities.slice().reverse().forEach(a=>{let li=document.createElement('li');li.textContent=a.name+' · '+a.minutes+' min · '+a.date;$('actlist').append(li)});
$('history').innerHTML='';[...data.activities].slice(-8).reverse().forEach(a=>{let li=document.createElement('li');li.textContent=a.date+': '+a.name+' ('+a.minutes+' min)';$('history').append(li)});
renderSchedules()}
document.querySelectorAll('nav button').forEach(b=>b.onclick=()=>{document.querySelectorAll('nav button').forEach(x=>x.classList.remove('active'));b.classList.add('active');document.querySelectorAll('main section').forEach(s=>s.classList.add('hidden'));$(b.dataset.tab).classList.remove('hidden');if(b.dataset.tab==='stats')render()});
function renderSchedules(){let d=$('weekday').value,items=data.schedules[d]||[];$('schedulelist').innerHTML='<h3>'+d+'</h3>';let tbl=document.createElement('table');tbl.innerHTML='<tr><th>Hora</th><th>Actividad</th><th></th></tr>';items.forEach((it,i)=>{let tr=document.createElement('tr');tr.innerHTML='<td></td><td></td><td></td>';tr.children[0].textContent=it.time;tr.children[1].textContent=it.text;let del=document.createElement('button');del.textContent='Quitar';del.onclick=()=>{items.splice(i,1);data.schedules[d]=items;save()};tr.children[2].append(del);tbl.append(tr)});$('schedulelist').append(tbl)}
$('weekday').onchange=()=>{let d=$('weekday').value;$('schoolend').value=d==='Lunes'?'13:00':(['Sábado','Domingo'].includes(d)?'':'13:35');renderSchedules()};
$('saveplan').onclick=()=>{let d=$('weekday').value,arr=data.schedules[d]||[];let start=$('schoolstart').value,end=$('schoolend').value,notes=$('classnotes').value.trim();if(start&&end)arr.unshift({time:start+'–'+end,text:'Colegio'+(notes?' · '+notes:'')});let time=$('planstart').value,task=$('planitem').value.trim();if(time&&task)arr.push({time,text:task});data.schedules[d]=arr;$('classnotes').value='';$('planitem').value='';save()};
$('addtask').onclick=()=>{let n=$('tasktext').value.trim();if(!n)return;data.tasks.push({name:n,date:$('taskdate').value,done:false});$('tasktext').value='';save()};
$('savescreen').onclick=()=>{let v=Number($('screenhours').value);if($('screenhours').value===''||v<0||v>24){$('screenmsg').textContent='Ingresa un valor entre 0 y 24 horas.';return}data.screens[today()]=v;$('screenmsg').textContent='Registro guardado. ¡Gracias por observar tus hábitos!';save()};
$('saveact').onclick=()=>{let n=$('actname').value.trim(),m=Number($('actmins').value);if(!n||!m||m<1)return alert('Completa la actividad y los minutos.');data.activities.push({name:n,minutes:m,date:$('actdate').value||today()});data.points+=10;$('actname').value='';$('actmins').value='';save()};
let breakInt=null;function stopBreak(){if(breakInt){clearInterval(breakInt);breakInt=null}}$('breakon').onclick=()=>{stopBreak();let mins=Math.max(10,Number($('breakevery').value)||45);$('breakmsg').textContent='Recordatorio activado: cada '+mins+' minutos mientras la página esté abierta.';breakInt=setInterval(()=>{alert('🌸 ¡Pausa activa! Levántate, camina un poco y descansa la vista.');},mins*60000)};$('breakoff').onclick=()=>{stopBreak();$('breakmsg').textContent='Recordatorios pausados.'};$('breakdone').onclick=()=>{data.points+=5;$('breakmsg').textContent='¡Muy bien! Sumaste 5 puntos.';save()};
let fsec=1500,fint=null;function showFocus(){$('focustimer').textContent=String(Math.floor(fsec/60)).padStart(2,'0')+':'+String(fsec%60).padStart(2,'0')}$('focusstart').onclick=()=>{if(fint)return;fsec=Math.max(5,Math.min(90,Number($('focusmins').value)||25))*60;showFocus();$('focusstatus').textContent='¡Modo concentración!';fint=setInterval(()=>{fsec--;showFocus();if(fsec<=0){clearInterval(fint);fint=null;$('focusstatus').textContent='¡Bloque completado! Tómate un descanso.';data.points+=5;save();}},1000)};$('focusreset').onclick=()=>{clearInterval(fint);fint=null;fsec=(Number($('focusmins').value)||25)*60;showFocus();$('focusstatus').textContent='Temporizador reiniciado.'};
render();showFocus();
</script></body></html>
