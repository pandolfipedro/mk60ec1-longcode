# Definições dos presets

Autoria do aplicativo: Pedro Pandolfi. As escolhas abaixo são bases editáveis, não uma afirmação de coding de fábrica.

| Campo | Jetta 2.5 | Jetta TSI | Fusca TSI |
|---|---|---|---|
| VIN plataforma | 1K | 16 / AJ | 16 / AT |
| Byte 0 inicial | 11 | A4 (multilink), B4 (torção) | F4 (multilink), E4 (torção) |
| Byte 2 inicial | 40 | 60 | 60 |
| Byte 4 inicial | 0A | 09 | 09 |
| Byte 6 inicial | 00 | 00 | 00 |
| Byte 15 inicial | 41 | 41 | 41 |
| Byte 16 em 18/19 bytes | 30 | 30 | 30 |
| Byte 16 em H46 | 20 | 20 | 20 |
| Byte 17 / 18 inicial | 00 / 00, se presentes | 00 / 00, se presentes | 00 / 00, se presentes |
| Byte 19 inicial | 20, se presente | 20, se presente | 20, se presente |

O VIN preenche somente bytes 1, 3, 5, 7, 9, 11 e 13. Os pares espelhados são 0→8, 2→10, 4→12 e 6→14.

A família do preset não determina o hardware instalado. Selecione o módulo pelo Auto-Scan. Veículos TSI com plataforma não suportada pelo módulo selecionado geram aviso de whitelist.

Manual e automático compartilham EDS 2 nestes motores; `configureTransmission()` altera somente a máscara 07 do byte 15 e preserva os outros bits. Não há inferência de HBV ou alteração do byte 16 bit 7 por causa do câmbio. Configure o HBV no editor avançado com base no equipamento e códigos PR.
