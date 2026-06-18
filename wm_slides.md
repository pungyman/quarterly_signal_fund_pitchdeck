---
theme: default
title: Quarterly Signal Fund · Wealth Management Portfolios
info: Quarterly Signal Fund - Wealth Management Portfolios (7 / 13 / 16 stock variants)
class: text-center
drawings:
  persist: false
transition: slide-left
mdc: true
fonts:
  sans: Inter
  mono: Fira Code
lineNumbers: false
---

<div class="h-full flex flex-col items-center justify-center">
  <h1 class="!text-7xl !font-extrabold !border-none !pb-0 !mb-0" style="color: #303192;">Quarterly Signal Fund</h1>
  <div class="mt-4 text-2xl font-semibold text-gray-500 tracking-wide">Wealth Management Portfolios</div>
</div>

---
layout: default
---

# Model Training Methodology

<p class="text-sm text-gray-500 mb-2">An adaptive 10-year window slides forward one prediction year at a time — retraining annually keeps the model dynamic and continually adapting to changing market conditions</p>

<div class="mx-4 mt-1">
  <div class="flex items-center gap-4 mb-3 ml-[52px] text-[0.7rem]">
    <span class="flex items-center gap-1.5"><span class="inline-block w-3 h-3 rounded-sm bg-[#303192]"></span> <span class="text-gray-500">Training Window (10 yrs)</span></span>
    <span class="flex items-center gap-1.5"><span class="inline-block w-3 h-3 rounded-sm bg-[#e85d75]"></span> <span class="text-gray-500">Prediction Year</span></span>
  </div>

  <div class="flex items-end gap-2 mb-1.5">
    <div class="w-[48px] shrink-0"></div>
    <div class="flex-1 relative h-5 border-b border-gray-200">
      <span class="absolute bottom-0.5 text-[0.6rem] text-gray-400 -translate-x-1/2" style="left: 2.63%;">2007</span>
      <span class="absolute bottom-0.5 text-[0.6rem] text-gray-400 -translate-x-1/2" style="left: 18.42%;">'10</span>
      <span class="absolute bottom-0.5 text-[0.6rem] text-gray-400 -translate-x-1/2" style="left: 34.21%;">'13</span>
      <span class="absolute bottom-0.5 text-[0.6rem] text-gray-400 -translate-x-1/2" style="left: 50%;">'16</span>
      <span class="absolute bottom-0.5 text-[0.6rem] text-gray-400 -translate-x-1/2" style="left: 65.79%;">'19</span>
      <span class="absolute bottom-0.5 text-[0.6rem] text-gray-400 -translate-x-1/2" style="left: 81.58%;">'22</span>
      <span class="absolute bottom-0.5 text-[0.6rem] text-gray-400 -translate-x-1/2" style="left: 97.37%;">2025</span>
    </div>
  </div>

  <div class="space-y-1">
    <div class="flex items-center gap-2">
      <div class="w-[48px] shrink-0 text-right text-[0.7rem] font-semibold text-[#303192] tabular-nums">Set 1</div>
      <div class="flex-1 relative h-7">
        <div class="absolute inset-y-0 rounded bg-[#303192] flex items-center justify-center" style="left: 0%; width: 52.63%;"><span class="text-white text-[0.65rem]">2007 – 2016</span></div>
        <div class="absolute inset-y-0 rounded bg-[#e85d75] flex items-center justify-center" style="left: 52.63%; width: 5.26%;"><span class="text-white text-[0.5rem] font-bold">'17</span></div>
      </div>
    </div>
    <div v-click class="flex items-center gap-2">
      <div class="w-[48px] shrink-0 text-right text-[0.7rem] font-semibold text-[#303192] tabular-nums">Set 2</div>
      <div class="flex-1 relative h-7">
        <div class="absolute inset-y-0 rounded bg-[#303192] flex items-center justify-center" style="left: 5.26%; width: 52.63%;"><span class="text-white text-[0.65rem]">2008 – 2017</span></div>
        <div class="absolute inset-y-0 rounded bg-[#e85d75] flex items-center justify-center" style="left: 57.89%; width: 5.26%;"><span class="text-white text-[0.5rem] font-bold">'18</span></div>
      </div>
    </div>
    <div v-click class="flex items-center gap-2">
      <div class="w-[48px] shrink-0 text-right text-[0.7rem] font-semibold text-[#303192] tabular-nums">Set 3</div>
      <div class="flex-1 relative h-7">
        <div class="absolute inset-y-0 rounded bg-[#303192] flex items-center justify-center" style="left: 10.53%; width: 52.63%;"><span class="text-white text-[0.65rem]">2009 – 2018</span></div>
        <div class="absolute inset-y-0 rounded bg-[#e85d75] flex items-center justify-center" style="left: 63.16%; width: 5.26%;"><span class="text-white text-[0.5rem] font-bold">'19</span></div>
      </div>
    </div>
    <div v-click>
      <div class="flex items-center gap-2 h-5">
        <div class="w-[48px] shrink-0"></div>
        <div class="flex-1 text-center text-gray-400 text-sm tracking-[0.3em]">···</div>
      </div>
      <div class="flex items-center gap-2 mt-1">
        <div class="w-[48px] shrink-0 text-right text-[0.7rem] font-semibold text-[#303192] tabular-nums">Set 9</div>
        <div class="flex-1 relative h-7">
          <div class="absolute inset-y-0 rounded bg-[#303192] flex items-center justify-center" style="left: 42.11%; width: 52.63%;"><span class="text-white text-[0.65rem]">2015 – 2024</span></div>
          <div class="absolute inset-y-0 rounded bg-[#e85d75] flex items-center justify-center" style="left: 94.74%; width: 5.26%;"><span class="text-white text-[0.5rem] font-bold">'25</span></div>
        </div>
      </div>
    </div>
  </div>
