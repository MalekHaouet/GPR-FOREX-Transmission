**Geopolitics in Motion: The Hidden Architecture Behind Currency Reactions**
**Author:** Malek Haouet
**Institution:** IE University — Dual Degree: Bachelor in Business Administration & Bachelor in International Relations
**Date:** May 2026

**Overview**
This repository contains the full replication code for the empirical analysis in my undergraduate thesis. The paper examines how structural economic exposure shapes the transmission of geopolitical risk to currency markets, using a monthly panel of 38 countries from January 2000 to December 2023.
The analysis follows a three-stage framework. Stage 1 establishes country-level GPR sensitivity and stress-period NEER performance. Stage 2A runs cross-sectional OLS and Spearman rank correlations across N=38 countries. Stage 2B runs panel interaction regressions with country and year fixed effects restricted to stress months. Stage 3 conducts an exploratory dynamic analysis via local projections and episode-level recovery analysis.

**Key Findings**
Four structural channels consistently condition exchange-rate behaviour under GPR stress. Non-FDI liability share amplifies depreciation and is significant in the panel only. CTOT exposure attenuates depreciation for commodity exporters and is also panel-only. CPI inflation is significant in both the cross-section and the panel but with opposite signs. The same goes for FX reserves that are significant in both methods but with opposite signs, reflecting a selection effect whereby structurally vulnerable economies hold larger precautionary buffers.

**Repository Structure**
The code folder contains all analysis notebooks intended to be run in order. Cell 1 handles setup, CTOT construction, and master panel build. Cell 2 produces descriptive statistics, summary tables, and correlation figures. Cell 3 runs Stage 1 and computes the primary cross-sectional dependent variable. The shared helper cell defines functions used by all hypothesis cells. Cells 4 through 10 run Stage 2A and 2B hypothesis testing for H2 through H8. Cell 11 runs the dynamic analysis including local projections, recovery analysis, and structural linkage.

**Data Sources**
The raw data must be downloaded manually. Due to licensing restrictions no raw data files are included in this repository.
NEER data comes from the Bank for International Settlements at bis.org/statistics/eer. GPR global and country indices come from Caldara and Iacoviello (2022) at matteoiacoviello.com/gpr. VIX come from FRED at fred.stlouisfed.org. The External Wealth of Nations dataset comes from Lane and Milesi-Ferretti via imf.org. Commodity Terms of Trade come from the IMF at imf.org. Trade in Value Added data comes from the OECD at oecd.org/sti/ind/tiva. FX reserves, inflation, trade openness, and GDP growth come from the World Bank World Development Indicators at data.worldbank.org. The exchange rate regime classification comes from Ilzetzki, Reinhart and Rogoff at carmenreinhart.com.

**Replication Instructions**
Download all data files listed above and place them in a folder on Google Drive. Open the notebooks in Google Colab. Update the BASE_DIR path in Cell 1 to point to your Drive folder. Run the data preparation notebook first, then run the analysis notebook cells in order from Cell 1 through Cell 11. All outputs including tables and figures will be saved to the output directory defined in Cell 1.

**Software**
All analysis was conducted in Python 3.10 via Google Colab. Key packages are pandas, numpy, statsmodels, scipy, matplotlib, openpyxl, and xlrd.

**Citation**
Haouet, M. (2026). Geopolitics in Motion: The Hidden Architecture Behind Currency Reactions. Undergraduate Thesis, IE University.

**Note on AI Assistance**
This project used Claude (Anthropic) and ChatGPT (OpenAI) as coding assistants during the empirical analysis phase. All analytical and substantive decisions including research design, methodology, variable selection, model specifications, and interpretation of results were made independently by the author.
