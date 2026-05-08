---
theme: default
title: Quarterly Signal Fund
info: Quarterly Signal Fund - Systematic Quant Strategy Pitch Deck
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
</div>

---
layout: default
---

# Overview of Approach

<div class="mt-4"></div>

<div class="mb-5 flex items-center justify-between gap-2 text-[0.7rem] font-semibold">
  <div class="flex-1 text-center py-2 px-1 rounded-lg bg-[#303192] text-white">📊 Quarterly Filings</div>
  <div class="text-[#303192] text-lg">→</div>
  <div class="flex-1 text-center py-2 px-1 rounded-lg bg-[#3a3ba5] text-white">🤖 ML Signal</div>
  <div class="text-[#303192] text-lg">→</div>
  <div class="flex-1 text-center py-2 px-1 rounded-lg bg-[#4545b8] text-white">📉 Volatility based scoring</div>
  <div class="text-[#303192] text-lg">→</div>
  <div class="flex-1 text-center py-2 px-1 rounded-lg bg-[#5050cb] text-white">💼 Portfolio</div>
  <div class="text-[#303192] text-lg">→</div>
  <div class="flex-1 text-center py-2 px-1 rounded-lg bg-[#5a5bd4] text-white">🎯 ATR / S&R Exit</div>
</div>

<div class="space-y-4 text-left text-[0.9rem] leading-relaxed">

<v-click>

- ML models extract **signal from quarterly results** posted by **NIFTY 500** companies

</v-click>
<v-click>

- Positions entered across a 3-day entry phase **every quarter** after SEBI filing deadlines (45–60 days after quarter end)

</v-click>
<v-click>

- Model output scores combined with **historical volatility** to construct a **stock portfolio** emphasising low drawdowns

</v-click>
<v-click>

- **Exit strategy** uses take-profit / stop-loss

</v-click>
</div>

<v-click>
<div class="mt-6 p-3 rounded-xl bg-[#303192]/8 border border-[#303192]/15">
<span class="font-bold text-[#303192]">Key Innovation</span>
<div class="mt-1 text-[0.85rem] italic opacity-90">
The ML model predicts <span class="font-bold not-italic text-[#303192]">relative</span> outperformance vs. the market — not absolute returns.<br>
Combined with a  <span class="font-bold not-italic text-[#303192]">fundamentals-for-entry</span>, <span class="font-bold not-italic text-[#303192]">technicals-for-exit</span> approach to limit downside.
</div>
</div>
</v-click>

---
layout: default
---

# Rolling Window Training

<p class="text-sm text-gray-500 mb-2">10-year training window slides forward annually — no future data leakage</p>

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
<span class="font-bold text-[#303192]">Result</span>
<span class="text-[0.85rem] ml-2">Each window produces probability scores for every Nifty 500 stock in the prediction year</span>
</div>

---
layout: default
---

# Features used to Extract Signal

<p class="text-sm text-gray-500 mb-2">Feature distribution across categories</p>

<div class="flex justify-center items-center h-[75%]">
  <img src="/images/slide3_img0.png" class="max-h-[400px] rounded-lg shadow-lg" />
</div>

---
layout: default
---

# Outperform the Market : Strategy 1

<div class="h-full flex items-center justify-center -mt-4">
  <img src="/images/wealth_generation.png" class="max-h-[440px] rounded-xl shadow-lg" />
</div>

---
layout: default
---

# Strategy 1 · For Wealth Generation

<div class="grid grid-cols-[2fr_1fr] gap-4 items-center h-[82%]">
  <img src="/images/slide4_img0.png" class="max-h-[430px] rounded-lg shadow-lg" />
  <img src="/images/slide4_img1.png" class="max-h-[430px] rounded-lg shadow-lg" />
</div>

---
layout: default
---

# Strategy 1 · Performance Summary

<div class="text-sm mb-3">
Trailing Returns (%) as of <strong>February 13, 2026</strong> · Backtest period: <strong>2017–2026</strong> (9 years)
</div>

<v-click>
<div class="mb-5">
<p class="table-label">Trailing Returns (%)</p>

| | 1 mo | 3 mo | 6 mo | 1 year | 3 years | 5 years |
|---|---:|---:|---:|---:|---:|---:|
| **Strategy 1** | 0.22 | 1.66 | 1.23 | 9.03 | 20.36 | 23.36 |
| **NIFTY 500 TRI** | -0.60 | -2.09 | 3.62 | 8.65 | 17.29 | 15.53 |

</div>
</v-click>

<v-click>
<div>
<p class="table-label">Key Metrics</p>

| | Ann. Return | Ann. Risk | Max. Drawdown |
|---|---:|---:|---:|
| **Strategy 1** | 21.44% | 13.78% | -29.62% |
| **NIFTY 500 TRI** | 14.89% | 16.24% | -38.11% |

</div>
</v-click>

<v-click>
<div class="mt-3 flex gap-4 justify-center text-sm">
  <div class="callout-badge callout-green">50% more return than NIFTY 500</div>
  <div class="callout-badge callout-green">lower volatility</div>
  <div class="callout-badge callout-green">shallower max drawdown</div>
</div>
</v-click>

---
layout: default
---

# Strategy 1 · Monthly Returns Profile

<div class="flex justify-center items-center h-[75%] mt-8">
  <img src="/images/slide6_img0.png" class="max-h-[400px] rounded-lg shadow-lg" />
</div>

---
layout: default
---

# Sleep Through Volatility : Strategy 2

<div class="h-full flex items-center justify-center -mt-4">
  <img src="/images/wealth_preservation_low_risk.png" class="max-h-[440px] rounded-xl shadow-lg" />
</div>

---
layout: default
---

# Strategy 2 · For Wealth Preservation

