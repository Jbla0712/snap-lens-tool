# 🛠️ Do It Yourself Instructions
Make sure to have an up-to-date version of **Python 3** installed.

## 🧩 Install Python Dependencies
Install project dependencies from `requirements.txt` with *pip*

```sh
pip install -r requirements.txt
```

## 🎨 Edit GUI (optional)

Make changes to `dialog.ui` with *Qt Designer*
```sh
qt5-tools designer dialog.ui
```

Convert xml design representation to python code
```sh
pyuic5 -x dialog.ui -o src/qt/dialog.py
```

## ‍👨‍💻 Build Binary

Install PyInstaller with *pip*
```sh
pip install pyinstaller
```

Create standalone binary with *PyInstaller*
```sh
pyinstaller --onedir --noconsole snap_lens_tool.py
```

Use `--onefile` instead of `--onedir` to output a single file.

The binary output files can be found under `./dist`.