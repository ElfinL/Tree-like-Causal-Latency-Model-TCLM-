# Tree-like Causal Latency Model (TCLM) & Dual-Pulse Synchronization Protocol (DPSP)

**樹狀因果延遲模型（TCLM）與雙脈衝同步協議（DPSP）**

From Observational-Delay Deconstruction to Interplanetary Deep-Space Chronometric Engineering

從觀測延遲解構到行星際深空計時工程

> Newton was right. Einstein was also right.
> The causal tree is a framework that allows both to be true simultaneously.
>
> 牛頓是對的。愛因斯坦也是對的。
> 因果樹，是同時讓兩者成立的一種框架。

---

## One-Sentence Summary / 一句話摘要

This work shows that equating the mathematical failure of the Lorentz transformation at \(v > c\) with "time reversal" confuses **signal propagation latency** with **physical time order**, and proposes a clean separation between topological causal order and geometric time-rate differences, together with an engineering protocol for deep-space time reconstruction.

本文指出：將勞侖茲變換在 \(v > c\) 時的數學失效直接等同於「時間倒流」，是把**訊號傳播延遲**誤認為**物理時間序**。本文提出拓撲因果序與幾何時間流速差的嚴格解耦，並提出一套深空時間還原的工程協議。

---

## The Problem This Addresses / 解決的問題

Most discussions of faster-than-light and time travel treat the appearance of imaginary numbers in the Lorentz factor as evidence that "time runs backward."

This paper argues that this is an operational category error: the geometric limit of latency compression is **Ping = 0**, not negative latency (\(L < 0\)).

多數關於超光速與時間旅行的討論，將勞侖茲因子出現虛數視為「時間倒流」的證據。本文指出這是操作層面的範疇錯誤：延遲壓縮的幾何極限是 **Ping = 0**，而非負延遲（\(L < 0\)）。

If you are working on / 若你正在研究：

- deep-space navigation / timing autonomy（深空導航與自主計時）
- relativistic time-transfer protocols（相對論時間傳遞協議）
- the operational meaning of causality under extreme conditions（極端條件下因果性的操作意義）
- the precise boundary between special-relativistic kinematics and general-relativistic causality（狹義相對論運動學與廣義相對論因果性的精確邊界）

this framework may be useful.

---

## What This Work Actually Claims / 本文實際主張

**TCLM** strictly decouples:

- **Topological Causal Order** (Trunk \(\mathcal{C}_{\text{trunk}}\), \(\operatorname{sgn}(\Delta\mathcal{C}) \equiv +1\)) — the irreversible order of event settlement
- **Geometric Time-Rate Difference** (Branches) — local proper-time rates and observational latency

**TCLM** 將時間嚴格解耦為：

- **拓撲因果序（主幹 \(\mathcal{C}_{\text{trunk}}\)，\(\operatorname{sgn}(\Delta\mathcal{C}) \equiv +1\)）** — 事件結算的不可逆順序
- **幾何時間流速差（樹枝）** — 局部固有時率與觀測延遲

---

**DPSP** (Dual-Pulse Synchronization Protocol) is a conceptual application-layer protocol that:

- locks only a single initial integration constant \(t_0\),
- measures local time-rate factor \(\Gamma_{\text{local}}\) via multi-baseline triangulation,
- reconstructs causal order relative to the handshake by worldline path integration,
- tolerates long communication blackouts.

**DPSP**（雙脈衝同步協議）是一個概念性應用層協議：

- 僅鎖定一次初始積分常數 \(t_0\)
- 以多基線三角測量本地時間流率因子 \(\Gamma_{\text{local}}\)
- 以世界線路徑積分還原相對於初始握手的因果序
- 容忍長期通訊中斷

---

**FASC** (Flow-Adaptive Synthesized Clock) is the clock implementation within DPSP:

- **Physical layer**: constant proper frequency \(f_0\), records local proper time \(\tau\).
- **Processing layer**: dynamically adjusts output frequency based on measured \(\Gamma_{\text{local}}\), so that \(\mathcal{C}_{\text{trunk}}\) advances consistently relative to \(t_0\).

FASC solves the problem that a node does not need to know another node's UTC to align causal order.

**FASC**（流速自適應合成時脈）是 DPSP 的時鐘實現：

- **物理固有層**：提供恆定固有頻率 \(f_0\)，記錄本地固有時 \(\tau\)。
- **數位調頻層**：根據測得的 \(\Gamma_{\text{local}}\) 動態調整輸出頻率，使 \(\mathcal{C}_{\text{trunk}}\) 相對於 \(t_0\) 一致推進。

FASC 解決的問題是：節點不需要知道彼此的 UTC，也能對齊因果序。

---

**Earth–Mars calibration target** (theoretical, pending end-to-end validation):

