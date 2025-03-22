### 📝 **Descrição do Script de Migração BRLN Bolt**

Este script Bash foi desenvolvido para **automatizar a migração completa de um nó Lightning existente para a estrutura do BRLN Bolt**, um setup limpo, seguro e modular com suporte às melhores práticas da comunidade Lightning Network.  

Ele garante uma transição suave, com foco em manter a segurança e a estabilidade da operação do node após a migração.

---

### 🔧 **Funcionalidades do Script**

1. **Atualização opcional do sistema**
2. **Instalação e configuração do Tor + i2pd**
3. **Instalação segura do Bitcoin Core (bitcoind)**
   - Com suporte a proxy Tor e integração com LND
4. **Download e verificação GPG do LND**
5. **Geração e configuração do arquivo `lnd.conf` personalizado**
   - Compatível com Tor, ClearNet e modo híbrido
   - Permite alternância entre Bitcoin Core local e remoto
6. **Criação dos serviços systemd para:**
   - `bitcoind`
   - `lnd`
   - `bos-telegram`
   - `thunderhub`
   - `lndg`
7. **Ferramentas de administração integradas:**
   - 🖥️ ThunderHub
   - ⚡ BOS - Balance of Satoshis
   - 🐍 LNDG (backend Django)
8. **Menu interativo com 3 etapas:**
   - `1` ➝ Instala o BRLN Bolt base (Tor + LND + Bitcoin Core)
   - `2` ➝ Alterna entre node Bitcoin local ou remoto
   - `3` ➝ Instala as ferramentas de administração

---

### ✨ **Diferenciais para migração**

- Permite configurar o `bitcoind` como local ou apontar para um servidor remoto.
- Automatiza permissões, estrutura de pastas e inicialização dos serviços.
- Ajuda a evitar erros comuns de migração (TLS, macaroon, permissões).
- Compatível com o ecossistema do **MiniBolt/BRLN Bolt**, focado em soberania e facilidade de uso.