</div>

<div v-click class="mx-4 mt-8 p-3 rounded-xl bg-[#303192]/8 border border-[#303192]/15">
<span class="font-bold text-[#303192]">Adaptive &amp; Dynamic</span>
<span class="text-[0.85rem] ml-2">Each window produces fresh probability scores for every NIFTY 500 stock, so the signal stays current as markets shift instead of being locked to one historical regime.</span>
</div>

---
layout: default
---

# Portfolio Concentration Variants

<p class="text-sm text-gray-500 mb-2">One signal engine, four levels of portfolio breadth — choose your risk / return profile</p>

<div class="grid grid-cols-4 gap-4 w-full mt-4">
  <div class="p-4 rounded-xl bg-[#303192]/8 border border-[#303192]/15 text-center">
    <div class="text-4xl font-extrabold text-[#303192]">7</div>
    <div class="text-sm font-semibold text-gray-600 mb-3">stocks · Concentrated</div>
    <div class="text-[0.8rem] text-gray-500">CAGR <span class="font-bold text-[#303192]">18.1%</span></div>
  </div>
  <div class="p-4 rounded-xl bg-[#303192]/8 border border-[#303192]/15 text-center">
    <div class="text-4xl font-extrabold text-[#303192]">13</div>
    <div class="text-sm font-semibold text-gray-600 mb-3">stocks · Balanced</div>
    <div class="text-[0.8rem] text-gray-500">CAGR <span class="font-bold text-[#303192]">19.7%</span></div>
  </div>
  <div class="p-4 rounded-xl bg-[#303192]/8 border border-[#303192]/15 text-center">
    <div class="text-4xl font-extrabold text-[#303192]">16</div>
    <div class="text-sm font-semibold text-gray-600 mb-3">stocks · Growth</div>
    <div class="text-[0.8rem] text-gray-500">CAGR <span class="font-bold text-[#303192]">21.7%</span></div>
  </div>
  <div class="p-4 rounded-xl bg-[#303192]/8 border border-[#303192]/15 text-center">
    <div class="text-4xl font-extrabold text-[#303192]">20</div>
    <div class="text-sm font-semibold text-gray-600 mb-3">stocks · Diversified</div>
    <div class="text-[0.8rem] text-gray-500">CAGR <span class="font-bold text-[#303192]">21.1%</span></div>
  </div>
</div>

