# EMTA Config & Scanner Pro — v3.2

Ferramenta de campo para técnicos de telecomunicações focada em leitura de etiquetas/códigos de modems e EMTAs, acesso rápido ao gateway (`192.168.0.1`), validação de níveis RF, cópia rápida de credenciais e arquivamento local com exportação.

## Funcionalidades Principais

- **Acesso Rápido & Campos Sincronizados**:
  - Atalho direto para `http://192.168.0.1` e cópia rápida de IP/URL.
  - Sincronização em tempo real entre os campos da barra superior e os campos principais (`Usuário IP`, `Senha do Usuário`, `Nome da Rede Wi-Fi`, `Senha Wi-Fi`).
  - Campo fixo de **Senha Padrão Claro** (`Claro_123456789`) com botão de copiar.

- **Diagnóstico de Conectividade (Ping / Reachability)**:
  - Execução de probes HTTP/TCP com medição de latência média (RTT) e status visual (`Online`, `Instável` ou `Sem alcance direto`).

- **Câmera, QR Code, Código de Barras & OCR**:
  - Leitura contínua via câmera (`ZXing`) com troca de câmera, controle de lanterna (quando suportado), foco ao toque e captura de foto.
  - Suporte a **Câmera Nativa / Foto**, rotação de imagem em 90° e reconhecimento de texto via **OCR (`Tesseract.js`)**.
  - Extração automática para campos como Modelo/EMTA, Fabricante, DOCSIS, P/N, Fabricação, Voltagem, IP, Usuário (`Claro_` / `NET_`), Redes Wi-Fi (`2.4`, `5.0`, `GHz`), Senhas, MAC (`CM MAC` / `EMTA MAC`) e Serial (`S/N`).

- **Indicador de Níveis RF (Padrão da Empresa)**:
  - **Tx / Upstream**: `38` a `51 dBmV`
  - **Rx / Downstream**: `-12` a `+12 dBmV`
  - **SNR DS**: `> 35 dB`
  - **SNR UP**: `> 27 dB`

- **Arquivo de EMTAs & Exportação**:
  - Armazenamento local (`LocalStorage`) com busca instantânea, carregamento nos campos, cópia individual ou em lote.
  - Exportação e importação em **JSON**, backup em **CSV** e geração local de **PDF** (`📄 Baixar PDF`) respeitando o filtro ativo.

## Como Usar

1. Abra o arquivo `index.html` em um navegador moderno (de preferência em `localhost` ou `https://` para uso da câmera ao vivo).
2. Utilize a câmera, carregue uma foto da etiqueta ou cole/digite os dados no campo de leitura para preencher os campos.
3. Confira os níveis RF, copie os dados necessários ou salve o registro no **Arquivo de EMTAs**.
4. Exporte os registros salvos em **PDF**, **CSV** ou **JSON** conforme necessário.

---
Criado por Fernando Sato — Versão 3.2
