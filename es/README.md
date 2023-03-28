# 💻📖 hacker-laws

Leyes, teorías, principios y patrones que los desarrolladores encontrarán útiles.

[Traducciones](#translations) [de](./translations/pt-BR.md) [:](./translations/id.md) [_](https://github.com/nusr/hacker-laws-zh) [_](./translations/de.md) [_](./translations/fr.md) [_](./translations/el.md) [_](https://github.com/csparpa/hacker-laws-it) [_](./translations/lv.md) [_](https://github.com/codeanddonuts/hacker-laws-kr) [_](./translations/pl.md) [_](https://github.com/solarrust/hacker-laws) [_](./translations/es-ES.md) [_](https://github.com/umutphp/hacker-laws-tr) [_](./translations/jp.md) [_](./translations/uk.md) [_](./translations/vi.md)

¿Te gusta este proyecto? Por favor, considere [patrocinarme a mí](https://github.com/sponsors/dwmkerr) ya los [traductores](#translations) . ¡Consulte también este podcast en [The Changelog - Laws for Hackers to Live By](https://changelog.com/podcast/403) para obtener más información sobre el proyecto! También puede [descargar el último libro electrónico en PDF](https://github.com/dwmkerr/hacker-laws/releases/latest/download/hacker-laws.pdf) . ¡Consulte la [Guía del colaborador](./.github/contributing.md) si está interesado en contribuir!

---

<!-- vim-markdown-toc GFM -->

- [Introducción](#introduction)
- [leyes](#laws)
    - [Principio 90–9–1 (Regla del 1%)](#9091-principle-1-rule)
    - [Ley de Amdahl](#amdahls-law)
    - [La teoría de las ventanas rotas](#the-broken-windows-theory)
    - [Ley de Brooks](#brooks-law)
    - [Teorema CAP (Teorema de Brewer)](#cap-theorem-brewers-theorem)
    - [Las tres leyes de Clarke](#clarkes-three-laws)
    - [Ley de Conway](#conways-law)
    - [Ley de Cunningham](#cunninghams-law)
    - [Número de Dunbar](#dunbars-number)
    - [El efecto Dunning-Kruger](#the-dunning-kruger-effect)
    - [Ley de Fitts](#fitts-law)
    - [Ley de Gall](#galls-law)
    - [Ley de Goodhart](#goodharts-law)
    - [Navaja de Hanlon](#hanlons-razor)
    - [Ley de Hick (Ley de Hick-Hyman)](#hicks-law-hick-hyman-law)
    - [Ley de Hofstadter](#hofstadters-law)
    - [Ley de Hutber](#hutbers-law)
    - [El Ciclo del Hype y la Ley de Amara](#the-hype-cycle--amaras-law)
    - [Ley de Hyrum (La ley de las interfaces implícitas)](#hyrums-law-the-law-of-implicit-interfaces)
    - [Ley de Kernighan](#kernighans-law)
    - [Ley de Linus](#linuss-law)
    - [Ley de Metcalfe](#metcalfes-law)
    - [Ley de Moore](#moores-law)
    - [Ley de Murphy / Ley de Sod](#murphys-law--sods-law)
    - [La navaja de Occam](#occams-razor)
    - [Ley de Parkinson](#parkinsons-law)
    - [Efecto de optimización prematuro](#premature-optimization-effect)
    - [ley de putt](#putts-law)
    - [Ley de Reed](#reeds-law)
    - [La Ley de Conservación de la Complejidad (Ley de Tesler)](#the-law-of-conservation-of-complexity-teslers-law)
    - [La ley de Deméter](#the-law-of-demeter)
    - [La ley de las abstracciones con fugas](#the-law-of-leaky-abstractions)
    - [La Ley del Instrumento](#the-law-of-the-instrument)
    - [La ley de la trivialidad](#the-law-of-triviality)
    - [La Filosofía Unix](#the-unix-philosophy)
    - [La Regla Scout](#the-scout-rule)
    - [El modelo de Spotify](#the-spotify-model)
    - [La regla de las dos pizzas](#the-two-pizza-rule)
    - [Ley de Wadler](#wadlers-law)
    - [Ley de Wheaton](#wheatons-law)
- [Principios](#principles)
    - [Todos los modelos son incorrectos (Ley de George Box)](#all-models-are-wrong-george-boxs-law)
    - [Valla de Chesterton](#chestertons-fence)
    - [El efecto del Mar Muerto](#the-dead-sea-effect)
    - [El principio de Dilbert](#the-dilbert-principle)
    - [El Principio de Pareto (La Regla 80/20)](#the-pareto-principle-the-8020-rule)
    - [El principio de Shirky](#the-shirky-principle)
    - [El principio de Peter](#the-peter-principle)
    - [El Principio de Robustez (Ley de Postel)](#the-robustness-principle-postels-law)
    - [SÓLIDO](#solid)
    - [El principio de responsabilidad única](#the-single-responsibility-principle)
    - [El principio abierto/cerrado](#the-openclosed-principle)
    - [El principio de sustitución de Liskov](#the-liskov-substitution-principle)
    - [El principio de segregación de la interfaz](#the-interface-segregation-principle)
    - [El principio de inversión de dependencia](#the-dependency-inversion-principle)
    - [El principio SECO](#the-dry-principle)
    - [El principio KISS](#the-kiss-principle)
    - [YAGNI](#yagni)
    - [Las falacias de la computación distribuida](#the-fallacies-of-distributed-computing)
    - [El principio del menor asombro](#the-principle-of-least-astonishment)
- [Leyendo lista](#reading-list)
- [Recursos en línea](#online-resources)
- [Libro electrónico PDF](#pdf-ebook)
- [Podcast](#podcast)
- [Traducciones](#translations)
- [Proyectos relacionados](#related-projects)
- [contribuyendo](#contributing)
- [HACER](#todo)

<!-- vim-markdown-toc -->

## Introducción

Hay muchas leyes de las que la gente habla cuando habla de desarrollo. Este repositorio es una referencia y una descripción general de algunos de los más comunes. ¡Por favor comparta y envíe PRs!

❗: Este repositorio contiene una explicación de algunas leyes, principios y patrones, pero no *aboga* por ninguno de ellos. Si deben aplicarse siempre será un tema de debate y dependerá en gran medida de en qué esté trabajando.

## leyes

¡Y aquí vamos!

### Principio 90–9–1 (Regla del 1%)

[Regla del 1% en Wikipedia](https://en.wikipedia.org/wiki/1%25_rule_(Internet_culture))

El principio 90-9-1 sugiere que dentro de una comunidad de Internet como una wiki, el 90% de los participantes solo consume contenido, el 9% edita o modifica contenido y el 1% de los participantes agrega contenido.

Ejemplos del mundo real:

- Un estudio de 2014 de cuatro redes sociales de salud digital encontró que el 1% superior creó el 73% de las publicaciones, el siguiente 9% representó un promedio de ~25% y el 90% restante representó un promedio del 2% ( [Referencia](https://www.jmir.org/2014/2/e33/) )

Ver también:

- [Principio de Pareto](#the-pareto-principle-the-8020-rule)

### Ley de Amdahl

[Ley de Amdahl en Wikipedia](https://en.wikipedia.org/wiki/Amdahl%27s_law)

> La Ley de Amdahl es una fórmula que muestra la *aceleración potencial* de una tarea computacional que se puede lograr aumentando los recursos de un sistema. Normalmente utilizado en computación paralela, puede predecir el beneficio real de aumentar el número de procesadores, que está limitado por la paralelización del programa.

Se ilustra mejor con un ejemplo. Si un programa se compone de dos partes, la parte A, que debe ser ejecutada por un solo procesador, y la parte B, que se puede paralelizar, entonces vemos que agregar múltiples procesadores al sistema que ejecuta el programa solo puede tener un beneficio limitado. . Potencialmente, puede mejorar en gran medida la velocidad de la parte B, pero la velocidad de la parte A permanecerá sin cambios.

El siguiente diagrama muestra algunos ejemplos de posibles mejoras en la velocidad:

<img width="480px" alt="Diagrama: Ley de Amdahl" src="./images/amdahls_law.png">

*(Referencia de la imagen: por Daniels219 en Wikipedia en inglés, Creative Commons Attribution-Share Alike 3.0 Unported, https://en.wikipedia.org/wiki/File:AmdahlsLaw.svg)*

Como se puede ver, incluso un programa que es 50% paralelizable se beneficiará muy poco más allá de 10 unidades de procesamiento, mientras que un programa que es 95% paralelizable aún puede lograr mejoras de velocidad significativas con más de mil unidades de procesamiento.

A medida que [la Ley de Moore](#moores-law) se ralentiza y la aceleración de la velocidad del procesador individual se ralentiza, la paralelización es clave para mejorar el rendimiento. La programación de gráficos es un excelente ejemplo: con la computación moderna basada en Shader, los píxeles o fragmentos individuales se pueden representar en paralelo; esta es la razón por la que las tarjetas gráficas modernas suelen tener muchos miles de núcleos de procesamiento (GPU o Unidades Shader).

Ver también:

- [Ley de Brooks](#brooks-law)
- [Ley de Moore](#moores-law)

### La teoría de las ventanas rotas

[La teoría de las ventanas rotas en Wikipedia](https://en.wikipedia.org/wiki/Broken_windows_theory)

La Teoría de las Ventanas Rotas sugiere que los signos visibles de delincuencia (o la falta de cuidado del medio ambiente) conducen a más delitos y más graves (oa un mayor deterioro del medio ambiente).

Esta teoría se ha aplicado al desarrollo de software, lo que sugiere que el código de mala calidad (o [deuda técnica](#TODO) ) puede llevar a la percepción de que los esfuerzos para mejorar la calidad pueden ignorarse o subestimarse, lo que lleva a un código de mala calidad adicional. Este efecto cae en cascada y conduce a una gran disminución de la calidad con el tiempo.

Ver también:

- [Deuda técnica](#TODO)

Ejemplos:

- [La programación pragmática: la entropía del software](https://flylib.com/books/en/1.315.1.15/1/)
- [Coding Horror: La teoría de la ventana rota](https://blog.codinghorror.com/the-broken-window-theory/)
- [Código abierto: el placer de programar: la teoría de la ventana rota](https://opensourceforu.com/2011/05/joy-of-programming-broken-window-theory/)
