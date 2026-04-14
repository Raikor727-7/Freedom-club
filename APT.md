# O que são grupos hackers ou APTs?
> **APT** significa: *Advanced Persistent Threat* (Ameaça Avançada e Persistente).

## Advanced (Avançada):
-  Usam técnicas sofisticadas, exploits zero-day, malware customizado, engenharia social bem feita, living-off-the-land (usar ferramentas nativas do sistema) e evitam detecção por longos períodos.

## Persistent (Persistente):
- Não são ataques rápidos. Eles entram na rede da vítima, ficam “dormindo” por meses ou anos, roubam dados aos poucos, se movimentam lateralmente e mantêm acesso mesmo depois de serem parcialmente descobertos.

## Threat (Ameaça): 
- Quase sempre são grupos patrocinados por Estados-nação (governos) ou atuam em nome deles. O objetivo principal é espionagem cibernética (roubo de segredos de Estado, tecnologia, dados diplomáticos, militares ou econômicos), embora alguns também façam operações financeiras ou destrutivas.

> Diferente de criminosos comuns (como grupos de ransomware que querem dinheiro rápido), os APTs são pacientes, bem financiados e têm objetivos estratégicos de longo prazo.

## Exemplos clássicos de grupos APT:

- **Lazarus Group** (Coreia do Norte)
    - Um dos mais famosos e prolíficos. Atua desde ~2009. Responsável por ataques como o WannaCry (2017), roubo de centenas de milhões em criptomoedas, espionagem contra bancos, governos e empresas. Tem muitas famílias de malware (mais de 130 no Malpedia). Faz tanto espionagem quanto operações para gerar receita para o regime.

