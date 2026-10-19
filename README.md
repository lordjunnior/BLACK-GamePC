<div align="center">

# 🔫 LordGames | BLACK (2006) para PC

### Port nativo e não oficial do **BLACK** do Xbox original para PC, com gráficos estendidos, teclado e mouse

![Plataforma](https://img.shields.io/badge/plataforma-Windows%2010%2B%2064--bit-0078D6?logo=windows&logoColor=white)
![API gráfica](https://img.shields.io/badge/gráficos-Direct3D%2012-107C10)
![Técnica](https://img.shields.io/badge/técnica-recompilação%20estática-red)
![Controle](https://img.shields.io/badge/controle-SDL3-blue)
![HDR](https://img.shields.io/badge/HDR10-suportado-orange)

**[⚡ Instalação](#-instalação)** · **[✨ Recursos](#-recursos)** · **[💻 Requisitos](#-requisitos-do-sistema)** · **[🛠️ Compilar](#️-compilar-o-projeto)** · **[🙏 Créditos](#-créditos)**

</div>

---

## 🎯 O que é isso?

Um **port nativo para PC** da versão de Xbox original de *BLACK*, feito por **recompilação estática**: o jogo deixa de depender do console e passa a rodar como um programa de Windows, com opções que o Xbox nunca teve.

> [!IMPORTANT]
> Este projeto **não inclui nenhum arquivo do jogo**. Você precisa fornecer os arquivos da **sua própria cópia, obtida legalmente**, para instalar ou compilar.

| 🎮 Antes (Xbox) | 🚀 Agora (PC) |
| --- | --- |
| Resolução fixa de 640x480 | Resolução nativa do seu monitor |
| Limitador de 30 FPS | Taxa de quadros livre ou personalizada |
| Controle apenas | Teclado, mouse e controle |
| Sem HDR | Saída HDR10 |

---

## 📦 Instalação

1. 📂 Coloque os arquivos do jogo na pasta `assets`. Pode ser uma **ISO** ou os **arquivos já extraídos**, da versão **USA** ou **Europa**.
2. ▶️ Execute o `BLACK.exe`.
3. ⚙️ Ajuste as opções no **menu do próprio jogo** enquanto joga, ou pelo **overlay de configurações**, aberto com **`F10`** por padrão.

---

## ✨ Recursos

<details open>
<summary><b>🖥️ Tela</b></summary>

<br>

| Opção | O que faz |
| --- | --- |
| **Monitor** | Escolhe em qual monitor o jogo aparece, em Tela cheia e Sem bordas (e onde o modo Janela abre). Lista cada monitor conectado pelo número do Windows e pela resolução da área de trabalho. |
| **Modo de exibição** | Alterna entre **Tela cheia**, **Sem bordas** e **Janela**. |
| **Resolução** | Lista todos os modos que o seu monitor informa e usa por padrão a resolução da sua área de trabalho, no lugar dos 640x480 originais. |
| **Resolução de renderização** | Renderiza o jogo de **20% a 200%** da resolução de saída, permitindo supersampling ou downscaling independente do tamanho da janela. |
| **Campo de visão (FOV)** | Define o FOV horizontal durante o jogo, de **45 a 140 graus** (o padrão do jogo é 70). |
| **FOV da arma** | Ajusta o campo de visão da arma e dos braços em primeira pessoa. |
| **Taxa máxima de quadros** | Limita ao refresh do monitor, a um valor personalizado, ou remove o limite, substituindo o limitador de 30 FPS do Xbox. |
| **V-Sync** | Reduz o rasgo de tela (tearing). |
| **Saída HDR** | Ativa HDR10 em telas com o HDR do Windows ligado, detectado automaticamente. Os brilhos chegam até o pico da tela. |
| **Contador de FPS** | Mostra a taxa de quadros na tela. |
| **Escala dos FMVs** | **Preencher** dá zoom nos vídeos 4:3 para cobrir telas widescreen. **4:3** mantém a proporção original. |

</details>

<details open>
<summary><b>🎨 Gráficos</b></summary>

<br>

| Opção | O que faz |
| --- | --- |
| **MSAA** | Antialiasing multiamostra em **2x, 4x ou 8x**, suavizando serrilhados e mantendo a imagem nítida. |
| **SMAA** | Antialiasing morfológico de subpixel, que suaviza o quadro inteiro com uma imagem mais macia. Também trata bordas com alpha test (cercas, folhagens) e **pode ser combinado com o MSAA**. |
| **Filtragem anisotrópica** | Força o nível escolhido em todas as texturas. |
| **Distância de renderização** | Aumenta o nível de detalhe e as distâncias de desenho além dos valores do jogo: **2x, 4x ou 8x**. |
| **Oclusão de ambiente** | Adiciona ambient occlusion em espaço de tela, criando sombras de contato suaves onde as superfícies se encontram. Escolha entre **SSAO** e **GTAO**. |
| **Desfoque ao recarregar** | Liga ou desliga o efeito de blur durante a recarga. |

</details>

<details open>
<summary><b>🕹️ Controles</b></summary>

<br>

- ⌨️🖱️ **Teclado e mouse:** suporte completo com raw input, sensibilidade ajustável, inversão de olhar e **teclas reconfiguráveis**.
- 🎮 **Controle:** suporte com **SDL3**.

</details>

<details open>
<summary><b>⚙️ Geral e extras</b></summary>

<br>

- ⏭️ **Pular intro:** pula os logos de abertura.
- ⏸️ **Pausar ao perder o foco:** pausa o jogo e o som quando a janela está em segundo plano ou minimizada.
- 🖱️ **Cursor personalizado:** coloque um `cursor.png` (ou `cursor.dds`) ao lado do executável para trocar a seta do Windows nos menus do jogo.

</details>

---

## 💻 Requisitos do sistema

### ✅ Mínimo

| Componente | Requisito |
| --- | --- |
| 🪟 **Sistema** | Windows 10 64-bit |
| 🧠 **CPU** | 2 núcleos com suporte a **SSE4.2** e **POPCNT**<br>Intel Nehalem (Intel Core 1ª geração) ou AMD Bulldozer (série AMD FX) |
| 🎮 **GPU** | Suporte a **Direct3D 12**<br>NVIDIA GeForce GT 630 (Kepler), AMD Radeon HD 7750 ou Intel HD Graphics 510 (Skylake) |
| 💾 **Memória** | 4 GB |
| 📀 **Armazenamento** | 2 GB para os arquivos do jogo e saves |

---

## 🛠️ Compilar o projeto

### 1️⃣ Clone o repositório

Use o [Git](https://git-scm.com/):

```bash
git clone https://github.com/lordjunnior/BLACK-GamePC.git
```

### 2️⃣ Adicione os arquivos do jogo

Coloque os dados extraídos do jogo na pasta `assets`. O `default.xbe` da versão **USA** precisa estar lá, junto com o restante dos arquivos do jogo.

### 3️⃣ Instale as dependências

Instale o [Visual Studio 2022](https://visualstudio.microsoft.com/downloads/) e selecione estas **Cargas de trabalho** e **Componentes individuais**:

- Desenvolvimento para desktop com C++
- Ferramentas C++ Clang para Windows
- Ferramentas C++ CMake para Windows

> [!TIP]
> O `build.bat` oferece instalar os componentes Clang e CMake para você, caso estejam faltando.

### 4️⃣ Compile

1. Execute o `build.bat`.
2. Ao terminar, rode `out\build\release\BLACK.exe`.

> [!NOTE]
> ⏱️ A primeira compilação **recompila o jogo inteiro** e pode levar de **30 a 90 minutos** em máquinas mais fracas.

---

## 🙏 Créditos

| Projeto | Contribuição |
| --- | --- |
| **[BLACK-XBERecomp](https://github.com/TGP482/BLACK-XBERecomp)** por **TGP482** | Projeto original em que este port se baseia. |
| **[Xbox XBE Recomp](https://github.com/TGP482/XboxXBE-Recomp)** | Ferramenta de recompilação usada para criar o port. |

💬 Comunidade do projeto original: [discord.gg/8dAn4ZSsap](https://discord.gg/8dAn4ZSsap)

---

<div align="center">

<sub>🔫 Mantido por <b>Lord Junnior</b> | LordGames · Tradução e adaptação para o português do Brasil.</sub>

</div>
