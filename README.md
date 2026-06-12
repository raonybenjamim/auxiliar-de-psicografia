# Auxiliar de Psicografia

O **Auxiliar de Psicografia** é uma aplicação web de página única (standalone) desenhada para simular um dispositivo de captação mediúnica ou "ouija" digital moderno. Com uma estética escurecida e tons pastéis em roxo, ele oferece uma experiência focada na interação tátil em dispositivos móveis.

A aplicação funciona inteiramente através de um único arquivo `index.html`, dispensando instalações complexas, servidores ou dependências externas. 

## 📋 Funcionalidades

- **Faixa de Caracteres Infinita:** Uma fita com letras, números e símbolos que desliza perfeitamente de forma contínua.
- **Dial Tátil:** Controle giratório inspirado em botões físicos de equipamentos de rádio antigos.
- **Feedback Háptico:** Vibração responsiva ao interagir com o dial (apenas em dispositivos suportados, como Android).
- **Auto-Embaralhamento:** O alfabeto se reorganiza sozinho a cada caractere selecionado para dificultar a previsibilidade e encorajar uma seleção guiada pelo subconsciente.
- **Exportação Fácil:** Salve todo o registro da sessão num arquivo de texto `.txt` direto para o seu dispositivo.

---

## 📖 Tutorial de Uso

### 1. Como Abrir
Por ser construído em HTML puro, você não precisa instalar nada.
- **No Computador:** Basta dar um clique duplo no arquivo `index.html` para que ele abra no seu navegador padrão (Google Chrome, Firefox, Safari, etc.).
- **No Celular:** Você pode enviar o arquivo `index.html` para o seu celular ou hospedar a pasta localmente na sua rede. Para ter a melhor experiência tátil com vibração, recomendamos o uso em dispositivos Android.

### 2. Escrevendo (Girando o Dial)
A parte inferior da tela contém o **Dial de Controle** (um grande círculo roxo escuro). 
1. Toque (ou clique) no Dial e mantenha pressionado.
2. Faça um movimento circular, como se estivesse girando o botão de volume de um rádio. 
3. Você verá que a **Faixa de Caracteres** no meio da tela começará a deslizar para a direita ou esquerda em sincronia com o seu movimento.
4. O objetivo é girar até que a letra que você deseja forme um alinhamento perfeito com o **Marcador Central** (a linha luminosa roxa apontando para baixo).

### 3. Selecionando a Letra
Assim que a letra desejada estiver sob o marcador central, **solte o Dial (levante o dedo)**.
- O sistema fará um "snap" automático para encaixar a letra perfeitamente no centro.
- A letra será adicionada na **Janela de Texto** no topo da tela.
- **Embaralhamento:** Imediatamente após a letra ser escrita, as letras da faixa vão mudar aleatoriamente de posição para a sua próxima escolha.

### 4. Apagando e Dando Espaço
As opções de espaço e apagar não são botões separados; elas fazem parte da caçada mediúnica.
- Procure na Faixa de Caracteres pelo símbolo **`␣`** para dar um espaço entre as palavras.
- Procure pelo símbolo **`⌫`** se precisar apagar a última letra digitada.

### 5. Limpar a Sessão e Salvar
No topo da tela, você tem dois botões de comando:
- **LIMPAR:** Apaga todo o histórico da janela de texto. O sistema pedirá uma confirmação antes de apagar permanentemente.
- **SALVAR TEXTO:** Cria um arquivo de texto chamado `psicografia_AAAAMMDD.txt` contendo tudo o que você escreveu e fará o download instantaneamente para o seu aparelho.

---

## ⚠️ Nota sobre Dispositivos Apple (iOS)
O mecanismo de Feedback Háptico (vibração ao girar e selecionar) utiliza a API web `navigator.vibrate`. Atualmente, navegadores no sistema iOS (iPhones e iPads) não suportam esta tecnologia via web. O aplicativo funcionará perfeitamente nestes dispositivos, mas a função de vibração tátil será silenciosamente ignorada pelo sistema da Apple.