<div class="mt-5 flex items-center justify-between gap-2 text-[0.72rem] font-semibold">
  <div class="flex-1 text-center py-2 px-1 rounded-lg bg-[#303192] text-white">Concentrated → Higher per-name conviction</div>
  <div class="text-[#303192] text-lg">·</div>
  <div class="flex-1 text-center py-2 px-1 rounded-lg bg-[#4545b8] text-white">Balanced → Best risk-adjusted</div>
  <div class="text-[#303192] text-lg">·</div>
  <div class="flex-1 text-center py-2 px-1 rounded-lg bg-[#5050cb] text-white">Growth → Highest return</div>
  <div class="text-[#303192] text-lg">·</div>
  <div class="flex-1 text-center py-2 px-1 rounded-lg bg-[#5a5bd4] text-white">Diversified → Broadest exposure</div>
</div>

<div class="mt-6 p-3 rounded-xl bg-[#303192]/8 border border-[#303192]/15">
<span class="font-bold text-[#303192]">Key Innovation</span>
<div class="mt-1 text-[0.85rem] italic opacity-90">
The ML model predicts <span class="font-bold not-italic text-[#303192]">relative</span> outperformance vs. the market — not absolute returns.<br>
Combined with a  <span class="font-bold not-italic text-[#303192]">fundamentals-for-entry</span>, <span class="font-bold not-italic text-[#303192]">technicals-for-exit</span> approach to limit downside.
</div>
</div>

<div class="mt-3 text-left text-[0.7rem] text-gray-400"><span class="font-semibold">Note:</span> CAGR figures correspond to period 2017–2026</div>

---
layout: default
---

# 7-Stock Portfolio

<div class="h-[78%] flex flex-col items-center justify-center gap-6 -mt-2">
  <div class="text-center">
    <div class="text-sm uppercase tracking-[0.25em] text-[#303192]/70 font-bold mb-3">Concentrated</div>
    <div class="text-5xl font-extrabold text-[#303192] leading-tight">Highest Conviction, Fewest Names</div>
    <div class="mt-3 text-lg text-gray-600">A tightly concentrated multi-cap variant of the quarterly signal portfolio</div>
  </div>

  <div class="grid grid-cols-3 gap-4 w-full max-w-[850px] text-center">
    <div class="p-4 rounded-xl bg-[#303192]/8 border border-[#303192]/15">
      <div class="text-3xl font-extrabold text-[#303192]">18.1%</div>
      <div class="text-sm font-semibold text-gray-600">annualised return</div>
    </div>
    <div class="p-4 rounded-xl bg-[#303192]/8 border border-[#303192]/15">
      <div class="text-3xl font-extrabold text-[#303192]">-20.0%</div>
      <div class="text-sm font-semibold text-gray-600">max drawdown</div>
    </div>
    <div class="p-4 rounded-xl bg-[#303192]/8 border border-[#303192]/15">
      <div class="text-3xl font-extrabold text-[#303192]">+4.1%</div>
      <div class="text-sm font-semibold text-gray-600">return p.a. vs NIFTY 500</div>
    </div>
  </div>
</div>

---
layout: default
---

# 7-Stock · Performance

<div class="grid grid-cols-[2fr_1fr] gap-4 items-center h-[82%]">
  <img src="/images/wm7_wealth.png" class="max-h-[430px] rounded-lg shadow-lg" />
  <img src="/images/wm7_calendar.png" class="max-h-[430px] rounded-lg shadow-lg" />
</div>

---
layout: default
---

# 7-Stock · Performance Summary

<div class="text-sm mb-3">
Trailing Returns (%) as of <strong>May 29, 2026</strong> · Backtest period: <strong>2017–2026</strong> (9 years)
</div>

<v-click>
<div class="mb-5">
<p class="table-label">Trailing Returns (%)</p>

| | 1 mo | 3 mo | 6 mo | 1 year | 3 years | 5 years |
|---|---:|---:|---:|---:|---:|---:|
| **7-Stock** | 1.01 | -8.13 | -1.68 | 12.23 | 19.75 | 21.06 |
| **NIFTY 500 TRI** | -0.37 | -3.00 | -4.50 | 1.30 | 14.66 | 13.73 |

</div>
</v-click>

<v-click>
<div>
<p class="table-label">Key Metrics</p>

| | Ann. Return | Ann. Risk | Max. Drawdown |
|---|---:|---:|---:|
| **7-Stock** | 18.14% | 11.20% | -20.01% |
| **NIFTY 500 TRI** | 14.09% | 16.38% | -38.11% |

</div>
</v-click>

