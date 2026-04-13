# AGENTS.md — awesome-galicia

## Propósito

Selección de software open source que da **soporte específico a Galicia** — su gobierno autonómico (Xunta de Galicia), concellos, universidades, empresas, infraestructuras y patrimonio. Todo el contenido en español. El foco es Galicia: el software debe dirigirse específicamente a esta comunidad autónoma o a sus municipios.

## Ámbito

- **4 provincias**: A Coruña, Lugo, Ourense, Pontevedra.
- Principales ciudades: Santiago de Compostela (capital), A Coruña, Vigo, Ourense, Lugo, Pontevedra, Ferrol, Santiago de Compostela.
- **Universidades**: USC (Universidade de Santiago de Compostela), UVigo (Universidade de Vigo), UDC (Universidade da Coruña).
- **Instituciones**: Xunta de Galicia, AMTEGA (Axencia para a Modernización Tecnolóxica de Galicia), IGE (Instituto Galego de Estatística), MeteoGalicia, SERGAS (Servizo Galego de Saúde), IET (Instituto de Estudos do Territorio).

## Criterios de inclusión

### Incluir

- Software que interactúa con la **Xunta de Galicia** o sus organismos (Sede Electrónica, Portal de Transparencia, datos abiertos).
- Herramientas para **concellos** de Galicia.
- Software de **universidades gallegas** (USC, UVigo, UDC) cuando sea específico de la región o la universidad.
- Herramientas de **datos abiertos** de Galicia (abert.os, IGE).
- Software relacionado con **MeteoGalicia** (meteorología, mareas, predicciones).
- Herramientas de **lengua gallega** (NLP, traductores, correctores, corpus).
- Software de **transporte** gallego (autobuses urbanos, Renfe Galicia, puertos).
- Herramientas de **cartografía y SIG** específicas de Galicia (IDE Galicia, IET).
- Software sobre **patrimonio y cultura** gallega (Camino de Santiago, patrimonio histórico).
- Herramientas de **turismo** de la región.
- Software de **pesca y mar** gallego.
- Proyectos del **sistema sanitario gallego** (SERGAS).
- Software **educativo** específico de la región.
- Herramientas de **medio ambiente** gallego.

### No incluir

- Software **genérico** que funciona en toda España sin funcionalidad específica de Galicia — eso pertenece a awesome-spain.
- Software de **ámbito europeo** — eso pertenece a awesome-europe.
- Software de **otras comunidades autónomas** españolas.
- Software creado por gallegos que **no tiene funcionalidad específica** de la región.
- Repositorios **archivados o de solo lectura** — van a `DELETED.md`.
- Repos donde el autor indica que el proyecto está **roto, sin mantenimiento o deprecado**.
- Repos **sin README significativo** o que son claramente repos de test/experimento.
- Ejercicios de clase o trabajos académicos sin utilidad real.

### Zona gris — usar criterio

- Proyectos de universidades gallegas que podrían ser genéricos — incluir si tienen datos o configuración específica de Galicia.
- Software que cubre Galicia junto con otras regiones — incluir si Galicia es un foco principal.
- Proyectos del CiTIUS (USC) que son herramientas genéricas de investigación — incluir solo si tienen soporte específico para gallego o datos gallegos.

## Estándares de calidad

