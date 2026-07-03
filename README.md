# WiFrisk - Pentest Wifi para Windows

<p align="center">
  <img src="Wi.png" alt="WiFrisk Banner" width="128" />
</p>

[![Versão](https://img.shields.io/badge/vers%C3%A3o-1.0.0-green.svg)](CHANGELOG.md)
[![Licence](https://img.shields.io/badge/licence-MIT-blue.svg)](LICENSE)
[![Windows](https://img.shields.io/badge/platform-Windows-blue.svg)](https://www.microsoft.com)

WiFrisk é uma ferramenta de pentest de redes Wi-Fi para Windows, projetada para facilitar atividades seguras de avaliação de redes sem fio em ambientes autorizados. Este projeto é destinado apenas a profissionais de segurança certificados que atuam em redes sob autorização explícita. Use com responsabilidade.

---

## Sumário
- [Recursos](#recursos)
- [Pré-requisitos](#pré-requisitos)
- [Instalação](#instalação)
- [Como usar](#como-usar)
- [Especificações do Adaptador USB EDUP AX1672 WiFi 6E (MTK7921AU)](#especificações-do-adaptador-usb-eduP-ax1672-wifi-6e)
- [Contribuição](#contribuição)
- [Conformidade e Ética](#conformidade-e-ética)
- [Atualizações](#atualizações)
- [Licença](#licença)
- [Contato](#contato)

---

## Recursos
- Varredura de redes sem fio disponíveis
- Análise de sinal e qualidade de conexão
- Detecção de dispositivos conectados
- Exportação de resultados para CSV/JSON
- Interface simples e leve para Windows
- Logs locais com opções de verbose

Observação: WiFrisk não deve ser utilizado sem autorização prévia do proprietário da rede. Em ambientes empresariais, siga as políticas de segurança da informação da organização.

---

## Pré-requisitos
- Windows 10 ou superior
- Python 3.x (se aplicável; substitua por runtime do seu app se for nativo)
- Privilégios de administrador podem ser necessários para certas operações
- Drivers de adaptador de rede compatíveis

Observação: se o projeto for nativo, liste as dependências específicas (SDKs, runtimes, etc.) e como instalá-las.

---

## Instalação

Opção A – Executável (recomendado)
1. Baixe o instalador disponível em releases.
2. Execute o instalador e siga as instruções.
3. Abra o WiFrisk a partir do Menu Iniciar.

Opção B – Do source (caso você seja desenvolvedor)
1. Clone o repositório:
   - git clone https://github.com/seu-usuario/WiFrisk.git
2. Navegue até a pasta do projeto:
   - cd WiFrisk
3. Instale dependências:
   - npm install (ou o comando equivalente para o seu runtime)
4. Construa o aplicativo:
   - npm run build (ou o comando que você usar)
5. Execute o aplicativo:
   - npm run start (ou o executável gerado)

Notas:
- Substitua os comandos pelos do seu stack (C#, Electron, Python, etc.).
- Instruções específicas devem refletir a forma de distribuição do seu projeto.

---

## Como usar

1. Abra o WiFrisk com privilégios de administrador (se necessário).
2. Escolha a interface de rede a ser analisada.
3. Inicie a varredura para listar redes disponíveis.
4. Selecione uma rede para ver detalhes (canal, potência, BSSID, etc.).
5. Exporte resultados, se desejar, para CSV ou JSON.
6. Consulte logs para diagnóstico.

Dicas:
- Use apenas em redes sob autorização explícita.
- Não utilize para atividades maliciosas ou invasivas.

---

## Especificações do Adaptador USB EDUP AX1672 WiFi 6E (MTK7921AU)

- Chipset: MTK7921AU
- Suporte a VIF, Monitoramento e Injeção de Pacotes, além de Modo AP
- Taxa de transmissão sem fio de até 3000 Mbps (AX3000)
- Velocidade sem fio por banda:
  - 2,4 GHz: até 600 Mbps
  - 5 GHz: até 1200 Mbps
  - 6 GHz: até 1200 Mbps
- Interface: USB 3.0 de alta velocidade
- Antenas: 2x antenas de 5 dBi (banda dupla)
- Sistema Operacional: Windows 10, Windows 11, Linux (kernel ≥ 5.19)
- Auto-instalação (instalação automática de drivers, quando suportado)
- Compatibilidade: suporta dispositivos 802.11 ax/ac/a/b/g/n
- Segurança sem fio:
  - WEP (64/128 bits)
  - WPA/WPA2
  - WPA-PSK/WPA2-PSK (TKIP/AES)
  - WPS
- Alcance estimado: 15-20 metros (varia com ambiente)
- Plug-and-play para Linux (≥ kernel 5.19)
- Observações de driver:
  - Windows 10: possível funcionamento em 5 GHz e 2,4 GHz
  - Windows 11/Linux: suporte a 6 GHz (se roteador for compatível)

Notas úteis:
- Este adaptador é adequado para videoconferência em HD, jogos e streaming sem interrupções quando utilizado sob as bandas suportadas.
- Garantia de conformidade com políticas de uso de rede e regulamentações locais.

---

## Contribuição

Contribuições são bem-vindas! Siga estas etapas:

1. Fork o repositório
2. Crie uma branch para a sua feature: git checkout -b feature/nova-funcionalidade
3. Faça commit das suas alterações: git commit -am 'feat: descrição da alteração'
4. Envie a branch: git push origin feature/nova-funcionalidade
5. Abra um pull request
