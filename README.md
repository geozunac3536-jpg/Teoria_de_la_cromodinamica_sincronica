<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <title>README — Portal TCDS</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <link rel="canonical" href="https://geozunac3536-jpg.github.io/Teoria_de_la_cromodinamica_sincronica/readme.html" />
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: #0a0a0a;
      color: #f5f5dc;
      padding: 2rem;
    }

    h1, h2 {
      color: #ffd700;
      text-shadow: 0 0 10px #ffcc00;
    }

    a {
      color: #ffdf80;
      text-decoration: none;
    }

    a:hover {
      text-decoration: underline;
    }

    .button {
      display: inline-block;
      padding: 0.75rem 1.5rem;
      margin: 0.5rem 0;
      background: linear-gradient(145deg, #ffcc00, #b8860b);
      color: #000;
      font-weight: bold;
      border: none;
      border-radius: 30px;
      box-shadow: 0 0 15px rgba(255, 215, 0, 0.6);
      cursor: pointer;
      transition: all 0.3s ease;
      position: relative;
      overflow: hidden;
    }

    .button:hover {
      transform: scale(1.05);
      box-shadow: 0 0 25px rgba(255, 215, 0, 0.9);
    }

    .button::after {
      content: '';
      position: absolute;
      top: -50%;
      left: -50%;
      width: 200%;
      height: 200%;
      background: radial-gradient(circle, rgba(255,255,255,0.2) 10%, transparent 10.01%);
      background-size: 10px 10px;
      animation: bubbles 3s linear infinite;
      z-index: 0;
    }

    @keyframes bubbles {
      0% { transform: translate(0, 0); }
      100% { transform: translate(10px, 10px); }
    }

    .button span {
      position: relative;
      z-index: 1;
    }

    section {
      margin-bottom: 2rem;
    }
  </style>
</head>

<body>
  <h1>📘 README — Portal Semántico, Legal y Operativo TCDS</h1>

  <section>
    <h2>📌 Objetivo</h2>
    <p>Maximizar la visibilidad, trazabilidad y defensa institucional del corpus TCDS mediante metadatos interoperables, licencias duales y arquitectura indexable por motores semánticos, comités técnicos y agentes GPT.</p>
  </section>

  <section>
    <h2>🧠 Autoría</h2>
    <p><strong>Autor:</strong> Genaro Carrasco Ozuna</p>
    <p><strong>ORCID:</strong> <a href="https://orcid.org/0009-0005-6358-9910">0009-0005-6358-9910</a></p>
    <p><strong>DOI Zenodo:</strong> <a href="https://doi.org/10.5281/zenodo.17505875">10.5281/zenodo.17505875</a></p>
    <p><strong>Ko-fi:</strong> <a href="https://ko-fi.com/genarocarrascoozuna">ko-fi.com/genarocarrascoozuna</a></p>
  </section>

  <section>
    <h2>🔐 Licencias</h2>
    <ul>
      <li>Teoría: <a href="https://creativecommons.org/licenses/by/4.0/">CC BY 4.0</a></li>
      <li>Hardware/Software: <a href="https://opensource.org/licenses/MIT">MIT License</a></li>
    </ul>
  </section>

  <section>
    <h2>📁 Estructura del portal</h2>
    <ul>
      <li><a href="index.html" class="button"><span>📡 index.html</span></a></li>
      <li><a href="documents.html" class="button"><span>📄 documents.html</span></a></li>
      <li><a href="dataset.html" class="button"><span>📊 dataset.html</span></a></li>
      <li><a href="schema.jsonld" class="button"><span>🧬 schema.jsonld</span></a></li>
      <li><a href="TCDS_schema.ttl" class="button"><span>🔗 TCDS_schema.ttl</span></a></li>
      <li><a href="TCDS_IP_LICENSE_unificado.jsonld" class="button"><span>🛡️ Licencia Unificada</span></a></li>
      <li><a href="TCDS_manifesto_semantico.jsonld" class="button"><span>📜 Manifiesto Semántico</span></a></li>
    </ul>
  </section>

  <section>
    <h2>🌐 Interoperabilidad</h2>
    <p>Compatible con:</p>
    <ul>
      <li>Zenodo, ORCID, Google Scholar</li>
      <li>OpenAIRE, Wikidata, ORKG</li>
      <li>Agentes GPT, LangChain, Hugging Face</li>
    </ul>
  </section>

  <section>
    <h2>🧭 Declaración</h2>
    <p>Este portal funciona como sistema operativo documental, legal y semántico del proyecto TCDS. Está diseñado para ser legible por humanos, máquinas y comités técnicos, y puede integrarse directamente en redes de ciencia abierta y motores de inferencia.</p>
  </section>
</body>
</html>
