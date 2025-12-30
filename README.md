🔥 Grinder

Grinder is the Great Rust Binder — a savage CLI that automatically generates PyO3 bindings for any Rust crate (local or crates.io). Zero boilerplate. Zero pain. You get .pyi type hints and Python wheels like magic. 🪄


---

🚀 Features

🧠 Automatically binds functions, structs, enums, constants — recursively

📦 Works with local crates and crates.io crates

🧾 Generates .pyi files for full Python type hints

🛞 Builds Python wheels (.whl) and can auto-install them

🧩 Default module name: py_<crate> (customizable)

⏩ Forward compatibility enabled by default

🤖 Fully automated — no manual wrappers needed

📁 Custom output folders for generated wheels



---

🧰 Installation

1️⃣ Build & install Grinder

After building with Hatch:

.\build.ps1

2️⃣ Install cargo-download (for online crates)

cargo install cargo-download


---

🕹️ Usage

📂 Local crate

grinder path/to/local/crate

Generates py_<crate_name>/ with a wheel

Generates <crate_name>.pyi in the crate root



---

🌐 Crate from crates.io

grinder regex -i

Downloads the crate from crates.io

Generates PyO3 bindings

Generates .pyi file

Builds a wheel

-i auto-installs the wheel 🚀



---

⚙️ Options

Option	Description

-i	Auto-install the generated wheel
--module-name <name>	Override default py_ module name
-fc	Enable forward compatibility (default)
--out <path>	Specify output folder for wheel
<crate>	Local path or crate name



---

🧪 Output Example

py_regex/
├── __init__.py
├── regex.pyi
└── py_regex-0.1.0-cp311-cp311-win_amd64.whl


---

🧠 Philosophy

Rust crate → Python module

No glue code. No tears. Just Grinder doing unholy levels of automation. 😈


---

🧯 Warning

This tool is powerful. If your crate is cursed, Grinder will still bind it. Use responsibly.


---

🔥 Grind Rust. Ship Python. Repeat.
