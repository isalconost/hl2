# 💻📖 hacker-laws

Laws, Theories, Principles and Patterns that developers will find useful.

[Translations](#translations): [🇮🇩](./translations/id.md) [🇧🇷](./translations/pt-BR.md) [🇨🇳](https://github.com/nusr/hacker-laws-zh) [🇩🇪](./translations/de.md) [🇫🇷](./translations/fr.md) [🇬🇷](./translations/el.md) [🇮🇹](https://github.com/csparpa/hacker-laws-it) [🇱🇻](./translations/lv.md) [🇰🇷](https://github.com/codeanddonuts/hacker-laws-kr) [🇵🇱](./translations/pl.md) [🇷🇺](https://github.com/solarrust/hacker-laws) [🇪🇸](./translations/es-ES.md) [🇹🇷](https://github.com/umutphp/hacker-laws-tr) [🇯🇵](./translations/jp.md) [🇺🇦](./translations/uk.md) [🇻🇳](./translations/vi.md)

Like this project? Please considering [sponsoring me](https://github.com/sponsors/dwmkerr) and the [translators](#translations). Also check out this podcast on [The Changelog - Laws for Hackers to Live By](https://changelog.com/podcast/403) to learn more about the project! You can also [download the latest PDF eBook](https://github.com/dwmkerr/hacker-laws/releases/latest/download/hacker-laws.pdf). Check the [Contributor Guide](./.github/contributing.md) if you are keen to contribute!

---

<!-- vim-markdown-toc GFM -->

* [Introduction](#introduction)
* [Laws](#laws)
    * [90–9–1 Principle (1% Rule)](#9091-principle-1-rule)
    * [Amdahl's Law](#amdahls-law)
    * [The Broken Windows Theory](#the-broken-windows-theory)
    * [Brooks' Law](#brooks-law)
    * [CAP Theorem (Brewer's Theorem)](#cap-theorem-brewers-theorem)
    * [Clarke's three laws](#clarkes-three-laws)
    * [Conway's Law](#conways-law)
    * [Cunningham's Law](#cunninghams-law)
    * [Dunbar's Number](#dunbars-number)
    * [The Dunning-Kruger Effect](#the-dunning-kruger-effect)
    * [Fitts' Law](#fitts-law)
    * [Gall's Law](#galls-law)
    * [Goodhart's Law](#goodharts-law)
    * [Hanlon's Razor](#hanlons-razor)
    * [Hick's Law (Hick-Hyman Law)](#hicks-law-hick-hyman-law)
    * [Hofstadter's Law](#hofstadters-law)
    * [Hutber's Law](#hutbers-law)
    * [The Hype Cycle & Amara's Law](#the-hype-cycle--amaras-law)
    * [Hyrum's Law (The Law of Implicit Interfaces)](#hyrums-law-the-law-of-implicit-interfaces)
    * [Kernighan's Law](#kernighans-law)
    * [Linus's Law](#linuss-law)
    * [Metcalfe's Law](#metcalfes-law)
    * [Moore's Law](#moores-law)
    * [Murphy's Law / Sod's Law](#murphys-law--sods-law)
    * [Occam's Razor](#occams-razor)
    * [Parkinson's Law](#parkinsons-law)
    * [Premature Optimization Effect](#premature-optimization-effect)
    * [Putt's Law](#putts-law)
    * [Reed's Law](#reeds-law)
    * [The Law of Conservation of Complexity (Tesler's Law)](#the-law-of-conservation-of-complexity-teslers-law)
    * [The Law of Demeter](#the-law-of-demeter)
    * [The Law of Leaky Abstractions](#the-law-of-leaky-abstractions)
    * [The Law of the Instrument](#the-law-of-the-instrument)
    * [The Law of Triviality](#the-law-of-triviality)
    * [The Unix Philosophy](#the-unix-philosophy)
    * [The Scout Rule](#the-scout-rule)
    * [The Spotify Model](#the-spotify-model)
    * [The Two Pizza Rule](#the-two-pizza-rule)
    * [Wadler's Law](#wadlers-law)
    * [Wheaton's Law](#wheatons-law)
* [Principles](#principles)
    * [All Models Are Wrong (George Box's Law)](#all-models-are-wrong-george-boxs-law)
    * [Chesterton's Fence](#chestertons-fence)
    * [The Dead Sea Effect](#the-dead-sea-effect)
    * [The Dilbert Principle](#the-dilbert-principle)
    * [The Pareto Principle (The 80/20 Rule)](#the-pareto-principle-the-8020-rule)
    * [The Shirky Principle](#the-shirky-principle)
    * [The Peter Principle](#the-peter-principle)
    * [The Robustness Principle (Postel's Law)](#the-robustness-principle-postels-law)
    * [SOLID](#solid)
    * [The Single Responsibility Principle](#the-single-responsibility-principle)
    * [The Open/Closed Principle](#the-openclosed-principle)
    * [The Liskov Substitution Principle](#the-liskov-substitution-principle)
    * [The Interface Segregation Principle](#the-interface-segregation-principle)
    * [The Dependency Inversion Principle](#the-dependency-inversion-principle)
    * [The DRY Principle](#the-dry-principle)
    * [The KISS principle](#the-kiss-principle)
    * [YAGNI](#yagni)
    * [The Fallacies of Distributed Computing](#the-fallacies-of-distributed-computing)
    * [The Principle of Least Astonishment](#the-principle-of-least-astonishment)
* [Reading List](#reading-list)
* [Online Resources](#online-resources)
* [PDF eBook](#pdf-ebook)
* [Podcast](#podcast)
* [Translations](#translations)
* [Related Projects](#related-projects)
* [Contributing](#contributing)
* [TODO](#todo)

<!-- vim-markdown-toc -->

## Introduction

There are lots of laws which people discuss when talking about development. This repository is a reference and overview of some of the most common ones. Please share and submit PRs!

❗: This repo contains an explanation of some laws, principles and patterns, but does not _advocate_ for any of them. Whether they should be applied will always be a matter of debate, and greatly dependent on what you are working on.

## Laws

And here we go!

Hello, I'm teh new paragraph!!! 

### 90–9–1 Principle (1% Rule)

[1% Rule on Wikipedia](https://en.wikipedia.org/wiki/1%25_rule_(Internet_culture))

The 90-9-1 principle suggests that within an internet community such as a wiki, 90% of participants only consume content, 9% edit or modify content and 1% of participants add content.

Real-world examples:

- A 2014 study of four digital health social networks found the top 1% created 73% of posts, the next 9% accounted for an average of ~25% and the remaining 90% accounted for an average of 2% ([Reference](https://www.jmir.org/2014/2/e33/))

See Also:

- [Pareto principle](#the-pareto-principle-the-8020-rule)

### Amdahl's Law

[Amdahl's Law on Wikipedia](https://en.wikipedia.org/wiki/Amdahl%27s_law)

> Amdahl's Law is a formula which shows the _potential speedup_ of a computational task which can be achieved by increasing the resources of a system. Normally used in parallel computing, it can predict the actual benefit of increasing the number of processors, which is limited by the parallelisability of the program.

Best illustrated with an example. If a program is made up of two parts, part A, which must be executed by a single processor, and part B, which can be parallelised, then we see that adding multiple processors to the system executing the program can only have a limited benefit. It can potentially greatly improve the speed of part B - but the speed of part A will remain unchanged.

The diagram below shows some examples of potential improvements in speed:

<img width="480px" alt="Diagram: Amdahl's Law" src="./images/amdahls_law.png" />

*(Image Reference: By Daniels219 at English Wikipedia, Creative Commons Attribution-Share Alike 3.0 Unported, https://en.wikipedia.org/wiki/File:AmdahlsLaw.svg)*

As can be seen, even a program which is 50% parallelisable will benefit very little beyond 10 processing units, whereas a program which is 95% parallelisable can still achieve significant speed improvements with over a thousand processing units.

As [Moore's Law](#moores-law) slows, and the acceleration of individual processor speed slows, parallelisation is key to improving performance. Graphics programming is an excellent example - with modern Shader based computing, individual pixels or fragments can be rendered in parallel - this is why modern graphics cards often have many thousands of processing cores (GPUs or Shader Units).

See also:

- [Brooks' Law](#brooks-law)
- [Moore's Law](#moores-law)

### The Broken Windows Theory

[The Broken Windows Theory on Wikipedia](https://en.wikipedia.org/wiki/Broken_windows_theory)

The Broken Windows Theory suggests that visible signs of crime (or lack of care of an environment) lead to further and more serious crimes (or further deterioration of the environment).

This theory has been applied to software development, suggesting that poor quality code (or [Technical Debt](#TODO)) can lead to a perception that efforts to improve quality may be ignored or undervalued, thus leading to further poor quality code. This effect cascades leading to a great decrease in quality over time.

See also:

- [Technical Debt](#TODO)

Examples:

- [The Pragmatic Programming: Software Entropy](https://flylib.com/books/en/1.315.1.15/1/)
- [Coding Horror: The Broken Window Theory](https://blog.codinghorror.com/the-broken-window-theory/)
- [OpenSource: Joy of Programming - The Broken Window Theory](https://opensourceforu.com/2011/05/joy-of-programming-broken-window-theory/)

