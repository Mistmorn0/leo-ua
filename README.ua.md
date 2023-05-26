<p align="center">
    <img width="1412" src="https://cdn.aleo.org/leo/banner.png">
</p>

<h1 align="center">Мова програмування Leo</h1>

<p align="center">
    <a href="https://circleci.com/gh/AleoHQ/leo"><img src="https://circleci.com/gh/AleoHQ/leo.svg?style=svg&circle-token=6e9ad6d39d95350544f352d34e0e5c62ef54db26"></a>
    <a href="https://codecov.io/gh/AleoHQ/leo"><img src="https://codecov.io/gh/AleoHQ/leo/branch/testnet3/graph/badge.svg?token=S6MWO60SYL"/></a>
    <a href="https://discord.gg/5v2ynrw2ds"><img src="https://img.shields.io/discord/700454073459015690?logo=discord"/></a>
</p>

Leo - це функціональна, статично типізована мова програмування, створена для написання приватних додатків.

## <a name='TableofContents'></a>Зміст

* [1. Огляд](#1-огляд)
* [2. Посібник зі збірки](#2-посібник-зі-збірки)
    * [2.1 Інсталяція Rust](#21-інсталяція-Rust)
    * [2.2 Збірка з вихідного коду](#22-збірка-з-вихідного-коду)
* [3. Швидкий старт](#3-швидкий-старт)
* [4. Вирішення проблем](#4-вирішення-проблем)
* [5. Документація](#5-документація)
* [6. Внесок](#6-внесок)
* [7. Ліцензія](#7-ліцензія)


## 1. Огляд

Ласкаво просимо до мови програмування Leo.


Leo надає високорівневу мову, яка абстрагується від низькорівневих криптографічних концепцій і дозволяє легко 
інтегрувати приватні додатки у ваш стек. Leo компілюється у схеми, що робить доведення з нульовим знанням практичним.

На синтаксис Leo вплинули традиційні мови програмування, такі як JavaScript, Scala та Rust, з сильним акцентом на читабельність та простоту використання.
Leo пропонує розробникам інструменти для перевірки правильності схем, включаючи модульні тести, інтеграційні тести та консольні функції.

Leo є частиною великої екосистеми для створення приватних додатків на [Aleo](https://aleo.org/). 
Наразі мова перебуває на стадії альфа-версії і може зазнавати суттєвих змін.

## 2. Посібник зі збірки

### 2.1 Інсталяція Rust

Ми рекомендуємо встановлювати Rust, використовуючи [rustup](https://www.rustup.rs/). Ви можете встановити `rustup` наступним чином:

- macOS або Linux:
  ```bash
  curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
  ```

- Windows (64-біт):

  Завантажте [Windows 64-bit executable](https://win.rustup.rs/x86_64) та дотримуйтесь інструкцій на екрані.

- Windows (32-біт):  
  
  Завантажте [Windows 32-bit executable](https://win.rustup.rs/i686) та дотримуйтесь інструкцій на екрані.

### 2.2 Збірка з вихідного коду

Ми рекомендуємо встановити Leo, зібравши з вихідного коду, як показано нижче:

```bash
# Завантажте вихідний код
git clone https://github.com/AleoHQ/leo
cd leo

# Встановіть 'leo'
$ cargo install --path .
```

Тепер, щоб використовувати leo, в терміналі запустіть:
```bash
leo
```

## 3. Швидкий старт

Використовуйте CLI Leo для створення нового проекту

```bash
# створити новий проект Leo 'hello-world'
leo new helloworld
cd helloworld

# збірка & налаштування & доказ & верифікація
leo run
```

Команда `leo new` створює новий проект Leo з заданим іменем.

Команда `leo run` компілює програму в інструкції Aleo та запускає її.

Вітаємо! Ви щойно запустили свою першу програму Leo.

## 4. Вирішення проблем
Якщо у вас виникли проблеми з встановленням та використанням Leo, будь ласа, ознайомтеся з нашим [посібником](docs/troubleshooting.md).

Якщо проблема все ще існує, будь ласа, [повідомте про проблему](https://github.com/AleoHQ/leo/issues/new/choose).

## 5. Документація

* [Hello World - Наступні кроки](https://developer.aleo.org/leo/hello)
* [Документація мови Leo](https://developer.aleo.org/leo/language)
* [Граматика Leo ABNF](./docs/grammar/abnf-grammar.txt)
* [Головна сторінка](https://developer.aleo.org/overview/)

## 6. Внесок
 
Будь ласа, дивіться наші рекомендації у [документації для розробників](./CONTRIBUTING.md)

Дякуємо, що допомагаєте зробити Leo кращим!

## 7. Ліцензія 
[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](./LICENSE.md)
