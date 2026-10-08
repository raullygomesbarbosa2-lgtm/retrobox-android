# Nébula Zero — prévia pública PS1 + PSP

Projeto experimental independente do Nébula Retro 0.2.x. Os motores são implementações originais deste projeto; não incorporam núcleos, código ou interfaces de outros emuladores.

## Esta é uma prévia técnica, não um emulador jogável

O app Android pode desenhar um padrão de teste da GPU de software própria do PS1 e examinar ISOs selecionadas. No PS1, localiza SYSTEM.CNF/BOOT e PS-X EXE, mas não inicia jogos. No PSP, extrai EBOOT.BIN, mas não carrega EBOOT/PRX comerciais criptografados. **Não roda jogos comerciais.**

## Estado dos motores

- **PS1:** implementação parcial própria de MIPS R3000A/COP0, RAM/scratchpad, loader PS-X EXE, leitor ISO-9660 e GPU 2D/3D inicial com primitivas/texturas e barramento GP0/GP1 básico. Ainda faltam HLE de BIOS, CD-ROM completo, áudio, temporização e renderizador Android de jogos.
- **PSP:** implementação parcial própria de Allegrex/MIPS, RAM/EDRAM, leitor ISO-9660 e loader de ELF32 não criptografado. Ainda faltam descriptografia e carregamento de PRX, VFPU, GE, HLE de firmware, áudio e gameplay.
- Não acompanha BIOS, firmware, jogos ou ISOs.

## Build

O workflow do GitHub Actions executa os testes de PS1/PSP e compila o APK debug do app Android. Os testes dos núcleos passaram no run #4. A primeira tentativa do build Android apontou uma configuração ausente do repositório Google Maven; ela foi corrigida e a nova execução precisa terminar com sucesso antes de haver um APK para baixar.
