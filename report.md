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


## Observação (FTP)
Autenticação bem-sucedida para 'ftp' em vsftpd (192.168.56.102). Diretório raiz vazio. Evidência sanitizada: outputs/ftp_evidence_sanitized.txt. Outputs completos mantidos localmente.

## Observação (SMB)
Enumeração SMB executada; password-spray com wordlists reduzidas não retornou credenciais. Evidência sanitizada: outputs/smb_evidence_sanitized.txt

## Observação (MySQL)
Tentativas de autenticação MySQL executadas; sem credenciais válidas encontradas com wordlists utilizadas. Evidência sanitizada: outputs/mysql_evidence_sanitized.txt
