# Nébula Zero — prévia pública de desenvolvimento

Este é um projeto experimental separado do APK Nébula Retro 0.2.x. A meta é criar motores autorais para PS1 e PSP, sem reutilizar código, cores ou interfaces de outros emuladores.

## Estado publicado nesta prévia

- **PS1:** base própria em Kotlin para parte da CPU MIPS R3000A e COP0, mapa parcial de RAM, leitor ISO-9660 de setor de dados de 2048 bytes, extração de SYSTEM.CNF/BOOT, carregador direto de PS-X EXE e GPU de software inicial (VRAM 1024×512, upload/cópia de pixels, primitivas planas e amostragem básica de texturas).
- **PSP:** ainda não iniciado.
- **APK:** ainda não existe build Android jogável nesta prévia. O código não abre jogos comerciais e a imagem ainda não está ligada a uma tela Android.
- **Testes:** arquivos de teste foram escritos, mas não foram executados neste ambiente.

## O que ainda falta

O protótipo precisa de mais instruções/exceções de CPU, serviços HLE de BIOS, emulação de CD-ROM e DMA, GPU completa com transparência e temporização, áudio/SPU, entrada, integração Android e testes em jogos. Depois de validar a base PS1, o motor PSP será uma etapa separada. Compatibilidade com todos os jogos não pode ser prometida.

Este arquivo é uma prévia do código, não um APK. Não inclui ISOs, jogos, BIOS ou firmware.
