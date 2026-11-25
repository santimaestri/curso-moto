# Bloque 5 · Sistema de encendido con CDI

*Clases 10 y 11*

El CDI guarda energía en un capacitor y la suelta de golpe sobre la bobina de alta cuando la bobina captora le avisa que es el momento. La bobina de alta la convierte en miles de voltios y salta la chispa en la bujía.

<figure style="margin:1.5em 0">
<svg viewBox="0 0 760 264" role="img" aria-label="La captora da la orden y el CDI descarga sobre la bobina de alta" style="width:100%;height:auto;color:var(--md-typeset-color)" font-family="inherit" font-size="13">
  <defs><marker id="cdi-arrow" viewBox="0 0 10 10" refX="9" refY="5" markerWidth="6" markerHeight="6" orient="auto-start-reverse"><path d="M0 0L10 5L0 10z" fill="#9a9a9a"/></marker></defs>
  <text x="24" y="30" font-size="15" font-weight="600" fill="currentColor">La captora da la orden y el CDI descarga sobre la bobina de alta</text>
  <g fill="none" stroke="#9a9a9a" stroke-width="1.25">
    <path d="M208 100H224V140H240" marker-end="url(#cdi-arrow)"/>
    <path d="M208 212H224V172H240" marker-end="url(#cdi-arrow)"/>
    <path d="M420 156H455" marker-end="url(#cdi-arrow)"/>
    <path d="M605 156H632" marker-end="url(#cdi-arrow)"/>
  </g>
  <rect x="24" y="72" width="184" height="56" rx="8" fill="none" stroke="#9a9a9a" stroke-width="1.25"/>
  <text x="116" y="96" text-anchor="middle" font-weight="600" fill="currentColor">Batería</text>
  <text x="116" y="112" text-anchor="middle" font-size="11.5" fill="currentColor" opacity=".7">12 V por llave y fusible</text>
  <rect x="24" y="184" width="184" height="56" rx="8" fill="none" stroke="#9a9a9a" stroke-width="1.25"/>
  <text x="116" y="208" text-anchor="middle" font-weight="600" fill="currentColor">Bobina captora</text>
  <text x="116" y="224" text-anchor="middle" font-size="11.5" fill="currentColor" opacity=".7">pulso alterno, más de 5 V</text>
  <rect x="240" y="120" width="180" height="72" rx="8" fill="#e53935" fill-opacity=".12" stroke="#e53935" stroke-width="2"/>
  <text x="330" y="144" text-anchor="middle" font-weight="600" fill="currentColor">CDI</text>
  <text x="330" y="160" text-anchor="middle" font-size="11.5" fill="currentColor">capacitor: se carga</text>
  <text x="330" y="176" text-anchor="middle" font-size="11.5" fill="currentColor">tiristor: lo descarga</text>
  <rect x="455" y="128" width="150" height="56" rx="8" fill="none" stroke="#9a9a9a" stroke-width="1.25"/>
  <text x="530" y="152" text-anchor="middle" font-weight="600" fill="currentColor">Bobina de alta</text>
  <text x="530" y="168" text-anchor="middle" font-size="11.5" fill="currentColor" opacity=".7">10.000 a 20.000 V</text>
  <rect x="632" y="128" width="104" height="56" rx="8" fill="none" stroke="#9a9a9a" stroke-width="1.25"/>
  <text x="684" y="152" text-anchor="middle" font-weight="600" fill="currentColor">Bujía</text>
  <text x="684" y="168" text-anchor="middle" font-size="11.5" fill="currentColor" opacity=".7">chispa</text>
  <text x="232" y="88" font-size="11.5" fill="currentColor" opacity=".7">energía</text>
  <text x="232" y="232" font-size="11.5" fill="currentColor" opacity=".7">orden de disparo</text>
</svg>
<figcaption>Encendido con CDI de corriente continua. En el de corriente alterna, la caja "Batería" la reemplaza la bobina de baja del estator; el resto del camino es igual.</figcaption>
</figure>

## Qué se vio

- Alimentación: el CDI de corriente continua recibe 12 V de la batería al poner contacto, a través del fusible y la llave. El de corriente alterna se alimenta de la bobina de baja del estator, así que funciona aunque la batería esté muerta.
- Señal: cuando la "ventanita" del volante magnético pasa frente a la bobina captora, esta manda un pulso alterno al CDI.
- Dentro del CDI: un capacitor (se carga) y un tiristor (lo descarga al recibir el pulso) hacia la bobina de alta.
- Bobina de alta: eleva la tensión; sale por el cable y el capuchón a la bujía.
- Apagado: el corte (killer) o la llave sacan de servicio el CDI, según cómo esté cableado. Llave de contacto de cuatro cables.
- El avance de encendido puede venir programado en el CDI y cambia con las RPM.

## Datos que hay que saber

| Punto | Valor que se dio en clase |
| --- | --- |
| Alimentación del CDI (de continua) | 12 V de batería |
| Señal de la bobina captora al CDI | Más de 5 V, alterna |
| Salida de la bobina de alta | Del orden de 10.000 a 20.000 V |

- Diagnóstico, de lo simple a lo complejo: chispa en la bujía → capuchón y cable → 12 V y masa en el CDI → señal de la captora (más de 5 V) → bobina de alta (resistencia de primario y secundario contra manual) → recién al final el CDI.
- El pico de alta tensión no se mide con un tester común: hace falta un instrumento para picos.
- Los colores de cables cambian entre marcas, sobre todo en motos chinas: siempre el diagrama del fabricante.

## Preguntas para chequearte

1. Recorré el camino de la energía desde la batería hasta la chispa, pieza por pieza.
2. ¿Qué hacen el capacitor y el tiristor dentro del CDI?
3. ¿Qué diferencia hay entre un CDI de continua y uno de alterna? ¿Cuál arranca con la batería muerta?
4. ¿Cuánta tensión tiene que mandar la bobina captora para que funcione el CDI?
5. No hay chispa: ¿en qué orden revisás y por qué el CDI va al final?