engineering alignment error budget \(\mathcal{O}(10^{-9}\,\text{s})\) after multi-frequency dispersion compensation and ephemeris constraints.
Hardware floor set by optical-lattice clocks (\(10^{-18}\)–\(10^{-19}\)).

**地火校準目標**（理論，尚待端到端驗證）：

經多頻色散補償與星曆約束後，工程對齊誤差預算為 \(\mathcal{O}(10^{-9}\,\text{s})\)。
硬體極限由光晶格鐘設定（\(10^{-18}\)–\(10^{-19}\)）。

---

## Explicit Scope & Falsifiability / 明確範圍與可否證性

This paper **does not** claim:

- that returning to the past is impossible,
- that any FTL mechanism is engineering-feasible,
- gravitational-wave detection capability,
- or that quantum entanglement provides instantaneous communication.

本文**不主張**：

- 回到過去在物理上不可能
- 任何超光速機制已具工程可行性
- 已具備重力波探測能力
- 量子糾纏可提供瞬時通訊

It claims only that, **on the velocity-superposition path**, the operational domain of propagation latency is \([0, \infty)\), and \(L < 0\) is undefined.

本文僅主張：**在速度疊加路徑上**，傳播延遲的操作定義域為 \([0, \infty)\)，\(L < 0\) 無定義。

**Falsifiability condition**: If a concrete physical mechanism is found that allows velocity superposition to achieve \(L < 0\) (signal arrival before emission), the model's inference on that path is falsified.

**可否證條件**：若存在一個具體的物理機制，使速度疊加可實現 \(L < 0\)（信號在發送之前到達），則本模型在該路徑上的推論被否證。

---

## Files in This Repository / 倉庫檔案

本倉庫主要檔案命名規則如下（版本號會隨更新變動）。請直接查看倉庫根目錄中**版本號最大**的檔案，即為目前最新版。

The naming convention is as follows (version numbers change with updates). Please look for the file with the **largest version number** in the repository root — that is the latest version.

| 類型 / Type | 檔名模式 / Filename Pattern | 說明 / Description |
|------|----------|------|
| 中文 Markdown | `中文版：樹狀因果延遲模型（TCLM）XXX.md` | 最新中文完整版 / Latest Chinese full version |
| 中文 PDF | `中文版：樹狀因果延遲模型（TCLM）XXX.pdf` | 最新中文 PDF / Latest Chinese PDF |
| English Markdown | `English Version Tree-like Causal Latency Model (TCLM)XXX.md` | Latest English full version / 最新英文完整版 |
| English PDF | `English Version Tree-like Causal Latency Model (TCLM)XXX.pdf` | Latest English PDF / 最新英文 PDF |
| Archive | `archive/` | 歷史版本/ Archived versions  |

---

## Papers / 論文

| Title | Status | Link |
|-------|--------|------|
| **Tree-like Causal Latency Model (TCLM) and Dual-Pulse Synchronization Protocol (DPSP)** | Main paper (Chinese & English) | [Zenodo](https://doi.org/10.5281/zenodo.22252215) |
| The Circular Reasoning in the Superluminal Ban | Logical note | [Zenodo](https://doi.org/10.5281/zenodo.22782047) |
| Star Velocity Recovery Protocol (SVRP) | Related protocol | [Zenodo](https://doi.org/10.5281/zenodo.22722590) |

> In case of any discrepancy between the English and Chinese versions, the **Chinese version shall prevail**.
>
> 若英文版與中文版有任何歧異，概以**中文版為準**。

---

## Who Should Read This / 適合讀者

- Researchers working on relativistic time transfer and deep-space chronometry（研究相對論時間傳遞與深空計時的研究者）
- Engineers designing autonomous timing systems for interplanetary missions（設計行星際任務自主計時系統的工程師）
- Physicists interested in the operational distinction between causal order and observed time（關注因果序與觀測時間之操作區分的物理學家）
- Anyone who has ever been told "FTL implies time travel" and felt the argument was incomplete（任何曾被「超光速意味著時間旅行」說法困擾、並覺得該論證不完整的人）

---

## Citation / 引用

```bibtex
@article{Lee2026TCLM,
  author  = {Lee, Wang Hin},
  title   = {Tree-like Causal Latency Model (TCLM) and Dual-Pulse Synchronization Protocol (DPSP): From Observational-Delay Deconstruction to Interplanetary and Cross-Galactic Deep-Space Chronometric Engineering},
  year    = {2026},
  publisher = {Zenodo},
  doi     = {10.5281/zenodo.22252215}
}
```

DOI: [10.5281/zenodo.22252215](https://doi.org/10.5281/zenodo.22252215)

---

## Author / 作者

**Lee Wang Hin (李泓軒, Elfin)**
Independent Researcher / 獨立研究員
Contact: elfin.indres@proton.me