# PROYECTO-FINAL-CONTABILIDAD-II
<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="description" content="Dulce Andrea Castro Bamaca">
<title>Contabilidad II | Tema: Contabilidad Administrativa</title>
<style>
:root{--navy:#102f5d;--blue:#0756a4;--blue2:#1268b3;--gold:#cc3433;--cream:#f5f7fa;--ink:#243447;--muted:#617286;--white:#fff;--line:#dce5ee;--green:#16735b;--red:#cc3433}
*{box-sizing:border-box;scroll-behavior:smooth}
body{margin:0;font-family:Inter,"Segoe UI",Arial,sans-serif;background:var(--cream);color:var(--ink);line-height:1.65}
header{background:linear-gradient(125deg,#102f5d 0%,#0756a4 68%,#cc3433 100%);color:white;padding:22px max(5vw,20px) 76px}
.topbar{max-width:1150px;margin:auto;display:flex;justify-content:space-between;align-items:center;gap:20px}
.brand{display:flex;align-items:center;gap:12px;font-weight:800;letter-spacing:.3px}
.logo{width:45px;height:45px;border:2px solid #fff8;border-radius:12px;display:grid;place-items:center;font-size:20px;color:var(--red);font-weight:900;background:#fff}
nav{display:flex;gap:17px;flex-wrap:wrap;justify-content:flex-end}
nav a{color:#fff;text-decoration:none;font-size:.91rem;font-weight:600;opacity:.92}
nav a:hover{color:var(--gold)}
.hero{max-width:1150px;margin:55px auto 0;display:grid;grid-template-columns:1.4fr .6fr;align-items:center;gap:30px}
.eyebrow{text-transform:uppercase;letter-spacing:2px;color:#fff;font-size:.78rem;font-weight:800}
h1{font-size:clamp(2.2rem,5vw,4.3rem);line-height:1.08;margin:12px 0 18px;max-width:760px}
.hero p{font-size:1.08rem;color:#e4edf5;max-width:690px}
.hero-card{background:#ffffff12;border:1px solid #ffffff35;border-radius:20px;padding:24px;backdrop-filter:blur(8px)}
.hero-card strong{display:block;color:#fff;font-size:2.2rem}
.hero-card span{font-size:.94rem;color:#edf5fc}
.button{display:inline-block;margin-top:14px;background:var(--red);color:#fff;padding:12px 18px;border-radius:9px;text-decoration:none;font-weight:800}
main{max-width:1150px;margin:-35px auto 60px;padding:0 20px}
.quicklinks{display:grid;grid-template-columns:repeat(4,1fr);gap:14px}
.quicklinks a{background:white;border:1px solid var(--line);padding:18px;border-radius:14px;text-decoration:none;color:var(--ink);box-shadow:0 7px 20px #1936500a;font-weight:750}
.quicklinks a span{display:block;color:var(--blue);font-size:1.45rem;margin-bottom:5px}
section{padding-top:52px;scroll-margin-top:20px}
.section-head{max-width:760px;margin-bottom:23px}
.kicker{color:var(--blue2);font-size:.78rem;font-weight:850;letter-spacing:1.6px;text-transform:uppercase}
h2{color:var(--navy);font-size:clamp(1.7rem,3vw,2.45rem);line-height:1.2;margin:7px 0 12px}
h3{color:var(--navy);margin-top:0;line-height:1.3}
.lead{font-size:1.04rem;color:var(--muted)}
.grid{display:grid;grid-template-columns:repeat(3,1fr);gap:17px}
.card{background:white;border:1px solid var(--line);border-radius:15px;padding:22px;box-shadow:0 6px 18px #19365008}
.card p:last-child{margin-bottom:0}
.icon{width:40px;height:40px;border-radius:11px;background:#e9f2fb;color:var(--blue);display:grid;place-items:center;font-size:1.2rem;margin-bottom:13px}
.callout{border-left:4px solid var(--red);background:#fff5f5;padding:17px 20px;border-radius:0 12px 12px 0;margin:18px 0}
table{width:100%;border-collapse:collapse;background:white;border-radius:12px;overflow:hidden;margin:15px 0;border:1px solid var(--line)}
th,td{text-align:left;padding:13px 15px;border-bottom:1px solid var(--line);vertical-align:top}
th{background:var(--navy);color:white}
tr:last-child td{border-bottom:0}
.formula{background:#edf4fb;border:1px solid #d4e4f4;padding:13px 16px;border-radius:10px;color:#123e69;font-family:Consolas,monospace;font-weight:700;overflow-wrap:anywhere}
.example{background:#f4faf7;border:1px solid #cde8dc;padding:16px;border-radius:12px;margin-top:13px}
.example b{color:var(--green)}
.tools-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:18px}
.tool-card{background:white;border:1px solid var(--line);border-radius:15px;padding:22px}
.tool-card .num{display:inline-grid;place-items:center;width:34px;height:34px;background:var(--blue);color:white;border-radius:10px;font-weight:800;margin-bottom:12px}
.pill{display:inline-block;border-radius:99px;background:#eaf2fa;color:var(--blue);font-size:.78rem;font-weight:800;padding:4px 10px;margin-bottom:8px}
.photo-grid{display:grid;grid-template-columns:repeat(2,1fr);gap:18px}
.photo-slot{background:white;border:2px dashed #aabed0;border-radius:15px;min-height:235px;padding:24px;display:flex;flex-direction:column;align-items:center;justify-content:center;text-align:center}
.photo-slot .camera{font-size:2rem;margin-bottom:8px}
.photo-slot p{color:var(--muted);max-width:340px}
.photo-slot input{max-width:100%;margin-top:10px}
.preview{display:none;max-width:100%;max-height:240px;object-fit:contain;border-radius:10px;margin-top:12px}
.resources a{color:var(--blue);font-weight:650}
footer{background:var(--navy);color:#d9e6f1;padding:30px 20px;text-align:center}
footer strong{color:var(--gold)}
.small{font-size:.88rem;color:var(--muted)}
@media(max-width:850px){.hero{grid-template-columns:1fr;margin-top:35px}.quicklinks{grid-template-columns:repeat(2,1fr)}.grid{grid-template-columns:repeat(2,1fr)}nav{gap:10px}.tools-grid{grid-template-columns:1fr}}
@media(max-width:560px){.topbar{align-items:flex-start;flex-direction:column}.hero{margin-top:25px}.quicklinks,.grid,.photo-grid{grid-template-columns:1fr}main{padding:0 14px}header{padding-left:18px;padding-right:18px}th,td{padding:10px;font-size:.91rem}}
@media print{nav,.button,input{display:none!important}header{padding-bottom:30px}main{margin:0 auto}.card,.tool-card{break-inside:avoid}body{background:white}}
</style>
</head>
<body>
<header id="inicio">
  <div class="topbar">
    <div class="brand"><div class="logo" style="width:58px;height:58px;border:2px solid #fff;background:#fff;border-radius:50%;padding:3px;overflow:hidden"><img src="https://commons.wikimedia.org/wiki/Special:FilePath/Escudo_de_la_universidad_Mariano_G%C3%A1lvez_Guatemala.svg" alt="Escudo de la Universidad Mariano Gálvez" style="width:100%;height:100%;object-fit:contain" onerror="this.style.display='none';this.parentElement.textContent='UMG';this.parentElement.style.color='#cc3433';this.parentElement.style.fontSize='14px'"></div><div>UNIVERSIDAD MARIANO GÁLVEZ<br><span style="font-size:.78rem;font-weight:600;opacity:.9">CONTABILIDAD ADMINISTRATIVA</span></div></div>
    <nav aria-label="Navegación principal">
      <a href="#fundamentos">Fundamentos</a><a href="#comparacion">Tipos de contabilidad</a><a href="#herramientas">Herramientas</a><a href="#evidencias">Evidencias</a>
    </nav>
  </div>
  <div class="hero">
    <div>
      <div class="eyebrow">Recurso académico · Contabilidad II</div>
      <h1>Información contable para decidir mejor.</h1>
      <p>Un recorrido práctico por los conceptos y herramientas que ayudan a planificar, controlar recursos y tomar decisiones gerenciales con fundamento.</p>
      <a class="button" href="#fundamentos">Explorar el contenido ↓</a>
    </div>
    <div class="hero-card"><strong>Decidir con datos</strong><span>Planificación · Control · Análisis · Evaluación financiera</span><hr style="border:0;border-top:1px solid #ffffff35;margin:20px 0"><span>Proyecto final individual<br>Curso: Contabilidad II (Contabilidad Administrativa)</span></div>
  </div>
</header>
<main>
  <div class="quicklinks">
    <a href="#fundamentos"><span>01</span>Fundamentos</a>
    <a href="#comparacion"><span>02</span>Tipos de contabilidad</a>
    <a href="#herramientas"><span>03</span>Herramientas prácticas</a>
    <a href="#evidencias"><span>04</span>Vida universitaria</a>
  </div>

  <section id="fundamentos">
    <div class="section-head"><div class="kicker">01 · Bases conceptuales</div><h2>¿Qué es la Contabilidad Administrativa?</h2><p class="lead">Es un sistema que identifica, mide, analiza e interpreta información financiera y operativa para apoyar la planificación, el control y las decisiones internas de una organización.</p></div>
    <div class="grid">
      <article class="card"><div class="icon">◎</div><h3>Objetivos principales</h3><ul><li>Planificar las operaciones y los presupuestos.</li><li>Controlar costos, gastos y resultados.</li><li>Evaluar el desempeño de áreas y responsables.</li><li>Apoyar decisiones oportunas.</li></ul></article>
      <article class="card"><div class="icon">↗</div><h3>Importancia gerencial</h3><p>Convierte datos en información útil para comparar alternativas, detectar desviaciones, asignar recursos y estimar consecuencias económicas antes de actuar.</p></article>
      <article class="card"><div class="icon">▦</div><h3>Usuarios y enfoque</h3><p>Se dirige principalmente a gerentes y responsables internos. Puede incluir datos históricos, estimaciones, indicadores operativos y proyecciones futuras.</p></article>
    </div>
    <div class="callout"><strong>Idea clave:</strong> la información contable no solo explica qué ocurrió; también ayuda a decidir qué conviene hacer a continuación.</div>
  </section>

  <section id="comparacion">
    <div class="section-head"><div class="kicker">02 · Diferencias esenciales</div><h2>Administrativa, financiera y de costos</h2><p class="lead">Son áreas relacionadas, pero tienen objetivos y usuarios diferentes.</p></div>
    <table>
      <thead><tr><th>Aspecto</th><th>Contabilidad administrativa</th><th>Contabilidad financiera</th><th>Contabilidad de costos</th></tr></thead>
      <tbody>
        <tr><td><b>Propósito</b></td><td>Apoyar decisiones, planificación y control.</td><td>Informar sobre la situación y resultados de la entidad.</td><td>Determinar y analizar el costo de productos, servicios o procesos.</td></tr>
        <tr><td><b>Usuarios</b></td><td>Principalmente internos: gerentes y jefaturas.</td><td>Internos y externos: propietarios, acreedores e inversionistas, entre otros.</td><td>Principalmente operaciones, producción y gerencia.</td></tr>
        <tr><td><b>Enfoque temporal</b></td><td>Pasado, presente y futuro.</td><td>Principalmente información histórica.</td><td>Histórico y estimado, según el sistema de costos.</td></tr>
        <tr><td><b>Regulación</b></td><td>Se adapta a las necesidades internas de la organización.</td><td>Se prepara conforme al marco contable aplicable.</td><td>Depende del propósito, sistema de costeo y normas aplicables a los informes.</td></tr>
        <tr><td><b>Ejemplo</b></td><td>Decidir si conviene abrir una nueva sucursal.</td><td>Preparar estados financieros para usuarios externos.</td><td>Calcular el costo unitario de fabricar una mesa.</td></tr>
      </tbody>
    </table>
  </section>

  <section id="herramientas">
    <div class="section-head"><div class="kicker">03 · Aplicación práctica</div><h2>Herramientas de gestión contable</h2><p class="lead">Cada herramienta responde una pregunta distinta. Los datos de los ejemplos son ilustrativos y se expresan en quetzales (Q).</p></div>
    <div class="tools-grid">
      <article class="tool-card"><span class="num">1</span><div class="pill">Rentabilidad</div><h3>¿La empresa genera utilidad?</h3><p>Los indicadores de rentabilidad relacionan las ganancias con las ventas, los activos o el patrimonio. Permiten valorar qué tan bien se convierten los recursos en resultados.</p><div class="formula">Margen neto = (Utilidad neta / Ventas netas) × 100</div><div class="example"><b>Ejemplo:</b> utilidad neta Q12,000 y ventas netas Q100,000.<br>Margen neto = 12,000 / 100,000 × 100 = <b>12%</b>.</div><p><b>Interpretación:</b> por cada Q100 vendidos, quedan Q12 de utilidad neta, según los datos del ejemplo.</p></article>
      <article class="tool-card"><span class="num">2</span><div class="pill">Eficiencia</div><h3>¿Se aprovechan los recursos?</h3><p>La eficiencia compara los resultados obtenidos con los recursos utilizados. Se puede medir en unidades producidas por hora, ventas por empleado o costos reales frente a costos presupuestados.</p><div class="formula">Productividad laboral = Unidades producidas / Horas trabajadas</div><div class="example"><b>Ejemplo:</b> se fabrican 240 unidades en 30 horas.<br>Productividad = 240 / 30 = <b>8 unidades por hora</b>.</div><p><b>Interpretación:</b> el promedio de producción es de ocho unidades por cada hora de trabajo.</p></article>
      <article class="tool-card"><span class="num">3</span><div class="pill">Liquidez</div><h3>Análisis del flujo de efectivo</h3><p>El flujo de efectivo registra entradas y salidas de dinero. Se clasifica normalmente en actividades de operación, inversión y financiación. Ayuda a anticipar faltantes de efectivo y planificar pagos.</p><div class="formula">Flujo neto = Entradas de efectivo − Salidas de efectivo</div><div class="example"><b>Ejemplo:</b> entradas Q25,000 y salidas Q19,000.<br>Flujo neto = 25,000 − 19,000 = <b>Q6,000 positivo</b>.</div><p><b>Interpretación:</b> durante el período, las entradas superaron las salidas por Q6,000. Esto no equivale necesariamente a utilidad contable.</p></article>
      <article class="tool-card"><span class="num">4</span><div class="pill">Decisión gerencial</div><h3>¿Comprar o producir?</h3><p>Se comparan los costos relevantes de fabricar internamente con el precio de compra. Deben considerarse costos evitables, capacidad disponible, calidad, tiempos y confiabilidad del proveedor.</p><div class="formula">Costo de producir = Costos relevantes de fabricación</div><div class="example"><b>Ejemplo:</b> comprar 1,000 piezas cuesta Q8 por pieza: Q8,000. Producirlas implica Q5,500 de costos relevantes.<br><b>Diferencia: Q2,500</b> a favor de producir, si la calidad y demás condiciones son equivalentes.</div><p><b>Precaución:</b> no se deben incluir costos que no cambian entre alternativas ni ignorar costos de oportunidad relevantes.</p></article>
      <article class="tool-card"><span class="num">5</span><div class="pill">Situación financiera</div><h3>Análisis patrimonial</h3><p>Examina los activos, pasivos y patrimonio para entender los recursos de la empresa y cómo se financian. Un análisis comparativo y porcentual ayuda a identificar cambios y riesgos.</p><div class="formula">Ecuación contable: Activos = Pasivos + Patrimonio</div><div class="example"><b>Ejemplo:</b> activos Q150,000 y pasivos Q60,000.<br>Patrimonio = 150,000 − 60,000 = <b>Q90,000</b>.</div><p><b>Interpretación:</b> los recursos ascienden a Q150,000 y se financian con Q60,000 de obligaciones y Q90,000 de patrimonio.</p></article>
      <article class="tool-card"><span class="num">6</span><div class="pill">Evaluación de proyectos</div><h3>Valor Actual Neto (VAN)</h3><p>El VAN compara el valor presente de los flujos de efectivo futuros con la inversión inicial. La tasa de descuento refleja el rendimiento requerido y el riesgo considerado.</p><div class="formula">VAN = Σ [Flujoₜ / (1 + r)ᵗ] − Inversión inicial</div><div class="example"><b>Ejemplo:</b> inversión inicial Q10,000; ingreso de Q6,000 al final de cada uno de dos años; tasa 10%.<br>VAN = 6,000/1.10 + 6,000/1.10² − 10,000 ≈ <b>Q413.22</b>.</div><p><b>Interpretación:</b> el VAN positivo indica que el proyecto supera la rentabilidad requerida bajo estos supuestos.</p></article>
      <article class="tool-card"><span class="num">7</span><div class="pill">Evaluación de proyectos</div><h3>Tasa Interna de Retorno (TIR)</h3><p>La TIR es la tasa de descuento que hace que el VAN del proyecto sea igual a cero. Se compara con la tasa mínima requerida, considerando los riesgos y el contexto del proyecto.</p><div class="formula">0 = Σ [Flujoₜ / (1 + TIR)ᵗ] − Inversión inicial</div><div class="example"><b>Ejemplo:</b> inversión Q10,000 y flujos de Q6,000 al final de cada uno de dos años.<br>La TIR es aproximadamente <b>13.07%</b>.</div><p><b>Interpretación:</b> si la tasa requerida fuera 10%, la TIR sería superior a esa tasa. Conviene revisar también el VAN y otros factores antes de decidir.</p></article>
      <article class="tool-card"><span class="num">8</span><div class="pill">Planificación y control</div><h3>Presupuestos y análisis de variaciones</h3><p>El presupuesto establece una referencia para planificar ingresos, costos y gastos. Comparar el presupuesto con los resultados reales ayuda a investigar diferencias y tomar medidas correctivas.</p><div class="formula">Variación = Resultado real − Resultado presupuestado</div><div class="example"><b>Ejemplo:</b> costo presupuestado Q5,000 y costo real Q5,600.<br>Variación = 5,600 − 5,000 = <b>Q600 desfavorable</b> para el costo.</div><p><b>Interpretación:</b> se gastaron Q600 más de lo previsto; es necesario investigar la causa.</p></article>
    </div>
    <div class="callout"><strong>Nota:</strong> los indicadores deben interpretarse junto con el sector, el período, la calidad de los datos y los objetivos de la empresa. Ninguna cifra aislada sustituye un análisis completo.</div>
  </section>

  <section id="decisiones">
    <div class="section-head"><div class="kicker">04 · Toma de decisiones</div><h2>Cómo utilizar la información</h2><p class="lead">Un proceso ordenado ayuda a convertir el análisis en acciones responsables.</p></div>
    <div class="grid">
      <article class="card"><div class="icon">1</div><h3>Definir el problema</h3><p>Precisar la decisión que debe tomarse y el objetivo que se desea alcanzar.</p></article>
      <article class="card"><div class="icon">2</div><h3>Reunir información</h3><p>Identificar costos, ingresos, capacidad, riesgos y otras variables relevantes.</p></article>
      <article class="card"><div class="icon">3</div><h3>Comparar alternativas</h3><p>Aplicar indicadores y estimaciones usando supuestos claros y consistentes.</p></article>
      <article class="card"><div class="icon">4</div><h3>Elegir y ejecutar</h3><p>Seleccionar la alternativa que mejor se ajuste a los objetivos y restricciones.</p></article>
      <article class="card"><div class="icon">5</div><h3>Medir resultados</h3><p>Comparar los resultados reales con lo esperado e identificar desviaciones.</p></article>
      <article class="card"><div class="icon">6</div><h3>Mejorar</h3><p>Usar los aprendizajes para ajustar presupuestos, procesos y decisiones futuras.</p></article>
    </div>
  </section>

  <section id="evidencias">
    <div class="section-head"><div class="kicker">05 · Vida universitaria</div><h2>Evidencias de participación institucional</h2><p class="lead">Agrega tus fotografías reales de participación individual en las actividades solicitadas por la universidad durante el año en curso.</p></div>
    <div class="callout"><strong>Importante:</strong> esta sección debe contener evidencia auténtica de ambas actividades. Los espacios de abajo permiten seleccionar fotos desde tu computadora; las imágenes se muestran en esta página mientras permanezca abierta, pero no se suben a internet ni se guardan automáticamente en el archivo.</div>
    <div class="photo-grid">
      <div class="photo-slot"><div class="camera">📷</div><h3>Aniversario de la Universidad</h3><p>Coloca una fotografía en la que se evidencie tu participación individual. Puedes añadir la fecha y una breve descripción.</p><label for="fotoAniversario"><b>Seleccionar fotografía</b></label><input id="fotoAniversario" type="file" accept="image/*" onchange="previewImage(event,'previewAniversario')"><img id="previewAniversario" class="preview" alt="Vista previa de foto de aniversario"><label for="descAniversario">Descripción</label><input id="descAniversario" type="text" placeholder="Fecha y actividad"></div>
      <div class="photo-slot"><div class="camera">📷</div><h3>Convención de la Universidad</h3><p>Coloca una fotografía en la que se evidencie tu participación individual. Puedes añadir la fecha y una breve descripción.</p><label for="fotoConvencion"><b>Seleccionar fotografía</b></label><input id="fotoConvencion" type="file" accept="image/*" onchange="previewImage(event,'previewConvencion')"><img id="previewConvencion" class="preview" alt="Vista previa de foto de convención"><label for="descConvencion">Descripción</label><input id="descConvencion" type="text" placeholder="Fecha y actividad"></div>
    </div>
  </section>

  <section id="conclusion">
    <div class="section-head"><div class="kicker">06 · Cierre</div><h2>Conclusión</h2></div>
    <div class="card"><p>La Contabilidad Administrativa es una herramienta esencial para dirigir una organización, porque permite planificar, controlar y evaluar el uso de los recursos. Los análisis de rentabilidad, eficiencia, flujo de efectivo, costos relevantes, patrimonio y evaluación de inversiones aportan perspectivas complementarias para tomar decisiones mejor fundamentadas. Su utilidad depende de que la información sea confiable, se interprete en contexto y se acompañe de seguimiento y control.</p></div>
  </section>

  <section id="recursos" class="resources">
    <div class="section-head"><div class="kicker">07 · Recursos de consulta</div><h2>Para ampliar el aprendizaje</h2><p class="lead">Consulta materiales reconocidos para profundizar los conceptos. Verifica con el docente qué bibliografía exige el curso.</p></div>
    <div class="card">
      <ul>
        <li><a href="https://www.ifrs.org/" target="_blank" rel="noopener noreferrer">Fundación IFRS</a> — información sobre normas internacionales de información financiera.</li>
        <li><a href="https://www.cpa.org/" target="_blank" rel="noopener noreferrer">American Institute of Certified Public Accountants (AICPA)</a> — recursos profesionales de contabilidad.</li>
        <li><a href="https://www.investor.gov/financial-tools-calculators" target="_blank" rel="noopener noreferrer">Investor.gov — herramientas y calculadoras financieras</a> — apoyo para comprender conceptos de inversión.</li>
      </ul>
      <p class="small">Los ejemplos y cálculos de esta página son didácticos. No sustituyen la revisión de los materiales impartidos en clase ni la asesoría profesional.</p>
    </div>
  </section>
  <div style="text-align:center;margin-top:35px"><a class="button" href="#inicio">↑ Volver al inicio</a> <button class="button" onclick="window.print()" style="border:0;cursor:pointer;font:inherit">Imprimir / Guardar en PDF</button></div>
</main>
<footer><strong>Contabilidad Administrativa</strong><br>Proyecto final individual · Contabilidad II · Universidad Mariano Gálvez de Guatemala<br><span style="font-size:.85rem">Completa los datos personales y agrega tus evidencias antes de entregar.</span></footer>
<script>
function previewImage(event, id) {
  const img = document.getElementById(id);
  const file = event.target.files && event.target.files[0];
  if (!file) { img.style.display = 'none'; return; }
  const reader = new FileReader();
  reader.onload = function(e) { img.src = e.target.result; img.style.display = 'block'; };
  reader.readAsDataURL(file);
}
</script>
</body>
</html>