- **APT28** (também chamado Fancy Bear, Sofacy, Sednit – atribuído ao GRU russo, inteligência militar)
    - Ativo desde ~2004. Famoso por interferência eleitoral (ex: [vazamento de e-mails do DNC em 2016](https://en.wikipedia.org/wiki/2016_Democratic_National_Committee_email_leak)), ataques contra OTAN, governos europeus, militares e logística. Usa malware como X-Agent, Sofacy, etc. Tem cerca de 42 famílias associadas no Malpedia.

- **Turla** (também Venomous Bear, Waterbug – atribuído ao FSB russo)
    - Um dos grupos mais antigos e sofisticados (desde ~2004). Especialista em espionagem contra governos, embaixadas, organizações internacionais e pesquisa. Conhecido por técnicas muito criativas (ex: usar satélites ou sites comprometidos como infraestrutura). Tem cerca de 39 famílias no Malpedia.

## Quais são os grupos “maiores” do mundo segundo o Malpedia?
O Malpedia não diz oficialmente “este é o maior”, mas ordena pela quantidade de famílias de malware associadas (quanto mais malware diferente um grupo usa ou desenvolve, maior costuma ser sua escala de operações). Aqui está o ranking aproximado atual (baseado na página de actors):

| Posição | Grupo | Famílias de Malware | Atribuição principal | Motivação principal |
| -- | -- | -- | -- | -- |  
| 1 | Lazarus Group | 136 | Coreia do Norte | "Espionagem + Geração de receita (criptomoedas, roubo bancário) para sustentar o regime" | 
| 2 | "APT28 (Fancy Bear, Sofacy)" | 42 | Rússia (GRU) | "Espionagem militar, interferência política e coleta de inteligência sobre OTAN e Europa" |
| 3 | "Turla (Venomous Bear, Waterbug)" | 39 | Rússia (FSB) | "Espionagem de longo prazo contra governos, embaixadas e organizações internacionais"
| 4 | Cleaver | 38 | Irã (provável) | Espionagem contra alvos do Oriente Médio e interesses ocidentais
| 5 | APT1 (Comment Crew) | 35 | China (PLA Unit 61398) | Roubo de propriedade intelectual e segredos industriais/militares
| 6 | UNC2452 | 35 | Rússia (relacionado ao SolarWinds) | Espionagem em cadeia de suprimentos e governos
| 7 | APT41 (Double Dragon) | 34 | China | Espionagem estatal + Atividades financeiras/criminais (dupla motivação)
| 8 | "APT29 (Cozy Bear,  Midnight Blizzard)" | 30 | Rússia (SVR/FSB) | "Espionagem diplomática, governamental e de infraestrutura crítica"
| 9 | CHRYSENE | 30 | Irã | Espionagem contra alvos regionais e ocidentais
| 10 | OilRig (APT34) | 29 | Irã | "Espionagem energética |  governamental e de infraestrutura"

_Esses números mudam com o tempo, pois novas famílias são descobertas e adicionadas._

## Como os 10 primeiros agem (táticas principais)

### Lazarus Group (Coreia do Norte)
**Motivação:** Espionagem estratégica + roubo de dinheiro para financiar o programa nuclear e o regime.  
**Como agem:** Phishing sofisticado, watering hole (sites infectados), exploits zero-day, roubo de criptomoedas, ransomware (ex: WannaCry) e supply chain attacks. São muito agressivos e versáteis.

### APT28 (Rússia)
**Motivação:** Apoiar objetivos militares e de inteligência russa, interferir em eleições/política.  
**Como agem:** Spear-phishing, exploits em webmail (ex: Roundcube), malware como X-Agent e Sofacy, credenciais roubadas e movimento lateral rápido.

### Turla (Rússia)
**Motivação:** Espionagem de longo prazo e coleta de inteligência diplomática/militar.  
**Como agem:** Técnicas extremamente criativas (uso de satélites, sites comprometidos como C2), backdoors persistentes e stealth elevado. São um dos grupos mais pacientes e sofisticados.

### Cleaver (Irã)
**Motivação:** Espionagem contra inimigos regionais e interesses ocidentais.  
**Como agem:** Ataques a setores de energia, governo e defesa, com foco em persistência e exfiltração de dados.

### APT1 (China)
**Motivação:** Roubo de tecnologia e propriedade intelectual para acelerar o desenvolvimento chinês.  
**Como agem:** Operações em grande escala contra empresas (principalmente EUA e Europa), uso de malware customizado e spear-phishing direcionado.

### UNC2452 (Rússia)
**Motivação:** Espionagem em larga escala via cadeia de suprimentos.  
**Como agem:** Comprometimento de software legítimo (ex: SolarWinds), movimento silencioso e acesso a múltiplas vítimas ao mesmo tempo.

### APT41 (China)
**Motivação:** Espionagem estatal + lucro financeiro (raro entre grupos chineses).  
**Como agem:** Misturam técnicas de espionagem com roubo de cripto, ransomware e ataques a jogos/empresas. Usam tanto ferramentas estatais quanto criminosas.

### APT29 (Cozy Bear – Rússia)
**Motivação:** Espionagem diplomática e de infraestrutura.  
**Como agem:** Spear-phishing em massa, uso de RDP, ferramentas living-off-the-land e campanhas longas contra governos e provedores de TI.

### CHRYSENE (Irã)
**Motivação:** Espionagem regional e contra interesses ocidentais.  
**Como agem:** Ataques direcionados a governos e indústrias, com foco em persistência.

### OilRig (Irã)
**Motivação:** Espionagem no setor de energia e governo.  
**Como agem:** Malware customizado voltado para exfiltração de dados sensíveis de infraestrutura crítica.

## Observações importantes

- Esses grupos não são “hackers independentes anti-governo”. São estruturas estatais (ou semi-estatais) com orçamento, treinamento militar/inteligência e objetivos nacionais.
- Muitos usam táticas parecidas: phishing (especialmente spear-phishing), exploração de vulnerabilidades, persistência longa e living-off-the-land.
- O ranking do Malpedia mede volume de malware conhecido, não necessariamente “quem é o mais perigoso hoje”. Em 2025/2026, grupos como Salt Typhoon (China) e Sandworm (Rússia) também apareceram muito em relatórios recentes.


> Como usar o Malpedia para ver isso?  
Acesse: [O site do Malpedia](https://malpedia.caad.fkie.fraunhofer.de/actors)  
Você verá a tabela com os grupos e o número de famílias.  
Clique em qualquer grupo (ex: Lazarus) para ver todas as famílias de malware ligadas a ele, descrições, aliases e referências.

# Parte 2: Checklist para Criar um Grupo Hackers **em um RPG**
## 2.1. Defina a Estrutura
**Quantos membros?**

> *Célula pequena (3-8)*: Mais difícil de rastrear, menos recursos  
*Organização média (20-50)*: Divisão de funções (recon, dev malware, operações, comunicação)  
*Rede ampla (100+)*: Maior poder de fogo, mas maior risco de infiltração

**Como se organizam?**

>Estrutura celular (ninguém conhece todos os membros)  
Hierarquia clara (líder, sub-líderes, operadores)  
Coletivo horizontal (decisões por consenso)

**Financiamento:**
- Doações anônimas (criptomoedas)
- Roubo de criptomoedas (como Lazarus)
- Apoio externo (nação rival da Terra 727)

ou até: Trabalhos paralelos legítimos que financiam a operação

## 2.2. Crie a Infraestrutura (OPSEC)
No mundo real, grupos como Turla usam técnicas sofisticadas, exemplos de infraestrutura básica:

| Camada | Elementos | Como os jogadores podem detectar |
| -- | -- | -- |  
| Comunicação | Criptografia (Signal, Matrix, IRC over Tor), servidores próprio | Tráfego cifrado em horários específicos, servidores incomuns | 
| Operações | VPS em países sem extradição, servidores sequestrados (comprometidos), infraestrutura via satélite | Rastreamento de C2 (command & control), padrões de tráfego | 
| Anonimização | Tor, VPNs em cadeia, uso de redes Wi-Fi públicas comprometidas | Erros operacionais (ex: IP vazado em log) | 
| Malware | Customizado (evita AV), living-off-the-land (usa ferramentas do sistema) | Artefatos forenses, comportamento anômalo |

## 2.3. Defina as Capacidades Técnicas
Nível de sofisticação do grupo(ou célula depende do seu RPG):

| Nível | Capacidades | Exemplos no seu RPG | 
| -- | -- | -- |
Baixo | Phishing básico, ferramentas públicas, alvos fáceis | Grupo iniciante, recém-formado |
| Médio | Malware customizado simples, engenharia social eficaz, persistência básica | Resistência local, com alguns técnicos experientes |
| Alto | Zero-days, movimento lateral avançado, stealth prolongado | Grupo apoiado por nação externa, ex-agentes do governo | 
| Lendário | Capacidade de atacar infraestrutura crítica, operações simultâneas, supply chain attacks | Ameaça nível APT — o grupo que seus jogadores temem | 

## 2.4. Motivação e Linhas Vermelhas
O que o grupo não faz é tão importante quanto o que faz, então defina regras:

exemplos:
- Não atacam hospitais → revela ética
- Não usam ransomware → são idealistas, não criminosos
- Não aceitam membros de certas facções → mostra vieses internos
