# Nébula Zero — prévia pública dos motores PS1 + PSP

Projeto experimental separado do APK Nébula Retro 0.2.x. A meta é criar motores autorais para PS1 e PSP, sem reutilizar código, cores ou interfaces de outros emuladores.

## Estado publicado nesta prévia

- **PS1:** parte da CPU MIPS R3000A/COP0; RAM/scratchpad parciais; leitor ISO-9660 que localiza SYSTEM.CNF/BOOT; carregador direto de PS-X EXE; GPU de software inicial com VRAM 1024×512, primitivas planas, amostragem de textura 4/8/15 bpp e transferência de pixels.
- **PSP:** primeira base Allegrex/MIPS com subconjunto de instruções, delay slots e exceções; leitor inicial que localiza e extrai PSP_GAME/SYSDIR/EBOOT.BIN de ISO-9660.
- **PSP ainda não inicia jogo:** EBOOT.BIN comercial normalmente exige descriptografia PRX, e isso, ELF/PRX loader, VFPU, GE, serviços de firmware, áudio e exibição ainda não estão implementados.
- **APK:** não há build Android jogável nesta prévia. A imagem do PS1 ainda não está ligada a uma tela Android; o PSP ainda não produz imagem.
- **Testes:** os testes foram escritos, mas ainda não executados neste ambiente.

## Próximos passos e limites

Ainda faltam a integração Android, barramentos completos, CD-ROM/UMD, DMA, temporização, áudio, GPU/GE completos, firmware HLE e testes reais. O objetivo é abrir imagens próprias de PS1 e PSP e desenhar os jogos na tela, mas compatibilidade universal não pode ser prometida. Esta prévia é apenas código, não um APK; não inclui jogos, ISOs, BIOS ou firmware.
