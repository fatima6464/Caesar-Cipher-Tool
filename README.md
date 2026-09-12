# 🔐 Caesar Cipher Tool

![HTML5](https://img.shields.io/badge/HTML5-orange.svg)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6-yellow.svg)
![Status](https://img.shields.io/badge/Status-Academic%20Project-brightgreen.svg)

An interactive, browser-based **Caesar Cipher** tool for encrypting and decrypting text messages with a custom shift key. Built as an **Information Security** course project to demonstrate one of the oldest classical encryption techniques in a hands-on, visual way.

---

## 📋 Overview

The Caesar Cipher is a substitution cipher where each letter in a message is shifted a fixed number of positions down the alphabet. This tool lets you type any message, choose a shift key, and instantly see the encrypted result — or reverse the process to decrypt it back.

## ✨ Features

- 🔒 **Encrypt** any message using a custom integer shift key
- 🔓 **Decrypt** the output back to the original message using the same key
- 🔤 **Letters-only shifting** — numbers, spaces, and symbols are left untouched
- 🔁 **Alphabet wraparound** — shifting past 'Z'/'z' correctly wraps back to 'A'/'a'
- 🔡 **Case-preserving** — uppercase and lowercase letters are shifted independently, preserving case
- 🧭 **Guided UI** — inline hints explain how the shift works (e.g. "A → D if key = 3")
- ✅ **Smart button state** — Decrypt is disabled until there's output to decrypt

## 🔐 How the Cipher Works

1. Each letter in the message is converted to its character code
2. The code is shifted forward (encryption) or backward (decryption) by the key value
3. If the shift goes past 'Z' or 'z', it wraps around to the start of the alphabet
4. The shifted code is converted back into a character
5. Non-letter characters (numbers, punctuation, spaces) are returned unchanged

**Example:** With key = `3`: `HELLO` → `KHOOR`

<img width="1917" height="917" alt="image" src="https://github.com/user-attachments/assets/165a1740-5cb0-43e0-80e8-fedfb8711af5" />


## 🛠️ Tech Stack

| Category | Details |
|---|---|
| Structure | HTML5 |
| Styling | Custom CSS (gradient background, card layout) |
| Logic | Vanilla JavaScript (ES6) |

## 📁 Project Structure

```
Caesar-Cipher-Tool/
├── index.html    # Full tool — UI, styling, and cipher logic in one file
└── README.md
```

## ▶️ How to Run

No build step, server, or dependencies required — everything runs client-side in the browser.

```bash
git clone https://github.com/<your-username>/Caesar-Cipher-Tool.git
cd Caesar-Cipher-Tool
open index.html
```

## 🌐 Try It Live

Since this is pure client-side HTML/CSS/JS, you can host it for free with **GitHub Pages**:
1. Repo → **Settings** → **Pages**
2. Source: `main` branch, root folder → Save
3. Visit `https://<your-username>.github.io/Caesar-Cipher-Tool/`

<img width="1917" height="908" alt="image" src="https://github.com/user-attachments/assets/8d856023-dbaa-421a-a413-ef7812aa0efa" />


## 🕹️ Usage

1. Type or paste your message into the **Enter Message** box
2. Enter a shift value in **Enter Key**
3. Click **Encrypt** to see the ciphered output
4. Click **Decrypt** to reverse it back to the original message using the same key

## 📚 What I Learned

- Implementing a classical substitution cipher algorithm from first principles (ASCII manipulation and modular arithmetic for wraparound)
- Handling case-sensitivity and non-alphabetic characters correctly in a cipher implementation
- Building simple, guided UI states (disabled buttons, inline hints) to make a cryptography concept approachable for a general user

## 🔮 Future Improvements

- Add a brute-force "crack the cipher" mode that tries all 25 possible shifts
- Frequency analysis visualization to demonstrate why Caesar Cipher is cryptographically weak
- Support for other classical ciphers (Vigenère, Atbash) for comparison

## 🎓 Course

Information Security — BS Computer Science

## 👩‍💻 Author

**Fatima Nadeem**
BS Computer Science

## 📎 Notes

- This is a classical/educational cipher, not suitable for real-world secure communication
- Tested in modern Chromium/Firefox browsers; no dependencies needed
