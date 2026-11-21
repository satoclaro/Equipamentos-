# EMTA Config & Scanner Pro (v1.3)

Ferramenta HTML para técnicos de telecomunicações em campo.

## Novidades da Versão 1.3
- **Abertura da Câmera Corrigida (`getUserMedia` + fallback de dispositivos + ZXing)**:
  - Usa `getUserMedia` direto com sequência de fallbacks (`facingMode` ideal -> exato -> `video: true` -> enumeração de câmeras `enumerateDevices` por `deviceId`), evitando falhas quando o aparelho/navegador rejeita restrições de resolução ou foco no `start()`.
  - Integra `decodeFromVideoDevice` / `decodeFromStream` do ZXing após o stream de vídeo estar ativo e em reprodução.
  - Inclui alternância de câmera, controle de luz (`torch`), toque no vídeo para focar, captura de foto e fallback por **Câmera Nativa / Foto**.
- **Rodapé Atualizado**: `Criado por Fernando Sato - Versão 1.3 - 20.11.26 - 21:29`.