<v-click>
<div class="mt-3 flex gap-4 justify-center text-sm">
  <div class="callout-badge callout-green">+4.1% return p.a. vs NIFTY 500</div>
  <div class="callout-badge callout-green">lower volatility</div>
  <div class="callout-badge callout-green">half the max drawdown</div>
</div>
</v-click>

---
layout: default
---

# 7-Stock · Monthly Returns Profile

<div class="flex justify-center items-center h-[75%] mt-8">
  <img src="/images/wm7_monthly.png" class="max-h-[400px] rounded-lg shadow-lg" />
</div>

---
layout: default
---

# 13-Stock Portfolio

<div class="h-[78%] flex flex-col items-center justify-center gap-6 -mt-2">
  <div class="text-center">
    <div class="text-sm uppercase tracking-[0.25em] text-[#303192]/70 font-bold mb-3">Balanced</div>
    <div class="text-5xl font-extrabold text-[#303192] leading-tight">The Best Risk-Adjusted Variant</div>
    <div class="mt-3 text-lg text-gray-600">Lowest volatility and shallowest drawdown of the three portfolios</div>
  </div>

  <div class="grid grid-cols-3 gap-4 w-full max-w-[850px] text-center">
    <div class="p-4 rounded-xl bg-[#303192]/8 border border-[#303192]/15">
      <div class="text-3xl font-extrabold text-[#303192]">19.7%</div>
      <div class="text-sm font-semibold text-gray-600">annualised return</div>
    </div>
    <div class="p-4 rounded-xl bg-[#303192]/8 border border-[#303192]/15">
      <div class="text-3xl font-extrabold text-[#303192]">1.46</div>
      <div class="text-sm font-semibold text-gray-600">Sharpe ratio</div>
    </div>
    <div class="p-4 rounded-xl bg-[#303192]/8 border border-[#303192]/15">
      <div class="text-3xl font-extrabold text-[#303192]">-17.2%</div>
      <div class="text-sm font-semibold text-gray-600">max drawdown</div>
    </div>
  </div>
</div>

---
layout: default
---

# 13-Stock · Performance

<div class="grid grid-cols-[2fr_1fr] gap-4 items-center h-[82%]">
  <img src="/images/wm13_wealth.png" class="max-h-[430px] rounded-lg shadow-lg" />
  <img src="/images/wm13_calendar.png" class="max-h-[430px] rounded-lg shadow-lg" />
</div>

---
layout: default
---

# 13-Stock · Performance Summary

<div class="text-sm mb-3">
Trailing Returns (%) as of <strong>May 29, 2026</strong> · Backtest period: <strong>2017–2026</strong> (9 years)
</div>

<v-click>
<div class="mb-5">
<p class="table-label">Trailing Returns (%)</p>

| | 1 mo | 3 mo | 6 mo | 1 year | 3 years | 5 years |
|---|---:|---:|---:|---:|---:|---:|
| **13-Stock** | -1.10 | -5.82 | -0.45 | 9.20 | 18.44 | 19.26 |
| **NIFTY 500 TRI** | -0.37 | -3.00 | -4.50 | 1.30 | 14.66 | 13.73 |

</div>
</v-click>

<v-click>
<div>
<p class="table-label">Key Metrics</p>

| | Ann. Return | Ann. Risk | Max. Drawdown |
|---|---:|---:|---:|
| **13-Stock** | 19.73% | 9.05% | -17.21% |
| **NIFTY 500 TRI** | 14.09% | 16.38% | -38.11% |

</div>
</v-click>

<v-click>
<div class="mt-3 flex gap-4 justify-center text-sm">
  <div class="callout-badge callout-green">+5.6% return p.a. vs NIFTY 500</div>
  <div class="callout-badge callout-green">lowest volatility</div>
  <div class="callout-badge callout-green">best Sharpe (1.46)</div>
</div>
</v-click>

---
layout: default
---

# 13-Stock · Monthly Returns Profile

<div class="flex justify-center items-center h-[75%] mt-8">
  <img src="/images/wm13_monthly.png" class="max-h-[400px] rounded-lg shadow-lg" />
</div>

---
layout: default
---

# 16-Stock Portfolio

