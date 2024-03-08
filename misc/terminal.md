# Terminal
---

### Bash terminal, fancy git bar

[Installation](https://l.facebook.com/l.php?u=https%3A%2F%2Fwww.pragmaticlinux.com%2F2022%2F06%2Fshow-the-git-branch-in-your-bash-terminal-prompt%2F%3Ffbclid%3DIwAR3YUcIUbX7CZ9cIo7GwXWspqzdJdCQMGpaWDFHrIO3ajSUeAi-dQ5c1Xgs&h=AT29y_mLhKpNtETd5OXn2KM2wVX4uDj9-ySHzO6FnCqr-AVbclN246BQ9dcUSceNYjT70En3uHi1kc6Xu2dkcZXXZVDwyMPvp3h2-4ns9i1RU72hABR5kJj-T91YS4WBn_KwCBRyCQc)

#### Prerequisits

```
Debian/Ubuntu/Raspberry PI: `sudo apt install git curl`
Fedora: `sudo dnf install git curl`
openSUSE: `sudo zypper install git curl`
```

#### Install

1. Install fancygit

```bash
curl -sS https://raw.githubusercontent.com/diogocavilha/fancy-git/master/install.sh | bash
```

2. Apply suggested theme 

```bash
fancygit --suggested-global-git-config-apply
```

3. Change font to some nerd font (for example JetBrainsMono Nerd Font Mono)

4. Disable time (optional)

```bash
fancygit --disable-time
```