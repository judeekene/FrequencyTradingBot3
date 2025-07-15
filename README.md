## 📈 High-Low Ratio Strategy Bot (C#)

A momentum-based trading algorithm that leverages **high-low ratios** and **moving average crossovers** to identify optimal trade entry points across multiple symbols.

### 🚦 Strategy Overview
This bot analyses price movements by comparing the frequency of daily **higher highs** and **lower lows** over a rolling window, then smooths this using moving averages:

- Calculates a **high-low ratio score** over ~5 weeks of market data  
- Applies **short-term and long-term moving averages** to that ratio  
- Generates trades based on **crossover conditions** and ratio thresholds  

Symbols and configuration are fully customizable.

---

### 🧩 Technology Stack

| Component       | Role                                 |
|----------------|--------------------------------------|
| **C#**          | Strategy logic and data processing   |
| **MarketData API** | Timeframe and symbol bars        |

---

### 🚀 Features

- ⏱ Daily time frame analysis over ~5 weeks (260 bars)  
- 📊 Dynamic volume and MA period parameters  
- 💹 Automated order execution based on signal strength

---

### 💡 Sample Logic Snippet

Here’s a glimpse into how ratio scores are generated:

```csharp
double ratio = (newHighs + newLows) > 0 
    ? (newHighs / (newHighs + newLows) * 100) 
    : 50; // Neutral default
```

More logic available on request or via demo!

---

### 🛡️ License & Disclosure

This strategy is shared under the **MIT License** — feel free to explore or collaborate, but proprietary execution logic is selectively withheld to protect original work.

> 📧 Contact me for walkthroughs, collaboration, or live testing opportunities:  
[mailto:your.email@example.com](mailto:judeekene@gmail.com)

---
