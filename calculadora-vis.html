<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Calculadora de Presupuesto · Complemento VIS</title>
<style>
  *{box-sizing:border-box;margin:0;padding:0;}
  body{font-family:'Segoe UI',Arial,sans-serif;background:#F0EDE6;color:#3D2B1F;min-height:100vh;}

  .top-bar{background:#063d2c;padding:14px 20px;display:flex;align-items:center;justify-content:space-between;}
  .logo{font-size:18px;font-weight:700;color:#fff;letter-spacing:2px;}
  .logo span{color:#5DCAA5;}
  .top-sub{font-size:11px;color:rgba(255,255,255,0.6);}

  .hero{background:#085041;padding:28px 20px 22px;text-align:center;}
  .hero-badge{display:inline-block;background:rgba(93,202,165,0.2);color:#9FE1CB;font-size:11px;padding:4px 12px;border-radius:20px;margin-bottom:10px;border:0.5px solid rgba(93,202,165,0.3);}
  .hero h1{font-size:24px;font-weight:700;color:#fff;margin-bottom:6px;}
  .hero h1 span{color:#5DCAA5;}
  .hero p{font-size:13px;color:rgba(255,255,255,0.7);max-width:400px;margin:0 auto;}

  .container{max-width:520px;margin:0 auto;padding:20px 16px 40px;}

  .card{background:#fff;border-radius:14px;padding:18px;margin-bottom:14px;border:0.5px solid #D4C5B0;}
  .card-title{font-size:13px;font-weight:700;color:#3D2B1F;margin-bottom:14px;display:flex;align-items:center;gap:8px;}
  .num{width:22px;height:22px;border-radius:50%;background:#1D9E75;color:#fff;font-size:11px;font-weight:700;display:flex;align-items:center;justify-content:center;flex-shrink:0;}

  .opt-grid{display:grid;grid-template-columns:1fr 1fr;gap:8px;}
  .opt{border:1.5px solid #E8E4DC;border-radius:10px;padding:12px 10px;cursor:pointer;transition:all .15s;text-align:center;}
  .opt:hover{border-color:#1D9E75;background:#F5FBF8;}
  .opt.sel{border-color:#1D9E75;background:#EAF3DE;}
  .opt-icon{font-size:22px;margin-bottom:5px;}
  .opt-name{font-size:12px;font-weight:600;color:#3D2B1F;}
  .opt-desc{font-size:10px;color:#888;margin-top:2px;}
  .opt-tag{font-size:10px;color:#0F6E56;font-weight:600;margin-top:3px;}

  .slider-label{display:flex;justify-content:space-between;margin-bottom:8px;}
  .sl-txt{font-size:12px;color:#888;}
  .sl-val{font-size:14px;font-weight:700;color:#0F6E56;}
  input[type=range]{width:100%;accent-color:#1D9E75;height:4px;}
  .sl-hints{display:flex;justify-content:space-between;font-size:10px;color:#aaa;margin-top:4px;}

  .pkg-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:8px;}
  .pkg{border:1.5px solid #E8E4DC;border-radius:10px;overflow:hidden;cursor:pointer;transition:all .15s;}
  .pkg:hover{border-color:#1D9E75;}
  .pkg.sel{border-color:#1D9E75;}
  .pkg-head{padding:10px 8px 8px;text-align:center;}
  .pkg-icon{font-size:20px;margin-bottom:4px;}
  .pkg-name{font-size:11px;font-weight:700;color:#3D2B1F;}
  .pkg-price{font-size:13px;font-weight:700;color:#0F6E56;margin-top:3px;}
  .pkg-tag{font-size:9px;background:#EAF3DE;color:#3B6D11;padding:2px 6px;border-radius:10px;display:inline-block;margin-top:3px;}
  .pkg-feat{font-size:9px;color:#888;padding:6px 8px 10px;text-align:center;line-height:1.6;border-top:0.5px solid #f0ede6;}
  .pkg.sel .pkg-head{background:#EAF3DE;}

  .toggle-row{display:flex;align-items:center;justify-content:space-between;padding:10px 0;border-bottom:0.5px solid #f0ede6;}
  .toggle-row:last-child{border-bottom:none;padding-bottom:0;}
  .tl{font-size:12px;font-weight:600;color:#3D2B1F;}
  .ts{font-size:10px;color:#888;margin-top:2px;}
  .toggle{width:40px;height:22px;border-radius:11px;background:#ddd;position:relative;cursor:pointer;transition:background .2s;flex-shrink:0;}
  .toggle.on{background:#1D9E75;}
  .knob{position:absolute;top:3px;left:3px;width:16px;height:16px;border-radius:50%;background:#fff;transition:left .2s;box-shadow:0 1px 3px rgba(0,0,0,0.2);}
  .toggle.on .knob{left:21px;}

  .result{background:linear-gradient(135deg,#063d2c 0%,#0F6E56 100%);border-radius:14px;padding:20px;margin-bottom:14px;}
  .res-label{font-size:11px;color:rgba(255,255,255,0.65);margin-bottom:4px;}
  .res-price{font-size:36px;font-weight:700;color:#fff;line-height:1;}
  .res-pkg-tag{display:inline-block;background:rgba(93,202,165,0.2);color:#9FE1CB;font-size:11px;padding:3px 10px;border-radius:20px;margin-top:8px;border:0.5px solid rgba(93,202,165,0.3);}
  .res-grid{display:grid;grid-template-columns:1fr 1fr;gap:8px;margin-top:14px;}
  .res-box{background:rgba(255,255,255,0.1);border-radius:8px;padding:10px;}
  .res-box-lbl{font-size:9px;color:rgba(255,255,255,0.6);margin-bottom:3px;text-transform:uppercase;letter-spacing:.5px;}
  .res-box-val{font-size:12px;font-weight:700;color:#fff;}

  .fin-detail{background:#EAF3DE;border-radius:10px;padding:14px;margin-top:10px;display:none;}
  .fin-title{font-size:12px;font-weight:700;color:#085041;margin-bottom:8px;}
  .fin-row{display:flex;justify-content:space-between;font-size:12px;color:#3B6D11;padding:3px 0;}
  .fin-row.tot{border-top:0.5px solid #9FE1CB;margin-top:4px;padding-top:6px;font-weight:700;font-size:13px;}

  .cta-row{display:flex;gap:8px;}
  .btn-main{flex:1;background:#1D9E75;color:#fff;border:none;border-radius:10px;padding:14px;font-size:14px;font-weight:700;cursor:pointer;letter-spacing:.5px;}
  .btn-main:hover{background:#0F6E56;}
  .btn-wa{background:#fff;color:#1D9E75;border:1.5px solid #1D9E75;border-radius:10px;padding:14px 16px;font-size:13px;font-weight:700;cursor:pointer;}
  .btn-wa:hover{background:#EAF3DE;}

  .footer{text-align:center;padding:20px 0 10px;font-size:11px;color:#aaa;}
  .footer strong{color:#6B4C3B;}
</style>
</head>
<body>

<div class="top-bar">
  <div>
    <div class="logo">COMPLEMENTO <span>VIS</span></div>
    <div class="top-sub">Acabados y remodelaciones · Medellín</div>
  </div>
  <div style="font-size:11px;color:rgba(255,255,255,0.5);">complementovis.com</div>
</div>

<div class="hero">
  <div class="hero-badge">PMV 5 · Calculadora de presupuesto</div>
  <h1>¿Cuánto cuesta <span>tu cocina?</span></h1>
  <p>Descubre tu presupuesto en segundos. Sin compromiso ni visita previa.</p>
</div>

<div class="container">

  <div class="card">
    <div class="card-title"><div class="num">1</div> ¿Qué espacio quieres remodelar?</div>
    <div class="opt-grid">
      <div class="opt sel" id="o-cocina" onclick="sel('espacio','cocina',this)">
        <div class="opt-icon">🍳</div>
        <div class="opt-name">Cocina</div>
        <div class="opt-desc">El más solicitado</div>
        <div class="opt-tag">90.5% lo elige</div>
      </div>
      <div class="opt" id="o-bano" onclick="sel('espacio','bano',this)">
        <div class="opt-icon">🚿</div>
        <div class="opt-name">Baño</div>
        <div class="opt-desc">Enchape y grifería</div>
      </div>
      <div class="opt" id="o-completo" onclick="sel('espacio','completo',this)">
        <div class="opt-icon">🏠</div>
        <div class="opt-name">Apartamento completo</div>
        <div class="opt-desc">Todos los espacios</div>
        <div class="opt-tag">Mejor relación precio</div>
      </div>
      <div class="opt" id="o-pisos" onclick="sel('espacio','pisos',this)">
        <div class="opt-icon">🪟</div>
        <div class="opt-name">Pisos y paredes</div>
        <div class="opt-desc">Cerámica o laminado</div>
      </div>
    </div>
  </div>

  <div class="card">
    <div class="card-title"><div class="num">2</div> ¿Cuántos metros cuadrados?</div>
    <div class="slider-label">
      <span class="sl-txt">Área del apartamento</span>
      <span class="sl-val" id="m2-val">45 m²</span>
    </div>
    <input type="range" min="35" max="90" value="45" step="5" oninput="updM2(this.value)"/>
    <div class="sl-hints"><span>35 m²</span><span>VIS típico</span><span>90 m²</span></div>
  </div>

  <div class="card">
    <div class="card-title"><div class="num">3</div> ¿Qué nivel de acabado prefieres?</div>
    <div class="pkg-grid">
      <div class="pkg sel" id="p-fundamental" onclick="sel('paquete','fundamental',this)">
        <div class="pkg-head">
          <div class="pkg-icon">⭐</div>
          <div class="pkg-name">Fundamental</div>
          <div class="pkg-price" id="pr-fundamental">$41.5M</div>
        </div>
        <div class="pkg-feat">Esencial y funcional · 4–6 sem.</div>
      </div>
      <div class="pkg" id="p-estandar" onclick="sel('paquete','estandar',this)">
        <div class="pkg-head">
          <div class="pkg-icon">⭐⭐</div>
          <div class="pkg-name">Estándar</div>
          <div class="pkg-price" id="pr-estandar">$49.5M</div>
          <div class="pkg-tag">Más elegido</div>
        </div>
        <div class="pkg-feat">Diseño y confort · 6–8 sem.</div>
      </div>
      <div class="pkg" id="p-superior" onclick="sel('paquete','superior',this)">
        <div class="pkg-head">
          <div class="pkg-icon">⭐⭐⭐</div>
          <div class="pkg-name">Superior</div>
          <div class="pkg-price" id="pr-superior">$58.6M</div>
        </div>
        <div class="pkg-feat">Premium · 8–10 sem.</div>
      </div>
    </div>
  </div>

  <div class="card">
    <div class="card-title"><div class="num">4</div> Opciones adicionales</div>
    <div class="toggle-row">
      <div><div class="tl">Diseño 3D personalizado</div><div class="ts">Visualiza tu hogar antes de empezar · Incluido</div></div>
      <div class="toggle on" id="t-3d" onclick="tog('d3',this)"><div class="knob"></div></div>
    </div>
    <div class="toggle-row">
      <div><div class="tl">Financiación con banco aliado</div><div class="ts">Hasta 100% · Cuotas desde $350.000/mes</div></div>
      <div class="toggle" id="t-fin" onclick="tog('fin',this)"><div class="knob"></div></div>
    </div>
    <div class="toggle-row">
      <div><div class="tl">Garantía postventa extendida</div><div class="ts">Revisiones técnicas por 1 año adicional</div></div>
      <div class="toggle" id="t-post" onclick="tog('post',this)"><div class="knob"></div></div>
    </div>
  </div>

  <div class="result">
    <div class="res-label">Tu presupuesto estimado</div>
    <div class="res-price" id="res-price">$41.500.000</div>
    <div class="res-pkg-tag" id="res-tag">Paquete Fundamental · Cocina</div>
    <div class="res-grid">
      <div class="res-box"><div class="res-box-lbl">Tiempo de entrega</div><div class="res-box-val" id="res-tiempo">4–6 semanas</div></div>
      <div class="res-box"><div class="res-box-lbl">Visita técnica</div><div class="res-box-val">Gratis</div></div>
      <div class="res-box"><div class="res-box-lbl">Precio final</div><div class="res-box-val">Fijo en contrato</div></div>
      <div class="res-box"><div class="res-box-lbl">Garantía</div><div class="res-box-val" id="res-garantia">6 meses</div></div>
    </div>
    <div class="fin-detail" id="fin-detail">
      <div class="fin-title">Simulación de financiación</div>
      <div class="fin-row"><span>Cuota inicial (30%)</span><span id="fin-ini">—</span></div>
      <div class="fin-row"><span>Saldo financiado</span><span id="fin-sal">—</span></div>
      <div class="fin-row"><span>Plazo</span><span>36 meses</span></div>
      <div class="fin-row tot"><span>Cuota mensual aprox.</span><span id="fin-cuo">—</span></div>
    </div>
  </div>

  <div class="cta-row" style="margin-bottom:14px;">
    <button class="btn-main" onclick="cotizar()">Solicitar cotización formal</button>
    <button class="btn-wa" onclick="whatsapp()">📲 WhatsApp</button>
  </div>

  <div class="footer">
    Precio estimado con fines informativos · El precio final se confirma en visita técnica gratuita<br>
    <strong>Complemento VIS</strong> · complementovis.com · 324 241 8601
  </div>

</div>

<script>
const precios={
  cocina:{fundamental:41500000,estandar:49500000,superior:58600000},
  bano:{fundamental:12000000,estandar:16000000,superior:22000000},
  completo:{fundamental:58000000,estandar:75000000,superior:95000000},
  pisos:{fundamental:8000000,estandar:12000000,superior:18000000}
};
const tiempos={fundamental:'4–6 semanas',estandar:'6–8 semanas',superior:'8–10 semanas'};
const garantias={fundamental:'6 meses',estandar:'1 año',superior:'2 años'};
const espacioNom={cocina:'Cocina',bano:'Baño',completo:'Apartamento completo',pisos:'Pisos y paredes'};
const paqueteNom={fundamental:'Fundamental',estandar:'Estándar',superior:'Superior'};
const state={espacio:'cocina',paquete:'fundamental',m2:45,d3:true,fin:false,post:false};

function fmt(n){return '$'+Math.round(n).toLocaleString('es-CO');}

function calc(){
  let base=precios[state.espacio][state.paquete];
  let factor=1+(state.m2-45)*0.008;
  let total=base*factor;
  if(state.post) total+=2500000;

  document.getElementById('res-price').textContent=fmt(total);
  document.getElementById('res-tag').textContent='Paquete '+paqueteNom[state.paquete]+' · '+espacioNom[state.espacio];
  document.getElementById('res-tiempo').textContent=tiempos[state.paquete];
  document.getElementById('res-garantia').textContent=state.post?'2 años (extendida)':garantias[state.paquete];

  // Actualizar precios en paquetes
  ['fundamental','estandar','superior'].forEach(p=>{
    let b=precios[state.espacio][p]*factor;
    if(p!==state.paquete&&state.post) b+=2500000;
    document.getElementById('pr-'+p).textContent='$'+(b/1000000).toFixed(1)+'M';
  });

  const fd=document.getElementById('fin-detail');
  if(state.fin){
    fd.style.display='block';
    const ini=total*0.3, sal=total*0.7, cuo=sal/36;
    document.getElementById('fin-ini').textContent=fmt(ini);
    document.getElementById('fin-sal').textContent=fmt(sal);
    document.getElementById('fin-cuo').textContent=fmt(cuo)+'/mes';
  } else {
    fd.style.display='none';
  }
}

function sel(grupo,val,el){
  if(grupo==='espacio'){
    document.querySelectorAll('#o-cocina,#o-bano,#o-completo,#o-pisos').forEach(e=>e.classList.remove('sel'));
    state.espacio=val;
  } else {
    document.querySelectorAll('#p-fundamental,#p-estandar,#p-superior').forEach(e=>e.classList.remove('sel'));
    state.paquete=val;
  }
  el.classList.add('sel');
  calc();
}

function updM2(v){
  state.m2=parseInt(v);
  document.getElementById('m2-val').textContent=v+' m²';
  calc();
}

function tog(key,el){
  el.classList.toggle('on');
  state[key]=!state[key];
  calc();
}

function cotizar(){
  window.open('https://wa.me/573242418601?text=Hola!%20Usé%20la%20calculadora%20y%20quiero%20una%20cotización%20formal%20para%20mi%20apartamento.','_blank');
}
function whatsapp(){
  const msg=encodeURIComponent('Hola! Usé la calculadora de presupuesto. Me interesa el paquete '+paqueteNom[state.paquete]+' para '+espacioNom[state.espacio]+'. ¿Me pueden contactar?');
  window.open('https://wa.me/573242418601?text='+msg,'_blank');
}
</script>
</body>
</html>
