# PULSE: atualizações

Este repositório guarda só o instalador e as versões compiladas do PULSE (sampler para tocar ao vivo).
O código-fonte fica em outro repositório, que é privado.

## Instalar numa máquina nova

1. Baixe o instalador: **[PULSE-Setup.exe](https://github.com/Jhonatanariasgt/pulse-updates/releases/latest/download/PULSE-Setup.exe)** (0,9 GB, versão 1.2.5)
   (programa, sons, presets e manual — tudo num arquivo só).
2. Rode o instalador e clique em **Instalar**. Se aparecer "O Windows protegeu o computador", clique em
   **Mais informações** e depois em **Executar assim mesmo**. Não precisa de administrador.
3. Depois disso, o PULSE se atualiza sozinho (*Ajustes → Atualizações*).

## Como funciona

| Arquivo | Conteúdo | Quem usa |
|---|---|---|
| `PULSE-Setup.exe` (Releases) | programa + sons + presets + manual | instalação nova (ou reinstalar: o que já está igual é pulado) |
| `PULSE-app-<versão>.zip` (Releases) | só o programa | atualizador do app |
| pacotes de sons (Releases `pack-*`) | teclados (Essential Keys), bateria (99 Drum Pads), imagens dos pedais | atualizador do app: instala o que faltar em a pasta `PULSE/Sons` |
| `manifest.json` | versão atual, links e SHA-256 | atualizador do app |

Já tem o PULSE instalado mas sem os sons? Abra *Ajustes → Atualizações → Verificar* e clique em **Instalar**:
o PULSE baixa os pacotes de sons sozinho.

O atualizador só instala o que bater com o SHA-256 do `manifest.json`.
