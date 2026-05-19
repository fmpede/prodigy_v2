# Nomade × Prodigy — Partnership Microsite

Propuesta interactiva de partnership entre Nomade Lab y Grupo Prodigy (agencia
programática LATAM con HQ en Bogotá y oficinas en CDMX, Quito y Miami). Foco
central: **acceso directo a 3 DSPs (DV360 · StackAdapt · Illumin)**, data & BI
custom para los clientes enterprise del roster, y AI advertising como nueva
superficie. Estructurada como capa técnica complementaria a la operación
programática que Prodigy ya tiene — no como reemplazo.

**Stack:** HTML + CSS + JS vanilla. Sin build step, sin framework, sin
dependencias externas (excepto Google Fonts). Idioma: español.

---

## Deploy a Vercel desde GitHub

### 1. Crear el repo en GitHub

```bash
# Desde esta carpeta
git init
git add .
git commit -m "Initial commit — Nomade x Prodigy microsite"
git branch -M main

# Creá el repo en github.com (vacío, sin README), después:
git remote add origin https://github.com/<tu-user>/nomade-prodigy-microsite.git
git push -u origin main
```

### 2. Conectar a Vercel

1. Andá a [vercel.com/new](https://vercel.com/new) e importá el repo nuevo.
2. **Framework Preset:** `Other` (HTML estático puro).
3. **Build Command:** dejar vacío.
4. **Output Directory:** dejar vacío.
5. **Install Command:** dejar vacío.
6. Click en **Deploy**.

---

## Preview local

```bash
python3 -m http.server 8000
# Abrí http://localhost:8000
```

---

## Estructura

```
.
├── index.html       # Microsite completo (HTML + CSS + JS inline)
├── vercel.json      # Configuración de cache headers
├── .gitignore
└── README.md
```

---

## Notas estratégicas

- **Prodigy es agencia programática, no advertiser directo.** El pitch es el playbook agencia (Asylum/Buentipo/CCOM): nos posicionamos como capa técnica complementaria detrás de su operación, no como reemplazo. Toda la copy fue revisada para nunca diagnosticar o implicar críticas sobre su setup actual.

- **Multi-DSP como diferenciador central.** El primer pillar del stack es "Multi-DSP · acceso directo" con DV360 + StackAdapt + Illumin listados explícitamente. Tag: "3 DSPs · direct access". Stat card en Quiénes Somos: "3 DSPs con acceso directo · DV360 · StackAdapt · Illumin".

- **Dashboard tabs alineadas con sus 3 líneas de producto:**
  - Gaming & E-Sports (su producto 3001)
  - Sports Marketing (su producto MVP)
  - Growth & Performance (su producto Growth)

  Los AI insights de cada vertical referencian explícitamente el valor de la operación multi-DSP (ej. "Cross-DSP arbitrage: StackAdapt está cotizando mismo inventario premium gaming a CPM 18% más bajo que DV360"; "Illumin CTV outperform: Illumin DSP está entregando viewability 94% en inventario CTV deportivo, vs. 87% baseline en DV360").

- **Verticals section también alineadas a sus líneas de producto** — refuerza que entendemos la estructura interna de Prodigy. La sección "Por qué importa para Prodigy" en el dashboard nombra explícitamente a BMW, Televisa, Banco Pichincha y Enel (de su roster real) y posiciona la data layer como "argumento de retención y upsell".

- **ChatGPT Ads framing LATAM:** "Track propio · sin presión inmediata", pipeline listo para cuando OpenAI abra LATAM. Posicionamiento first-mover en programmatic LATAM. (A diferencia de prospects US como Waveform donde es "activate now".)

- **Contacto:** Federico Pedemonte únicamente.

- **Geografía:** mencionamos 5 países (US, MX, CO, AR, ES). Prodigy opera en CO, MX, EC, US (Miami) — overlap natural en CO, MX y US.