<div class="grid grid-cols-[2fr_1fr] gap-4 items-center h-[82%]">
  <img src="/images/slide7_img0.png" class="max-h-[430px] rounded-lg shadow-lg" />
  <img src="/images/slide7_img1.png" class="max-h-[430px] rounded-lg shadow-lg" />
</div>

---
layout: default
---

# Strategy 2 · Performance Summary

<div class="text-sm mb-3">
Trailing Returns (%) as of <strong>February 13, 2026</strong> · Backtest period: <strong>2017–2026</strong> (9 years)
</div>

<v-click>
<div class="mb-5">
<p class="table-label">Trailing Returns (%)</p>

| | 1 mo | 3 mo | 6 mo | 1 year | 3 years | 5 years |
|---|---:|---:|---:|---:|---:|---:|
| **Strategy 2** | 0.57 | 0.91 | 4.07 | 13.00 | 18.05 | 14.55 |
| **NIFTY 500 TRI** | -0.60 | -2.09 | 3.62 | 8.65 | 17.29 | 15.53 |

</div>
</v-click>

<v-click>
<div>
<p class="table-label">Key Metrics</p>

| | Ann. Return | Ann. Risk | Max. Drawdown |
|---|---:|---:|---:|
| **Strategy 2** | 17.87% | 5.84% | -6.62% |
| **NIFTY 500 TRI** | 14.89% | 16.24% | -38.11% |

</div>
</v-click>

<v-click>
<div class="mt-3 flex gap-4 justify-center text-sm">
  <div class="callout-badge callout-green">3% higher annualised return</div>
  <div class="callout-badge callout-green">1/3rd risk</div>
  <div class="callout-badge callout-green">1/6th max drawdown</div>
</div>
</v-click>

---
layout: default
---

# Strategy 2 · Monthly Returns Profile

<div class="flex justify-center items-center h-[75%] mt-8">
  <img src="/images/slide9_img0.png" class="max-h-[400px] rounded-lg shadow-lg" />
</div>

---
layout: default
---

# Large & Mid Cap Focus : Strategy 3

<div class="h-[78%] flex flex-col items-center justify-center gap-6 -mt-2">
  <div class="text-center">
    <div class="text-sm uppercase tracking-[0.25em] text-[#303192]/70 font-bold mb-3">Key USP</div>
    <div class="text-5xl font-extrabold text-[#303192] leading-tight">Only Large Cap + Mid Cap Stocks</div>
    <div class="mt-3 text-lg text-gray-600">A liquid, institution-friendly variant of the quarterly signal portfolio</div>
  </div>

  <div class="grid grid-cols-3 gap-4 w-full max-w-[850px] text-center">
    <div class="p-4 rounded-xl bg-[#303192]/8 border border-[#303192]/15">
      <div class="text-3xl font-extrabold text-[#303192]">20</div>
      <div class="text-sm font-semibold text-gray-600">stocks selected quarterly</div>
    </div>
    <div class="p-4 rounded-xl bg-[#303192]/8 border border-[#303192]/15">
      <div class="text-3xl font-extrabold text-[#303192]">0%</div>
      <div class="text-sm font-semibold text-gray-600">small-cap exposure</div>
    </div>
    <div class="p-4 rounded-xl bg-[#303192]/8 border border-[#303192]/15">
      <div class="text-3xl font-extrabold text-[#303192]">NIFTY 250</div>
      <div class="text-sm font-semibold text-gray-600">large + mid cap benchmark</div>
    </div>
  </div>
</div>

---
layout: default
---

# Strategy 3 · For Liquid Large & Mid Cap Exposure

<div class="grid grid-cols-[2fr_1fr] gap-4 items-center h-[82%]">
  <img src="/images/strategy3_img1.png" class="max-h-[430px] rounded-lg shadow-lg" />
  <img src="/images/strategy3_img2.png" class="max-h-[430px] rounded-lg shadow-lg" />
</div>

---
layout: default
---

# Strategy 3 · Performance Summary

<div class="text-sm mb-3">
Trailing Returns (%) as of <strong>February 13, 2026</strong> · Backtest period: <strong>2017–2026</strong> (9 years)
</div>

<v-click>
<div class="mb-5">
<p class="table-label">Trailing Returns (%)</p>

| | 1 mo | 3 mo | 6 mo | 1 year | 3 years | 5 years |
|---|---:|---:|---:|---:|---:|---:|
| **Strategy 3** | -0.23 | 1.52 | 4.80 | 12.82 | 25.91 | 22.88 |
| **NIFTY 250 TRI** | -0.50 | -1.82 | 4.27 | 9.35 | 19.14 | 17.01 |

</div>
</v-click>

<v-click>
<div>
<p class="table-label">Key Metrics</p>

| | Ann. Return | Ann. Risk | Max. Drawdown |
|---|---:|---:|---:|
| **Strategy 3** | 21.69% | 10.94% | -25.01% |
| **NIFTY 250 TRI** | 14.39% | 16.56% | -38.55% |

</div>
</v-click>

<v-click>
<div class="mt-3 flex gap-4 justify-center text-sm">
  <div class="callout-badge callout-green">large + mid cap only</div>
  <div class="callout-badge callout-green">7.3% higher annualised return</div>
  <div class="callout-badge callout-green">lower volatility</div>
</div>
</v-click>

---
layout: default
---

# Strategy 3 · Monthly Returns Profile

<div class="flex justify-center items-center h-[75%] mt-8">
  <img src="/images/strategy3_img4.png" class="max-h-[400px] rounded-lg shadow-lg" />
</div>

---
layout: default
class: text-center
---

<div class="h-full flex flex-col items-center justify-center">
  <h1 class="!text-5xl !font-extrabold !border-none" style="color: #303192;">Thank You</h1>
</div>
