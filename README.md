# Nébula Retro — PSP + PS1

Frontend Android próprio, com telas e fluxo de biblioteca originais em Kotlin. Não é o app Lemuroid. A emulação é feita pelos projetos open-source PPSSPP (PSP) e PCSX-ReARMed (PS1), integrados pela biblioteca LibretroDroid — os motores não foram reimplementados do zero.

## Baixar

- [Lançamento Nébula Retro v0.2.0](https://github.com/raullygomesbarbosa2-lgtm/retrobox-android/releases/tag/v0.2.0)
- [Baixar APK v0.2.0 diretamente](https://github.com/raullygomesbarbosa2-lgtm/retrobox-android/releases/download/v0.2.0/Nebula-Retro-v0.2.0.apk)
- [Código-fonte do frontend](https://github.com/raullygomesbarbosa2-lgtm/retrobox-android/releases/download/v0.2.0/Nebula-Retro-source-v0.2.0.zip)

## Como usar

1. Escolha uma pasta separada para jogos de PS1 e outra para PSP.
2. Toque em **Atualizar biblioteca**; o app examina as pastas selecionadas e suas subpastas.
3. Toque em um jogo para iniciar. A jogabilidade abre em paisagem com controles táteis.

## Núcleos, BIOS e compatibilidade

- **PSP:** núcleo PPSSPP, que pode usar HLE sem BIOS de PSP. Na primeira abertura de um jogo PSP, o app precisa de internet para baixar arquivos auxiliares do PPSSPP; eles não são BIOS nem jogos.
- **PS1:** núcleo PCSX-ReARMed pode usar HLE sem BIOS de PS1, mas a compatibilidade varia e alguns jogos podem não iniciar corretamente.
- Nenhum jogo, imagem de disco, BIOS ou firmware proprietário acompanha o app.
- Desempenho varia por aparelho, jogo e configurações; não há garantia de 30 FPS em todos os celulares.

## Compatibilidade de aparelhos

O APK inclui as ABIs `arm64-v8a`, `armeabi-v7a` e `x86`. Aparelhos que só aceitam `x86_64` não são compatíveis com esta compilação. `minSdk` é 23 (Android 6.0).

## Código e licenças

O projeto contém o frontend Android próprio e integra bibliotecas/núcleos GPL de terceiros. Consulte `COPYING` e `SOURCE_LICENSES.md` no arquivo-fonte; os núcleos são obtidos do repositório público [LemuroidCores](https://github.com/Swordfish90/LemuroidCores), fixado no commit `fee2e824525daa22bcf318f96127fe43fa8a15ad`. Veja também [PPSSPP](https://github.com/hrydgard/ppsspp), [PCSX-ReARMed](https://github.com/libretro/pcsx_rearmed) e [LibretroDroid](https://github.com/Swordfish90/LibretroDroid).

O build e a verificação do APK são feitos por GitHub Actions. A compilação não substitui testes de gameplay ou instalação em cada aparelho.
