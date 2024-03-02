### Install all extensions from the vs-extensions.txt

For Unix-like shells (Zsh and Bash):

```bash
cat vs-extensions.txt | xargs -L1 code --install-extension
```

For Windows Command Prompt (CMD):

```cmd
for /F "tokens=*" %a in (vs-extensions.txt) do code --install-extension %a
```

---

### List all installed extensions

For Unix-like shells (Zsh and Bash):

```bash
code --list-extensions | xargs -L 1 echo code --install-extension
```

For Windows Command Prompt (CMD):

```cmd
code --list-extensions | % { "code --install-extension $_" }
```

