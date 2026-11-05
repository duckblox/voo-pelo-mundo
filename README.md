[README.md](https://github.com/user-attachments/files/34453684/README.md)
# ✈️ Voo pelo Mundo

> **Decole do Brasil. Descubra o mundo.**

## ▶️ [**JOGAR AGORA → duckblox.github.io/voo-pelo-mundo**](https://duckblox.github.io/voo-pelo-mundo/)

*Abra o link no navegador do computador, do tablet ou do celular (de preferência Chrome ou Edge, que têm mais vozes). Não precisa instalar nada nem criar conta. Precisa só de internet para carregar o globo 3D (veja **Detalhes úteis**).*

---

Um jogo para aprender geografia viajando de avião: o Boeing decola do Rio de Janeiro, cruza oceanos e continentes e pousa em outro país (ou volta para casa), com cabine, passageiros, globo terrestre e a paisagem do destino.

## 🎮 Como jogar
Na tela inicial:

1. **Escolha o destino** tocando em uma bandeira.
2. **Escolha o sentido:** 🇧🇷 *Ida* (Brasil → país) ou *Volta* (país → Brasil).
3. Aperte **✈️ DECOLAR** e acompanhe o voo. Não há pontos, tempo nem erro: é só olhar, ouvir e descobrir.

## 🌍 Destinos
Rio de Janeiro ↔ **Nova York** (EUA), **Paris** (França), **Londres** (Reino Unido), **Lisboa** (Portugal), **Buenos Aires** (Argentina), **Roma** (Itália), **Moscou** (Rússia), **Cairo** (Egito), **Cidade do Cabo** (África do Sul), **Dubai** (Emirados Árabes), **Nova Délhi** (Índia), **Pequim** (China), **Tóquio** (Japão) e **Sydney** (Austrália).

Ao pousar, um cartão mostra a **bandeira**, o aeroporto, a capital, o continente, o monumento famoso, curiosidades, quantos quilômetros foram voados e **por onde o avião passou**. Em seguida vem um **quiz rápido em português e inglês** (continente e capital), sem nota e sem erro: se a resposta não for a certa, o jogo só mostra a correta.

## 🧊 Rotas seguras (e a Antártida)
Os aviões comerciais escolhem caminhos com **aeroportos por perto**, para o caso de uma emergência. Por isso quase nenhuma rota passa pela Antártida, onde há pouquíssimos aeroportos.
- Em linha reta, o Rio → Sydney passaria bem em cima da Antártida. No jogo, o voo faz **escala na África do Sul** e contorna o continente gelado.
- No globo, os **pontos amarelos 🟡** são aeroportos de emergência perto da rota.
- Durante o voo, o jogo avisa em inglês e português: *"Safe route: planes avoid Antarctica"*.

## 🎥 8 câmeras (teclas **1** a **8**)
| Tecla | Câmera | O que mostra |
|---|---|---|
| 1 | 🧑‍✈️ Cabine de comando | Os pilotos, os instrumentos e a pista pela janela da frente |
| 2 | 🪑 Passageiros | A poltrona, a tela de voo com mapa e a janela com a asa |
| 3 | 🛒 Corredor | Fileiras de passageiros e comissárias servindo |
| 4 | 🌍 Globo | O globo terrestre com continentes, cidades e a rota do avião |
| 5 | 🪟 Asa | A janela, a asa, o motor e o flap abrindo |
| 6 | 🛩️ Externa | O avião visto por trás, alinhado com a pista |
| 7 | ↔️ Lateral | O avião de perfil, decolando e pousando |
| 8 | 🛬 Frontal | O avião vindo de frente, com luzes e motores girando |

## 🧭 Aprendendo no caminho
- **Continentes e oceanos:** o nome aparece no alto da tela conforme o avião sobrevoa.
- **Países:** mais de 40 países aparecem no caminho, com a capital e a bandeira dos principais, e no fim você vê a lista do que sobrevoou.
- **Altitude e velocidade:** o painel mostra altitude em metros e em pés, velocidade em km/h e quanto falta.
- **Inglês sem pressão:** frases curtas aparecem em **inglês e português** ("Takeoff! / Decolando!").
- **Pouso de verdade:** a voz do avião conta a altura até o chão ("One thousand, five hundred… fifty, forty, thirty, twenty, ten… retard"), com o número grande na tela e a tradução embaixo.
- **Do amanhecer ao pôr do sol:** o céu muda durante o voo, e as luzes da cidade acendem na chegada.

## 🔊 Som
Música, motor, avisos e toque na pista são criados pelo próprio código (Web Audio). As falas usam as vozes do próprio navegador (em português e em inglês).
- Na tela inicial aparece quais vozes foram encontradas. O botão **🔔 Testar voz** confere se estão funcionando.
- Em **⚙️ Configurações** há volumes separados para a voz, a música e o motor.
- Os botões **🎵 Música** e **🔊** do topo ligam e desligam o som.

## 🌿 Modo calmo
Vem ligado por padrão: sem tremor de câmera nem balanço, para uma viagem tranquila. Dá para desligar em ⚙️ Configurações.

## ℹ️ Detalhes úteis
- O globo 3D usa a biblioteca **Three.js**, carregada de `cdnjs.cloudflare.com`. Por isso é preciso estar conectado à internet na primeira abertura.
- O jogo **não coleta nem guarda dados**. Nada é salvo no aparelho.
- O mapa usa **contornos simplificados** dos continentes, sem fronteiras de países. Os marcadores e as cidades estão na posição correta.
- A qualidade das vozes depende do aparelho e do navegador. Se não houver voz em português ou inglês, as legendas continuam na tela.
- O voo dura cerca de 100 segundos de jogo (a duração real da viagem é só uma comparação mostrada no cartão de chegada).

## 🛠️ Para quem quer aprender a programar
O `index.html` é um único arquivo. O script é dividido em seções marcadas com comentários `/* ---------- ... ---------- */` (bandeiras, destinos, mapa, voz e áudio, perfil de voo, cenários 2D, viagem e laço principal). Comece por estes valores:
- `DS`: a lista de destinos (cidade, aeroporto, coordenadas, monumento e curiosidades). Copie um bloco para criar um destino novo. O campo `via` cria uma rota com escala (lista de coordenadas).
- `EA`: os aeroportos de emergência mostrados como pontos amarelos no globo.
- `FG`: as bandeiras, desenhadas em SVG com formas simples.
- `PG`: os polígonos dos continentes (longitude e latitude).
- `CNT`: os países citados durante o voo (nome, posição e capital).
- `T`: a duração do voo, em segundos de jogo.
- `FT`: os avisos de altura do pouso, em pés, em inglês e português.
- `lmk`: o desenho dos monumentos de cada país.

## 🧩 Tecnologias
HTML, CSS e JavaScript puro, com `<canvas>` 2D para as câmeras e **Three.js** para o globo. Sem imagens externas: tudo é desenhado pelo código.
