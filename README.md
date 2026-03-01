<p align="center">
  <img src="https://gustavozs.ovh/assets/Astralvioleta.png" width="180" alt="Astral Cloud Logo">
</p>

<h1 align="center">🌌 Astral Cloud — Instalador Automático</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Versão-2.1.0-6e54ff?style=for-the-badge">
  <img src="https://img.shields.io/badge/Status-Estável-2ea44f?style=for-the-badge">
  <img src="https://img.shields.io/badge/OS-Ubuntu%20%7C%20Debian-1f6feb?style=for-the-badge">
  <img src="https://img.shields.io/badge/Licença-MIT-E9430F?style=for-the-badge">
</p>

<p align="center">
  <strong>Infraestrutura de hospedagem pronta em poucos minutos.</strong><br>
  Script oficial para configuração do <b>Pterodactyl Panel & Wings</b> com Docker, SSL e otimizações de rede.
</p>

---

## 🚀 Funcionalidades

Chega de perder horas configurando dependências manualmente. O script cuida de todo o "trabalho sujo":

* **Stack Completa:** Instalação automática de PHP, MySQL, Nginx e Docker.
* **Performance BR:** Troca automática de mirrors para repositórios brasileiros (downloads muito mais rápidos).
* **Segurança:** Configuração de Firewall (UFW) e permissões de diretórios.
* **Certificado SSL:** Integração nativa com Let's Encrypt para HTTPS automático.
* **Resiliência:** Configuração de serviços via `systemd` para auto-inicialização no boot.

---

## 🐧 Compatibilidade

Otimizado para as distribuições Linux mais sólidas do mercado:

| Sistema | Versões Homologadas | Status |
| :--- | :--- | :--- |
| **Ubuntu** | `22.04 LTS` e `24.04 LTS` | 🟢 Recomendado |
| **Debian** | `11`, `12` e `13 (Trixie)` | 🟢 Estável |

> [!IMPORTANT]
> **Atenção à Virtualização:** Para que o Wings funcione, sua VPS **precisa** ser **KVM** ou **Dedicado**. O Docker não é compatível com virtualizações compartilhadas como OpenVZ ou LXC.

---

## ⚡ Instalação One-Click

Conecte-se ao seu servidor via SSH como **root** e rode o comando:

```bash
curl -sSL "https://raw.githubusercontent.com/DoutorLouness/instalacao-ptero/refs/heads/main/install.sh?v=$RANDOM" | bash