<div class="h-[78%] flex flex-col items-center justify-center gap-6 -mt-2">
  <div class="text-center">
    <div class="text-sm uppercase tracking-[0.25em] text-[#303192]/70 font-bold mb-3">Growth</div>
    <div class="text-5xl font-extrabold text-[#303192] leading-tight">Maximum Growth & Alpha</div>
    <div class="mt-3 text-lg text-gray-600">The highest-returning variant — strongest absolute growth and market outperformance</div>
  </div>

  <div class="grid grid-cols-3 gap-4 w-full max-w-[850px] text-center">
    <div class="p-4 rounded-xl bg-[#303192]/8 border border-[#303192]/15">
      <div class="text-3xl font-extrabold text-[#303192]">21.7%</div>
      <div class="text-sm font-semibold text-gray-600">annualised return</div>
    </div>
    <div class="p-4 rounded-xl bg-[#303192]/8 border border-[#303192]/15">
      <div class="text-3xl font-extrabold text-[#303192]">+7.6%</div>
      <div class="text-sm font-semibold text-gray-600">return p.a. vs NIFTY 500</div>
    </div>
    <div class="p-4 rounded-xl bg-[#303192]/8 border border-[#303192]/15">
      <div class="text-3xl font-extrabold text-[#303192]">0.77</div>
      <div class="text-sm font-semibold text-gray-600">benchmark correlation</div>
    </div>
  </div>
</div>

---
layout: default
---

# 16-Stock · Performance

<div class="grid grid-cols-[2fr_1fr] gap-4 items-center h-[82%]">
  <img src="/images/wm16_wealth.png" class="max-h-[430px] rounded-lg shadow-lg" />
  <img src="/images/wm16_calendar.png" class="max-h-[430px] rounded-lg shadow-lg" />
</div>

---
layout: default
---

# 16-Stock · Performance Summary

<div class="text-sm mb-3">
Trailing Returns (%) as of <strong>May 29, 2026</strong> · Backtest period: <strong>2017–2026</strong> (9 years)
</div>

<v-click>
<div class="mb-5">
<p class="table-label">Trailing Returns (%)</p>

| | 1 mo | 3 mo | 6 mo | 1 year | 3 years | 5 years |
|---|---:|---:|---:|---:|---:|---:|
| **16-Stock** | -1.27 | -5.14 | -1.36 | 10.11 | 17.95 | 19.98 |
| **NIFTY 500 TRI** | -0.37 | -3.00 | -4.50 | 1.30 | 14.66 | 13.73 |

</div>
</v-click>

<v-click>
<div>
<p class="table-label">Key Metrics</p>

| | Ann. Return | Ann. Risk | Max. Drawdown |
|---|---:|---:|---:|
| **16-Stock** | 21.66% | 13.13% | -26.42% |
| **NIFTY 500 TRI** | 14.09% | 16.38% | -38.11% |

</div>
</v-click>

<v-click>
<div class="mt-3 flex gap-4 justify-center text-sm">
  <div class="callout-badge callout-green">highest annualised return</div>
  <div class="callout-badge callout-green">+7.6% return p.a. vs NIFTY 500</div>
  <div class="callout-badge callout-green">shallower drawdown than index</div>
</div>
</v-click>

---
layout: default
---

# 16-Stock · Monthly Returns Profile

<div class="flex justify-center items-center h-[75%] mt-8">
  <img src="/images/wm16_monthly.png" class="max-h-[400px] rounded-lg shadow-lg" />
</div>

---
layout: default
---

# 20-Stock Portfolio

<div class="h-[78%] flex flex-col items-center justify-center gap-6 -mt-2">
  <div class="text-center">
    <div class="text-sm uppercase tracking-[0.25em] text-[#303192]/70 font-bold mb-3">Diversified</div>
    <div class="text-5xl font-extrabold text-[#303192] leading-tight">Broadest Exposure, Most Names</div>
    <div class="mt-3 text-lg text-gray-600">The most diversified variant — widest holding base for institution-friendly breadth</div>
  </div>

  <div class="grid grid-cols-3 gap-4 w-full max-w-[850px] text-center">
    <div class="p-4 rounded-xl bg-[#303192]/8 border border-[#303192]/15">
      <div class="text-3xl font-extrabold text-[#303192]">21.1%</div>
      <div class="text-sm font-semibold text-gray-600">annualised return</div>
    </div>
    <div class="p-4 rounded-xl bg-[#303192]/8 border border-[#303192]/15">
      <div class="text-3xl font-extrabold text-[#303192]">+7.0%</div>
      <div class="text-sm font-semibold text-gray-600">return p.a. vs NIFTY 500</div>
    </div>
    <div class="p-4 rounded-xl bg-[#303192]/8 border border-[#303192]/15">
      <div class="text-3xl font-extrabold text-[#303192]">0.73</div>
      <div class="text-sm font-semibold text-gray-600">benchmark correlation</div>
    </div>
  </div>
