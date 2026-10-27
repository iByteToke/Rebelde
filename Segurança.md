# Segurança e Verificação - REBELDE ($RBD) 🛡️

A segurança dos detentores de **REBELDE ($RBD)** e a transparência absoluta do código são os pilares fundamentais deste projeto. Este documento detalha as medidas de segurança implementadas no contrato inteligente e o estado da sua verificação na blockchain.

## 1. Verificação do Contrato (Contract Verification)
O contrato inteligente da $RBD foi totalmente verificado e publicado na BNB Smart Chain (BSC). Isto significa que o código-fonte legível por humanos corresponde exatamente ao *bytecode* em execução na blockchain, permitindo que qualquer pessoa audite o seu funcionamento.

* **Endereço do Contrato:** `0x09fe4c3C8c82DD03aD8166B456d1f573EAb894F6`
* **Status no BscScan:** ✅ Verificado (Matching Bytecode and ABI)
* **Link para Auditoria Pública:** [BscScan - Código do Contrato](https://bscscan.com/address/0x09fe4c3C8c82DD03aD8166B456d1f573EAb894F6#code)

## 2. Recursos de Segurança do Código (Security Features)
O código foi desenvolvido seguindo as melhores práticas do padrão BEP-20, com proteções rígidas ("hardcoded") para proteger os investidores:

* **No Minting (Sem Impressão de Moedas):** O contrato **não possui** a função `mint()`. É tecnicamente impossível para o criador ou para qualquer outra pessoa gerar novos tokens. A oferta máxima está trancada para sempre.
* **No Tax (Sem Taxas Ocultas):** Não existem funções para cobrar taxas (fees) sobre transferências, compras ou vendas. O contrato não desvia fundos das transações dos utilizadores.
* **Initial Burn (Queima Inicial):** Imediatamente após a implementação, 2.000.000 RBD foram enviados para o endereço nulo (`0x000...000`), reduzindo a oferta permanentemente e provando o mecanismo de deflação.
* **Possibilidade de Renúncia (Renounce Ownership):** O contrato possui a função `renounceOwnership()`. Isto permite ao criador abdicar do controlo do contrato a qualquer momento, tornando a $RBD um bem 100% gerido pela própria blockchain e pela comunidade.

## 3. Relato de Vulnerabilidades (Reporting a Vulnerability)
Embora o contrato seja uma implementação direta e segura do padrão BEP-20, levamos a segurança muito a sério. 

Se encontrar qualquer vulnerabilidade ou comportamento inesperado, por favor:
1. **Não** explore a falha de forma maliciosa.
2. Abra uma *Issue* neste repositório do GitHub descrevendo o problema, ou entre em contacto direto com o criador (Thomas A. Anderson) através dos canais oficiais da comunidade.

## 4. Auditorias de Terceiros (Audits)
A $RBD encoraja a comunidade e empresas de segurança independentes a realizarem auditorias ao nosso código-fonte aberto. Quaisquer relatórios de auditoria futuros serão publicados e linkados nesta secção.
