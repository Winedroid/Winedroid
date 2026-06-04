# 🍷 WineDroid

Roda programas Windows diretamente no Android via Termux + proot + XFCE + Wine + VNC.

## Install

```bash
cp winedroid $PREFIX/bin/winedroid
chmod +x $PREFIX/bin/winedroid
winedroid install
```

## Uso

```bash
winedroid install        # instala tudo (primeira vez, ~10-20 min)
winedroid start          # inicia o VNC
winedroid stop           # para o VNC
winedroid run app.exe    # roda um .exe
winedroid status         # status do ambiente
winedroid shell          # terminal Ubuntu
winedroid passwd 1234    # muda senha VNC
```

## Como acessar

1. Instale o app **AVNC** ou **VNC Viewer** no Android
2. Conecte em `127.0.0.1:5901`
3. Senha padrão: `donut123`

## O que é instalado

- **proot-distro** — Ubuntu 22.04 isolado
- **XFCE4** — desktop leve
- **TigerVNC** — servidor VNC
- **Wine** — roda .exe Windows
- **Winetricks** — instala runtimes (.NET, DirectX, etc.)

## Requisitos

- Termux atualizado
- ~3-5GB de espaço livre
- Android 7+
