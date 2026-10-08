# Nébula Retro — PSP + PS1

App Android derivado do frontend de código aberto Lemuroid, personalizado para **PlayStation Portable (PSP)** e **PlayStation original (PS1)**. Não inclui CHIP-8, jogos, ISOs, BIOS ou firmware.

## Como usar

1. Escolha uma pasta da biblioteca no aparelho.
2. Separe os arquivos em pastas `PSP` e `PS1`, porque os dois consoles usam arquivos `.iso`.
3. Depois que a biblioteca for examinada, toque no jogo para iniciá-lo. Durante o jogo, o app usa a tela horizontal e os controles táteis do console.

## Núcleos e BIOS

- PSP: núcleo PPSSPP com HLE; não exige BIOS externa.
- PS1: núcleo PCSX-ReARMed pode recorrer a HLE sem BIOS; a compatibilidade varia e alguns jogos podem não iniciar corretamente.
- O núcleo PPSSPP pode baixar assets auxiliares ao primeiro uso; isso não é BIOS nem jogo.

30 FPS é uma meta, não uma garantia para todos os celulares. O desempenho depende do aparelho, do jogo e das configurações.

## Código e licenças

O app é baseado no [Lemuroid](https://github.com/Swordfish90/Lemuroid), sob GPLv3. O projeto inclui `COPYING`, avisos e instruções de build; os núcleos vêm da distribuição pública [LemuroidCores](https://github.com/Swordfish90/LemuroidCores) no commit fixado no código.

- [PPSSPP](https://github.com/hrydgard/ppsspp)
- [PCSX-ReARMed](https://github.com/libretro/pcsx_rearmed) · [documentação sobre HLE](https://docs.libretro.com/library/pcsx_rearmed/)

O APK é compilado pelo workflow **Build Nébula Retro 0.1.3** em GitHub Actions. A versão CHIP-8 anterior não executa jogos PSP/PS1.
