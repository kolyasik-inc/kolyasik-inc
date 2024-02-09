# Instalação Arch Linux

## Index

| Numero | Conteudos |
|---|---|
| 1 | [Pre-Configs da ISO](#is-00) |

---

##### is-00
# Pre-Configs da ISO

### **teclado**

_No caso de ser teclado brasileiro_ `loadkeys br-abnt2`

_No caso de teclado americano_ `loadkeys us-acentos`

```bash
localectl list-keymaps | less
loadkeys us
```

### **relogio**

```bash
# sincronizar relogio
timedatectl set-ntp true
# acertar manualmente o relogio
date -s '2014-12-25 12:34:56'
```

---

##### pt-00
# Particionamento e Subvolumes

## **Particionamento**

### **Primeiro Metodo**

```bash
# Limpeza do disco substitua /sdX ou /mapper/VolumeLogico
sudo wipefs --all --force /dev/sdX

cfdisk /dev/sda
# select disk label "dos"
# create partition "sdX1"  size "8gb" type " linux swap / solaris"
# create partition "sdX2" size remaining space with type "linux"
# and "write"

mkfs.ext4 /dev/sda2
```

~Fim.~

---
