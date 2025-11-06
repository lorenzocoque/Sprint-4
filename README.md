# 🏆 Gerenciador de Placar Inteligente – Copa *Passa a Bola*

<p align="center">
  <img src="imagem_2025-09-16_171050116.png" alt="Logo Passa a Bola" width="500"/>
</p>

[![ESP32](https://img.shields.io/badge/ESP32-00979D?style=for-the-badge&logo=espressif&logoColor=white)](https://www.espressif.com/en/products/socs/esp32)  
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)  
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)  
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)  

---

## 👩‍💻 Integrantes

<p align="center">
  <span style="font-size:16px;">Enzo Ramos – RM: 563705 | Felipe Cerazi – RM: 562746 | Gustavo Peaguda – RM: 562923 | Lorenzo Coque – RM: 563385</span>
</p>

---

## 📖 Sobre o Projeto

O **Gerenciador de Placar Inteligente** é uma solução tecnológica desenvolvida para a **Copa Passa a Bola**, um campeonato amador de futebol feminino.  

O sistema foi projetado para integrar **hardware e software** de forma eficiente, automatizando o controle do placar e proporcionando uma experiência dinâmica e interativa.  

A solução conecta e integra:
- **ESP32 com botões simulados no Wokwi**  
- **Máquina virtual hospedada na Microsoft Azure**  
- **Ambiente de testes Postman**  
- **Notebook no Google Colab**  

🎯 **Objetivo principal:** permitir a atualização do placar em tempo real, controlando gols, cartões e tempo de jogo por meio de uma interface física com botões, de forma simples, confiável e responsiva.

---

### ⚡ Funcionalidades dos Botões

- 🟡 Adicionar ou remover **cartões amarelos**  
- 🔴 Adicionar ou remover **cartões vermelhos**  
- ⚽ Adicionar ou remover **gols da equipe A**  
- ⚽ Adicionar ou remover **gols da equipe B**  
- ⏱️ **Pausar, retomar ou reiniciar** o tempo de jogo  

---

## 🏗️ Arquitetura do Sistema

<p align="center">
  <img src="arquitetura_sistema.png" alt="Arquitetura do Sistema" width="600"/>
</p>

### 🔍 Explicação Detalhada

1. **ESP32 + Botões (Wokwi):** capta as ações físicas realizadas pelo usuário (como gols, cartões e tempo de jogo).  
2. **MQTT + Azure:** os eventos gerados pelo ESP32 são transmitidos via protocolo MQTT para uma máquina virtual na Azure, responsável pelo processamento e encaminhamento dos dados.  
3. **Google Colab (Python):** um script em Python recebe os dados, processa-os e atualiza dinamicamente a interface do placar desenvolvida em HTML e CSS.  
4. **Postman:** o arquivo `score atualizado.json` permite testar endpoints e validar a comunicação entre os serviços de forma modular.  

---

## 🛠️ Requisitos e Recursos Necessários

- 💻 Computador com acesso ao **Google Colab**  
- ☁️ Conexão com a **máquina virtual na Azure**  
- [🎮 Simulador **Wokwi ESP32**](https://wokwi.com/projects/442288825722106881)  
- 🧰 **Postman** com o arquivo `score atualizado.json` importado  
- 🌐 Navegador para visualização do placar em tempo real  

---

## ⚙️ Guia de Utilização

### 1️⃣ Simulação no Wokwi
1. Acesse o projeto no Wokwi: [Clique aqui](https://wokwi.com/projects/442288825722106881).  
2. Interaja com os botões virtuais para simular gols, cartões ou ações de controle do tempo.  

<p align="center">
  <img src="projeto_wokwi.png" alt="Projeto Wokwi" width="600"/>
</p>

---

### 2️⃣ Execução no Google Colab
1. Abra o arquivo `Untitled2.ipynb` no **Google Colab**.  
2. Execute as células para conectar o ambiente ao **ESP32** via **MQTT** e **endereço IP da Azure**.  
3. O placar será atualizado em tempo real conforme as interações realizadas nos botões.  

---

### 3️⃣ Testes no Postman
1. Importe o arquivo `score atualizado.json` no **Postman**.  
2. Utilize os endpoints disponíveis para testar eventos simulados e verificar logs de atualização.  

---

### 4️⃣ Visualização do Placar
A interface exibe, em tempo real:
- ⚽ Quantidade de gols por equipe  
- 🟡 e 🔴 Cartões amarelos e vermelhos  
- ⏱️ Estado atual do cronômetro (pausado, em andamento ou reiniciado)  

---

### 5️⃣ Demonstração em Vídeo
Confira o funcionamento completo do projeto no vídeo demonstrativo:  
🎬 [Assista no YouTube](https://youtu.be/FIKXscPuLE4)

---

## 🚀 Contribuições

Este projeto possui caráter **educacional e colaborativo**, desenvolvido com o propósito de aprendizado prático em integração de hardware, software e nuvem.  

Sinta-se à vontade para:
- 📚 Estudar o código e compreender a arquitetura  
- ✨ Propor aprimoramentos e melhorias de design  
- 🧩 Explorar novas possibilidades de integração  

---

> Desenvolvido com dedicação por **Enzo Ramos, Felipe Cerazi, Gustavo Peaguda e Lorenzo Coque** ⚽💻  