**Mismo listón que [awesome-spain](https://github.com/GeiserX/awesome-spain):**

- **No repos archivados**: si se descubre archivado tras la inclusión, mover a `DELETED.md` inmediatamente.
- **No repos extremadamente sin mantenimiento**: al menos un commit en los últimos 3 años, salvo que sea un proyecto claramente estable/completo.
- **No repos rotos**: si el README dice «deprecated», «no longer maintained», «use X instead» o similar — no incluir. Mover a `DELETED.md` si ya está listado.
- **Estrellas mínimas**: preferir repos con al menos unas pocas estrellas, pero herramientas nicho excepcionales con 0-1 estrellas pueden incluirse si cubren un hueco importante.
- **Verificar cada repo** antes de añadir: comprobar `archived`, `pushed_at`, `stargazers_count` vía `gh api repos/owner/name`.

## Formato de entrada

```markdown
- [Nombre](https://github.com/owner/repo) [![Stars](...)](stargazers) [![Last Commit](...)](commits) [![Language](...)](repo) [![License](...)](LICENSE) [![Tag](...)](url) - Descripción que empieza en mayúscula y termina con punto.
```

Las insignias se generan automáticamente con `scripts/transform-readme.py`. Para contribuir, basta con añadir la entrada en formato simple:

```markdown
- [Nombre](https://github.com/owner/repo) - Descripción que empieza en mayúscula y termina con punto.
```

- La descripción **no debe empezar con el nombre** del proyecto.
- Máximo una línea por entrada.
- Validar con awesome-lint-extra: `python3 lint.py` o mediante el workflow de CI.
- Entradas en **orden alfabético** dentro de cada categoría.
- Categorías en **orden alfabético** en el índice y en el cuerpo del documento.
- Entradas en `DELETED.md` también en **orden alfabético** dentro de cada sección.

## Verificación antes de añadir

Antes de incluir un repositorio, comprobar:

- **Existe y es público**: el enlace de GitHub funciona y el repo no es privado.
- **No está archivado o de solo lectura**: si archivado, va a `DELETED.md` (sección «Archivados»).
- **No está deprecado**: comprobar si el README dice «deprecated», «unmaintained», «broken», «use X instead».
- **Actividad razonable**: al menos un commit en los últimos 3 años, salvo que sea un proyecto estable/completo.
- **No es un duplicado**: cruzar con `README.md` y `DELETED.md`.
- **Calidad mínima**: tiene documentación (README) y no es un repositorio vacío o de test.

## Pull requests y contribuciones

- Las PRs deben usar la plantilla en `.github/PULL_REQUEST_TEMPLATE.md`.
- **Obligatorio**: incluir en la PR la **URL del servicio, API o institución gallega** a la que el software da soporte.
- Plantillas de issues disponibles para sugerir proyectos (`anadir-proyecto.md`) y solicitar retirada (`retirar-proyecto.md`).

## Estructura

- Secciones con `##`, subsecciones con `###`.
- Índice de contenido al principio entre comentarios `<!--lint disable/enable awesome-list-item-->`.
- Al final: sección Contribuir, Nota y Descargo de responsabilidad (como párrafos en negrita, no encabezados ##).

## Temas prohibidos

No se aceptan proyectos relacionados con: pornografía, contenido NSFW, loterías o apuestas, religión, política partidista.

## Difusión

- Notificar a los propietarios de repos abriendo un issue titulado «Listado en awesome-galicia» con un breve mensaje en español (tuteo) ofreciendo retirar si lo prefieren. Solo 1 issue por organización/usuario — no spamear repos del mismo propietario.
- Publicar en comunidades gallegas (Reddit, foros de la USC/UVigo/UDC, Telegram de devs gallegos) tras alcanzar masa crítica.
- Enviar PR a [sindresorhus/awesome](https://github.com/sindresorhus/awesome) tras 30 días desde la creación del repo.

## Aprendizajes

- La Xunta tiene la organización `IET-Xunta` con repos de visores geográficos (XVM, DHGC, CDIX, SINA) — antiguos pero funcionales.
- No existe organización `amtega-pdi` en GitHub (404). La AMTEGA no tiene presencia pública significativa en GitHub.
- El `concello-santiago-de-compostela` tiene repos útiles: portal-datos-abertos, consul, ckan-gl, migasfree.
- El CiTIUS (USC) tiene muchos repos de investigación genérica — solo incluir los que tienen soporte específico para gallego (Linguakit, SimpleNLG-GL, DepPattern, explorador-diacronico).
- `David-Lor` mantiene VigoBusAPI y VigoBus-TelegramBot, ambos activos y con buena calidad.
- MeteoGalicia tiene varios wrappers y clientes (homeassistant-meteogalicia con 16★ es el más popular).
- `crpih/xiada` es el tagger/lemmatizer para gallego del CRPIH (Centro Ramón Piñeiro), activo en 2026.
- `xavier-gz/SLI_Galician_Corpora` son corpus lingüísticos del SLI (Seminario de Lingüística Informática) de la UVigo.
- La mayoría de repos con "Santiago de Compostela" son ejercicios de clase — filtrar con criterio.

*Generated by [LynxPrompt](https://lynxprompt.com) CLI*
