# Instalação Arch Linux

## Index

| Numero | Conteudos |
|---|---|
| 1 | [Pre-Configs da ISO](#is-00) |

---

##### is-00
## Pre-Configs da ISO

### teclado

No caso de ser teclado brasileiro $ `loadkeys br-abnt2`
No caso de teclado americano `loadkeys us-acentos`

```bash
localectl list-keymaps | less
loadkeys us
```

## relogio

### sincronizar relogio

```bash
timedatectl set-ntp true
```

### acertar manualmente o relogio

```bash
date -s '2014-12-25 12:34:56'
```
