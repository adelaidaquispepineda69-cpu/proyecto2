<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Asfalto · Poleras urbanas para hombre</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Anton&family=DM+Sans:wght@400;500;700&display=swap" rel="stylesheet">
<style>
:root{
  --concreto:#D9DAD5; --tiza:#F7F7F4; --tinta:#14213D; --cobalto:#2D4BF5; --pintura:#E8B931;
  --display:"Anton","Impact","Arial Narrow",sans-serif;
  --body:"DM Sans","Helvetica Neue",Arial,sans-serif;
}
*{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{font-family:var(--body);background:var(--concreto);color:var(--tinta);line-height:1.5}
a{color:inherit}
button{font:inherit;cursor:pointer;color:inherit}
:focus-visible{outline:3px solid var(--cobalto);outline-offset:2px}
.wrap{max-width:1120px;margin:0 auto;padding:0 20px}

/* Cabecera */
header{position:sticky;top:0;z-index:20;background:var(--tinta);color:var(--tiza)}
header .wrap{display:flex;align-items:center;justify-content:space-between;height:60px}
.logo{font-family:var(--display);font-size:1.6rem;letter-spacing:.04em;text-decoration:none}
nav{display:flex;gap:22px;align-items:center}
nav a{text-decoration:none;font-weight:500;font-size:.95rem}
nav a:hover{color:var(--pintura)}
.cart-btn{background:var(--pintura);color:var(--tinta);border:0;padding:8px 14px;font-weight:700;border-radius:2px}

/* Hero */
.hero{background:var(--tinta);color:var(--tiza);overflow:hidden;padding:48px 0 0}
.hero .wrap{position:relative}
.hero h1{font-family:var(--display);font-weight:400;font-size:clamp(4.2rem,17vw,13rem);line-height:.88;letter-spacing:.01em;text-transform:uppercase}
.hero .sub{display:flex;flex-wrap:wrap;gap:20px 40px;align-items:flex-end;justify-content:space-between;padding:28px 0 36px;border-top:3px solid var(--pintura);margin-top:24px}
.hero p{max-width:34ch;font-size:1.1rem}
.cta{display:inline-block;background:var(--cobalto);color:#fff;text-decoration:none;font-weight:700;padding:14px 26px;border-radius:2px}
.cta:hover{background:#1f38c9}
.hero .tee-big{position:absolute;right:2%;top:-8px;width:min(34vw,320px);transform:rotate(8deg);opacity:.95}
@media(max-width:640px){.hero .tee-big{display:none}}

/* Tienda */
.shop{padding:56px 0 72px}
.shop h2{font-family:var(--display);font-weight:400;font-size:clamp(2.2rem,6vw,3.6rem);text-transform:uppercase;line-height:1}
.filters{display:flex;flex-wrap:wrap;gap:8px;margin:22px 0 32px}
.filters button{border:2px solid var(--tinta);background:transparent;padding:7px 16px;font-weight:500;border-radius:100px}
.filters button[aria-pressed="true"]{background:var(--tinta);color:var(--tiza)}
.grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(240px,1fr));gap:26px 20px}
.card{display:flex;flex-direction:column}
.thumb{background:var(--tiza);aspect-ratio:1/1.05;display:grid;place-items:center;position:relative;border-radius:2px}
.thumb svg{width:78%;height:auto}
.tag{position:absolute;left:10px;top:10px;background:var(--pintura);font-size:.8rem;font-weight:700;padding:2px 9px;border-radius:2px}
.card h3{font-size:1.05rem;font-weight:700;margin-top:12px}
.card .meta{font-size:.92rem;color:#3c4763}
.price{font-weight:700;font-size:1.15rem;margin:4px 0 10px}
.sizes{display:flex;gap:6px;margin-bottom:12px}
.sizes button{width:40px;height:36px;border:2px solid var(--tinta);background:transparent;font-weight:500;border-radius:2px}
.sizes button[aria-pressed="true"]{background:var(--tinta);color:var(--tiza)}
.add{background:var(--cobalto);color:#fff;border:0;padding:11px;font-weight:700;border-radius:2px;margin-top:auto}
.add:hover{background:#1f38c9}

/* Valores */
.info{background:var(--tiza);padding:48px 0}
.info .wrap{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:28px}
.info h3{font-size:1.1rem;margin-bottom:6px}
.info p{font-size:.97rem;max-width:36ch}

/* Pie */
footer{background:var(--tinta);color:var(--tiza);padding:36px 0;font-size:.95rem}
footer .wrap{display:flex;flex-wrap:wrap;gap:16px;justify-content:space-between;align-items:center}

/* Carrito */
.drawer{position:fixed;inset:0 0 0 auto;width:min(380px,100%);background:var(--tiza);z-index:40;transform:translateX(100%);transition:transform .25s;display:flex;flex-direction:column;box-shadow:-8px 0 30px rgba(20,33,61,.25)}
.drawer.open{transform:none}
.drawer header{position:static;background:var(--tinta)}
.drawer header button{background:none;border:0;color:var(--tiza);font-size:1.6rem}
.items{flex:1;overflow:auto;padding:16px 20px}
.item{display:flex;justify-content:space-between;gap:10px;padding:12px 0;border-bottom:1px solid var(--concreto)}
.item small{display:block;color:#3c4763}
.item button{border:0;background:none;color:var(--cobalto);font-weight:700;text-decoration:underline}
.empty{padding:20px 0}
.foot{padding:16px 20px;border-top:3px solid var(--pintura)}
.total{display:flex;justify-content:space-between;font-weight:700;font-size:1.15rem;margin-bottom:12px}
.foot .cta{display:block;text-align:center}
.foot .cta[aria-disabled="true"]{opacity:.45;pointer-events:none}
@media(prefers-reduced-motion:reduce){*{transition:none!important;scroll-behavior:auto!important}}
</style>
</head>
<body>

<svg width="0" height="0" style="position:absolute" aria-hidden="true">
  <symbol id="tee" viewBox="0 0 200 220">
    <path d="M62 18 L18 40 L2 88 L38 100 L46 82 L46 206 L154 206 L154 82 L162 100 L198 88 L182 40 L138 18 C130 38 70 38 62 18 Z" fill="currentColor"/>
    <path d="M62 18 C70 38 130 38 138 18" fill="none" stroke="rgba(0,0,0,.25)" stroke-width="5"/>
  </symbol>
</svg>

<header>
  <div class="wrap">
    <a class="logo" href="#">ASFALTO</a>
    <nav>
      <a href="#tienda">Poleras</a>
      <a href="#envios">Envíos</a>
      <button class="cart-btn" id="openCart" aria-label="Abrir carrito">Carrito (<span id="count">0</span>)</button>
    </nav>
  </div>
</header>

<section class="hero">
  <div class="wrap">
    <svg class="tee-big" viewBox="0 0 200 220" style="color:var(--cobalto)" aria-hidden="true">
      <use href="#tee"/>
      <text x="100" y="128" text-anchor="middle" font-family="Anton,Impact,sans-serif" font-size="30" fill="#F7F7F4">ASFALTO</text>
    </svg>
    <h1>Hecho<br>para la<br>calle</h1>
    <div class="sub">
      <p>Poleras de algodón grueso para hombre. Cortes oversize, básicas y gráficas que aguantan el día entero.</p>
      <a class="cta" href="#tienda">Ver poleras</a>
    </div>
  </div>
</section>

<main class="shop" id="tienda">
  <div class="wrap">
    <h2>Poleras</h2>
    <div class="filters" id="filters" role="group" aria-label="Filtrar por tipo">
      <button data-f="todas" aria-pressed="true">Todas</button>
      <button data-f="oversize" aria-pressed="false">Oversize</button>
      <button data-f="basica" aria-pressed="false">Básicas</button>
      <button data-f="grafica" aria-pressed="false">Gráficas</button>
    </div>
    <div class="grid" id="grid"></div>
  </div>
</main>

<section class="info" id="envios">
  <div class="wrap">
    <div><h3>Algodón de 220 g</h3><p>Tela gruesa que no se transparenta ni pierde la forma después de lavarla.</p></div>
    <div><h3>Envíos a todo el país</h3><p>Entrega en 2 a 5 días hábiles. Pagas al recibir en tu ciudad.</p></div>
    <div><h3>Cambio de talla</h3><p>Si no te queda, la cambiamos dentro de los 7 días sin costo.</p></div>
  </div>
</section>

<footer>
  <div class="wrap">
    <strong class="logo">ASFALTO</strong>
    <span>Pedidos por WhatsApp · Lunes a sábado, 9 a. m. a 8 p. m.</span>
  </div>
</footer>

<aside class="drawer" id="drawer" aria-label="Carrito de compras">
  <header>
    <div class="wrap" style="padding:0 20px"><strong>Tu carrito</strong><button id="closeCart" aria-label="Cerrar carrito">×</button></div>
  </header>
  <div class="items" id="items"></div>
  <div class="foot">
    <div class="total"><span>Total</span><span id="total">S/ 0</span></div>
    <a class="cta" id="buy" href="#" aria-disabled="true" target="_blank" rel="noopener">Pedir por WhatsApp</a>
  </div>
</aside>

<script>
// Cambia este número por el de tu tienda (código de país + número, sin + ni espacios)
const WHATSAPP = "51900000000";

const productos = [
  {id:1, nombre:"Concreto",  tipo:"oversize", color:"#2A2F3A", tinta:"#F7F7F4", texto:["JULIACA","ALTIPLANO"], precio:79, etiqueta:"Nuevo"},
  {id:2, nombre:"Neblina",   tipo:"oversize", color:"#B9BEC4", tinta:"#14213D", texto:["SIN","PRISA"], precio:79},
  {id:3, nombre:"Cobalto",   tipo:"grafica",  color:"#2D4BF5", tinta:"#F7F7F4", texto:["CALLE","24"], precio:69, etiqueta:"Más vendida"},
  {id:4, nombre:"Pintura",   tipo:"grafica",  color:"#E8B931", tinta:"#14213D", texto:["ASFALTO","CLUB"], precio:69},
  {id:5, nombre:"Basalto",   tipo:"basica",   color:"#14213D", tinta:"#F7F7F4", texto:[], precio:49},
  {id:6, nombre:"Tiza",      tipo:"basica",   color:"#F2F2EC", tinta:"#14213D", texto:[], precio:49},
  {id:7, nombre:"Ladrillo",  tipo:"oversize", color:"#8C3B2F", tinta:"#F7F7F4", texto:["RUTA","SUR"], precio:84},
  {id:8, nombre:"Musgo",     tipo:"basica",   color:"#4A5A44", tinta:"#F7F7F4", texto:[], precio:49}
];
const nombresTipo = {oversize:"Oversize", basica:"Básica", grafica:"Gráfica"};
const tallas = ["S","M","L","XL"];
const sel = {};      // talla elegida por producto
let carrito = [];    // {id, talla, qty}
let filtro = "todas";

const $ = s => document.querySelector(s);

function polera(p){
  const lineas = p.texto.map((t,i) =>
    `<text x="100" y="${112+i*30}" text-anchor="middle" font-family="Anton,Impact,sans-serif" font-size="${t.length>6?22:30}" fill="${p.tinta}">${t}</text>`
  ).join("");
  return `<svg viewBox="0 0 200 220" style="color:${p.color}" role="img" aria-label="Polera ${p.nombre}"><use href="#tee"/>${lineas}</svg>`;
}

function pintarTienda(){
  const lista = productos.filter(p => filtro === "todas" || p.tipo === filtro);
  $("#grid").innerHTML = lista.map(p => {
    sel[p.id] = sel[p.id] || "M";
    return `<article class="card">
      <div class="thumb">${p.etiqueta ? `<span class="tag">${p.etiqueta}</span>` : ""}${polera(p)}</div>
      <h3>${p.nombre}</h3>
      <div class="meta">${nombresTipo[p.tipo]} · Algodón 220 g</div>
      <div class="price">S/ ${p.precio}</div>
      <div class="sizes" role="group" aria-label="Talla de ${p.nombre}">
        ${tallas.map(t => `<button data-p="${p.id}" data-t="${t}" aria-pressed="${sel[p.id]===t}">${t}</button>`).join("")}
      </div>
      <button class="add" data-add="${p.id}">Agregar al carrito</button>
    </article>`;
  }).join("");
}

function pintarCarrito(){
  const n = carrito.reduce((a,i) => a + i.qty, 0);
  $("#count").textContent = n;
  const total = carrito.reduce((a,i) => a + i.qty * productos.find(p => p.id === i.id).precio, 0);
  $("#total").textContent = "S/ " + total;
  $("#items").innerHTML = carrito.length ? carrito.map((i,idx) => {
    const p = productos.find(x => x.id === i.id);
    return `<div class="item"><div><strong>${p.nombre}</strong><small>Talla ${i.talla} · ${i.qty} × S/ ${p.precio}</small></div><button data-del="${idx}">Quitar</button></div>`;
  }).join("") : `<p class="empty">Tu carrito está vacío. Elige una polera y su talla.</p>`;
  const buy = $("#buy");
  buy.setAttribute("aria-disabled", carrito.length ? "false" : "true");
  if(carrito.length){
    const detalle = carrito.map(i => `${i.qty} × ${productos.find(p=>p.id===i.id).nombre} (talla ${i.talla})`).join(", ");
    buy.href = `https://wa.me/${WHATSAPP}?text=` + encodeURIComponent(`Hola, quiero pedir: ${detalle}. Total: S/ ${total}`);
  } else buy.href = "#";
}

$("#filters").addEventListener("click", e => {
  const b = e.target.closest("button"); if(!b) return;
  filtro = b.dataset.f;
  document.querySelectorAll("#filters button").forEach(x => x.setAttribute("aria-pressed", x === b));
  pintarTienda();
});

$("#grid").addEventListener("click", e => {
  const t = e.target.closest("[data-t]");
  if(t){ sel[t.dataset.p] = t.dataset.t; pintarTienda(); return; }
  const a = e.target.closest("[data-add]");
  if(a){
    const id = +a.dataset.add, talla = sel[id];
    const ya = carrito.find(i => i.id === id && i.talla === talla);
    ya ? ya.qty++ : carrito.push({id, talla, qty:1});
    pintarCarrito();
    $("#drawer").classList.add("open");
  }
});

$("#items").addEventListener("click", e => {
  const d = e.target.closest("[data-del]");
  if(d){ carrito.splice(+d.dataset.del, 1); pintarCarrito(); }
});
$("#openCart").addEventListener("click", () => $("#drawer").classList.add("open"));
$("#closeCart").addEventListener("click", () => $("#drawer").classList.remove("open"));
document.addEventListener("keydown", e => { if(e.key === "Escape") $("#drawer").classList.remove("open"); });

pintarTienda();
pintarCarrito();
</script>
</body>
</html># proyecto2
tienda
