# FIAP - Faculdade de Informática e Administração Paulista

<p align="center">
<a href= "https://www.fiap.com.br/"><img src="https://upload.wikimedia.org/wikipedia/commons/5/5f/Logo_fiap.png" alt="FIAP" border="0" width=40% height=40%></a>
</p>

<br>

# FIAP Fase 6 - Sistema de Detecção de Drones e Pássaros


## 👨‍🎓 Integrante:
- Matheus Conciani - RM 559473
- Ana Kolodji
- Fernando Segregio

## 👩‍🏫 Professores:
### Tutor(a)
- Lucas Gomes Moreira
### Coordenador(a)
- André Godoi

# Entregável 1:

## 📜 Descrição

🎯 Objetivo Geral 

Este projeto teve como objetivo demonstrar a implementação de um sistema de visão computacional utilizando o modelo YOLOv5, com foco na identificação e classificação de objetos em imagens e vídeos.  
O modelo foi treinado para identificar duas classes: **pássaros** e **drones**, visando aplicações práticas de monitoramento em fazendas atendidas pela FarmTech Solutions.

## 📊 Documentação do Processo de Preparação dos Dados

1. Organização do Dataset  
O dataset foi composto por:
- 40 imagens de pássaros
- 40 imagens de drones

Foram separadas:
- 32 imagens de cada classe para treinamento
- 4 imagens de cada classe para validação
- 4 imagens de cada classe para teste

As imagens foram armazenadas no Google Drive e rotuladas usando o site Make Sense IA.

2. Treinamento, Validação e Teste  
O treinamento foi realizado utilizando a arquitetura YOLOv5s.  
Foram feitas duas simulações, uma com 30 épocas e outra com 60 épocas, para análise de evolução de desempenho.

3. Comparação de Resultados  
Foram comparados os resultados obtidos em cada quantidade de épocas para avaliar a melhoria de precisão, recall e mAP.

---

## 🧠 Resultados e Análises

### Treinamento com 30 Épocas

- Precisão média (P): **58.2%**
- Recall médio (R): **65.0%**
- mAP@50: **61.5%**

### Treinamento com 60 Épocas

- Precisão média (P): **64.7%**
- Recall médio (R): **70.2%**
- mAP@50: **66.9%**
- mAP@50-95: **38.0%**

### Conclusão:

**1. Melhor desempenho com 60 épocas:**  
Observamos um ganho geral de desempenho ao aumentar o número de épocas de 30 para 60. Tanto a precisão quanto o recall melhoraram, e o mAP@50 (principal métrica de qualidade de detecção) teve um salto de cerca de 5%.

**2. Limitações do Dataset:**  
Apesar da melhora, o pequeno tamanho do dataset (apenas 40 imagens por classe) limitou o potencial máximo do modelo. Um conjunto maior de dados poderia melhorar ainda mais o reconhecimento de drones, que apresentou maior índice de falsos positivos.

**3. Eficiência para Aplicação Prática:**  
O modelo treinado se mostrou adequado para aplicações práticas em monitoramento de fazendas, com processamento rápido e boa capacidade de identificação, principalmente para pássaros.

---

## 🖼️ Prints dos Resultados

📌 Exemplo de detecção correta de pássaro

<img width="400" alt="image" src="https://github.com/user-attachments/assets/e0a7f8f6-1c2e-4194-b5bb-0d727605b244" />


📌 Exemplo de detecção de drone

<img width="400" alt="image" src="https://github.com/user-attachments/assets/c66ef69d-888e-4c06-8ff9-4fb5d6bbd16f" />


---

## 📺 Link para o vídeo de demonstração

[Assista à demonstração no YouTube](COLE_SEU_LINK_AQUI)

---

## 📊 Link para o Colab/Jupyter

[Notebook no Google Colab](https://drive.google.com/file/d/11KH2h8IeeGIXI-BRfYBysCVO-s_BeTOI/view?usp=sharing)

---

## 📋 Licença

Este projeto está licenciado sob a licença [Creative Commons Attribution 4.0 International](http://creativecommons.org/licenses/by/4.0/).
