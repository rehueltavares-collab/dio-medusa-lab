# Relatório Técnico — Lab Medusa (Resumo)

## Autor
Rehuel da Silva Tavares

## Objetivo
Demonstrar técnicas de força-bruta (FTP, Web, SMB) usando Medusa em ambiente controlado.

## Ambiente
- Kali Linux (atacante)
- Metasploitable2 (alvo)
- DVWA (alvo web)
- Rede: Host-Only (VirtualBox)

## Procedimentos executados
- Enumeração: nmap
- FTP brute-force: medusa -M ftp ...
- Web-form: medusa -M web-form ... (ajustar campos)
- SMB: enum4linux + medusa -M smbnt (password spraying)

## Evidências
- outputs/*.txt
- images/*.png

## Recomendações
- Rate-limiting, MFA, políticas de senha, desabilitar serviços inseguros.

