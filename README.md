# 🍷 VinhariaAgnello - Monitoramento Inteligente de Adegas | DevPrime

Seja bem-vindo ao projeto **Sistema de Monitoramento Inteligente**, uma solução automatizada desenvolvida pelo grupo **DevPrime** para **monitoramento ambiental da Vinharia Agnello**, garantindo as **condições ideais de conservação de vinhos** com precisão e eficiência energética.

---

## 🚀 Tecnologias Utilizadas

<div style="display: flex; gap: 10px; align-items: center;">
  <img src="https://img.shields.io/badge/Arduino-00979D?style=for-the-badge&logo=Arduino&logoColor=white" alt="Arduino Badge"/>
  <img src="https://img.shields.io/badge/C_Language-00599C?style=for-the-badge&logo=c&logoColor=white" alt="C Language Badge"/>
  <img src="https://img.shields.io/badge/Wokwi%20Simulator-00DAA8?style=for-the-badge&logo=wokwi&logoColor=white" alt="Wokwi Badge"/>
</div>

---

## 🛠️ Componentes Utilizados

- 🌡️ **Sensor DHT11** – Leitura de temperatura e umidade  
- ☀️ **Sensor LDR (Fotocélula)** – Medição da intensidade luminosa  
- ⏰ **RTC DS1307** – Relógio de tempo real para manter data e hora mesmo sem energia  
- 💡 **LEDs RGB (Verde, Amarelo, Vermelho)** – Indicadores de status ambiental  
- 🔊 **Buzzer** – Alerta sonoro em situações críticas  
- 👁️ **Sensor PIR (Movimento)** – Economia de energia com acionamento automático do display LCD  
- 🖥️ **Display LCD 16x2 com I2C** – Exibição dos dados de monitoramento em tempo real  
- 💾 **EEPROM** – Registro histórico de anomalias ambientais

---

## 🍇 Objetivo do Projeto

Manter as **condições ideais de armazenamento de vinhos** é crucial para preservar aroma, sabor e qualidade. O **VinhaGuard** foi desenvolvido com esse propósito, controlando os seguintes parâmetros:

| Parâmetro      | Faixa Ideal           |
|----------------|------------------------|
| Temperatura    | 13°C a 14°C           |
| Umidade        | 60% a 80%             |
| Luminosidade   | Baixa (< 30%)         |

---

## 🎯 Funcionalidades

✅ **Leitura automática** e precisa de temperatura, umidade e luz  
✅ **Exibição em tempo real** dos dados com data e hora no LCD  
✅ **Alerta visual e sonoro** quando as condições saem da faixa ideal  
✅ **Gravação de anomalias** na EEPROM para análise histórica  
✅ **Economia de energia**: o LCD só acende quando há movimento na adega  
✅ **Inicialização temática** com animação personalizada para a vinharia

---

## 📊 Interface de Exibição (LCD)

- **Linha 1:** `Luz: XX% | T: XX.X°C`
- **Linha 2:** `U: XX.X% | HH:MM`

> A interface é acionada automaticamente ao detectar presença com o sensor PIR.

---

## 🔔 Sistema de Alerta

- 🟢 **LED Verde:** Tudo dentro dos padrões ideais  
- 🟡 **LED Amarelo:** 1 parâmetro fora da faixa segura  
- 🔴 **LED Vermelho + Buzzer:** 2 ou mais parâmetros fora dos limites → **risco ao vinho!**

---

## 🧠 Lógica Inteligente

- O sistema verifica alterações **a cada minuto**
- Apenas condições **fora do padrão** são registradas para **otimizar o uso da EEPROM**
- Ajustado para o fuso horário **UTC-3** (Brasil)

---

## 🧪 Simulação Online

🔗 Simule o projeto no Wokwi:

[![Simular no Wokwi]([https://img.shields.io/badge/Simular%20no-Wokwi-green?style=for-the-badge&logo=wokwi&logoColor=white](https://wokwi.com/projects/431407540931396609))](https://wokwi.com/)  


---

## 👨‍💻 Desenvolvido por

### 👥 Grupo DevPrime

- 💡 Focados em soluções práticas com automação
- 🤝 Colaborativo e orientado à preservação da qualidade

---

## 📂 Organização do Projeto