</div>

---
layout: default
---

# 20-Stock · Performance

<div class="grid grid-cols-[2fr_1fr] gap-4 items-center h-[82%]">
  <img src="/images/wm20_wealth.png" class="max-h-[430px] rounded-lg shadow-lg" />
  <img src="/images/wm20_calendar.png" class="max-h-[430px] rounded-lg shadow-lg" />
</div>

---
layout: default
---

# 20-Stock · Performance Summary

<div class="text-sm mb-3">
Trailing Returns (%) as of <strong>May 29, 2026</strong> · Backtest period: <strong>2017–2026</strong> (9 years)
</div>

<v-click>
<div class="mb-5">
<p class="table-label">Trailing Returns (%)</p>

| | 1 mo | 3 mo | 6 mo | 1 year | 3 years | 5 years |
|---|---:|---:|---:|---:|---:|---:|
| **20-Stock** | -0.65 | -6.89 | -1.92 | -0.13 | 15.13 | 21.71 |
| **NIFTY 500 TRI** | -0.37 | -3.00 | -4.50 | 1.30 | 14.66 | 13.73 |

</div>
</v-click>

<v-click>
<div>
<p class="table-label">Key Metrics</p>

| | Ann. Return | Ann. Risk | Max. Drawdown |
|---|---:|---:|---:|
| **20-Stock** | 21.10% | 13.48% | -30.92% |
| **NIFTY 500 TRI** | 14.09% | 16.38% | -38.11% |

</div>
</v-click>

<v-click>
<div class="mt-3 flex gap-4 justify-center text-sm">
  <div class="callout-badge callout-green">20 holdings · broadest exposure</div>
  <div class="callout-badge callout-green">+7.0% return p.a. vs NIFTY 500</div>
  <div class="callout-badge callout-green">21.7% 5-year return</div>
</div>
</v-click>

---
layout: default
---

# 20-Stock · Monthly Returns Profile

<div class="flex justify-center items-center h-[75%] mt-8">
  <img src="/images/wm20_monthly.png" class="max-h-[400px] rounded-lg shadow-lg" />
</div>

---
layout: default
---

# Implementation Notes

<div class="h-[76%] flex flex-col justify-center gap-5">
  <div class="p-5 rounded-xl bg-[#303192]/8 border border-[#303192]/15">
    <div class="text-sm uppercase tracking-[0.2em] text-[#303192]/70 font-bold mb-3">7-Stock Portfolio</div>
    <div class="grid grid-cols-2 gap-5">
      <div>
        <div class="text-xl font-bold text-[#303192] mb-2">Churned Twice Every Quarter</div>
        <div class="text-gray-600">The concentrated 7-stock portfolio is churned twice every quarter to keep the holding set aligned with the latest signal output.</div>
      </div>
      <div>
        <div class="text-xl font-bold text-[#303192] mb-2">Aggressive TP / SL Discipline</div>
        <div class="text-gray-600">Aggressive target-profit and stop-loss rules are used as active risk-management controls to limit downside.</div>
      </div>
    </div>
  </div>

  <div class="p-5 rounded-xl bg-white border border-[#303192]/15 shadow-sm">
    <div class="text-sm uppercase tracking-[0.2em] text-[#303192]/70 font-bold mb-2">All Strategies</div>
    <div class="text-xl font-bold text-[#303192] mb-2">Cash Deployment Assumption</div>
    <div class="text-gray-600">Cash held after exiting positions is assumed to be invested in a liquid instrument, such as Liquid BeES, until it is redeployed into new signals.</div>
  </div>
</div>

---
layout: default
class: text-center
---

<div class="h-full flex flex-col items-center justify-center">
  <h1 class="!text-5xl !font-extrabold !border-none" style="color: #303192;">Thank You</h1>
</div>
