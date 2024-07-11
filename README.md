# Optimizer Finance Litepaper

Website: [optimizerfinance.com](https://www.optimizerfinance.com/)



### Optimizer Finance Litepaper/Whitepaper Outline

#### 1. Executive Summary

* **Purpose**: Brief overview of the document’s objectives.
  * The purpose of this litepaper is to provide an overview of Optimizer Finance, its current applications and projects, and future goals.  This is meant to provide an understanding of the organization regarding where it is currently and where it intends to be in the near future. &#x20;
* **Vision**: Statement on the mission and goals of Optimizer Finance.
  * Optimizer Finance is a research lab at the forefront of DeFi and Machine Learning.  Optimizer Finance intends to optimize financial products and services in both traditional and DeFi through the use of advanced data analytics and machine learning techniques.  By prioritizing innovation, research, and collaboration, Optimizer Finance's products outperform the market and provide cutting-edge solutions to drive the DeFi sector.  The integration of AI and blockchain should be more than a buzzword; Optimizer Finance takes this integration seriously and has the results to back this up. &#x20;
* **Core Offerings**: Summary of the DAO robo advisors, LST index fund, and domain valuator.
  * As of current writing, Optimizer Finance has three projects/products which are:
    * DAO Robo Advisors
    * Machine Learning Managed Index Funds
    * Domain Valuators

#### 2. Introduction

* **Background**: Brief history of Optimizer Finance.
  * Optimizer Finance started from the thesis that machine learning pairs with blockchain technology, and that ML management will enhance financial decision making in DeFi and the blockchain industry as a whole.  With blockchain's principles of decentralization and automation, ML and AI have opportunity to further these principles. &#x20;
  * Optimizer Finance grew from a graduate school project to see if a ML portfolio management strategy could enhance Decentralized Autonomous Organization (DAO) financial decision making and result in increased stability compared to the current strategies being deployed.  Given the promising results obtained from this initial hypothesis testing, the concept grew to further explore the integration of ML into other portions of DeFi.   &#x20;
* **Market Context**: Overview of the current landscape in DeFi, blockchain domains, and machine learning in finance.
  * The DeFi space provides an environment for testing and truly new and innovative concepts, and the potential for smart contracts in finance is steadily being realized in traditional finance.  Industry finance titans are testing and developing products using blockchain technology and even utilizing public blockchains. &#x20;
  * Related to DeFi, the introduction of Real World Assets (RWA) has provided a bridge between traditional finance and blockchain-enabled financial applications.  However, with the vast majority of RWA being non-digitally native, there is still friction in integrating the two concepts.  Domains present an interesting type of RWA, as they are digitally-native.  The on chain domain reigstrar 3DNS enables anyone to mint a domain as a blockchain asset, allowing easy and direct trading, management, and potential for financial applications such as collateralized loans.  Domain names may be the best type of RWA at this point, and companies like 3DNS and .Box are at the forefront of further integrating the Domain and blockchain industries. &#x20;
  * The introduction of LLM models such as Chatgpt, and the increasing availability of cheap computing power has made machine learning accessible to a wider audience, allowing developers to test concepts integrating ML.  Traditional finance is steadily integrating ML into operations, with the use of robo advisors steadily increasing in the industry.  Robo advisors allow for impartial financial analysis and remove emotion from trading, which has resulted in outsized returns compared to previous stratgies and methods.  The most impactful ML methods in Finance to date have been forecasting, useful for predicting asset prices and market movements; and reinforcement learning, which has been shown to outcompete with regarding to portfolio rebalancing.  With the increased access to ML technologies through severeal software libraries, we are seeing a revolution in ML for Finance.  However, this increased ease in access has made it difficult to discern which concepts and products are truly revolutionary, and those which use AI and ML as buzzwords to drive hype and potentially dupe investors. &#x20;

#### 3. Problem Statement

* **DAO Treasury Management Issues**: Inefficiencies, risks, and complexities.  While intending to be decentralized and autonomous, many decisions, particularly in financial management, are human led and driven, leading to potential conflicts of risk, collusion, and is a weak point in DAOs.
* **Lack of Sophisticated Tools**: Challenges in traditional asset management.  While blockchain enables digitally native financial applications, traditional methods and strategies are still prevalent in DeFi, whereas the industry should strive to lead FinTech applications. &#x20;
* **Domain Valuation Challenges**: Issues in valuing web3 domains compared to web2 domains.  Web2 domain sales data is gated behind paywalls and can be expensive or difficult to access.  This makes the development of domain valuation models slower and less robust.  Further, web2 domain sales and management have serious pain points and domains are treated as if they are not natively digital. &#x20;

#### 4. Solutions Offered

* **DAO Robo Advisors**
  * **Overview**: Introduction to the Vault and Treasury Robo Advisors.
    * In a bid to enhance DAO treasury management, two robo advisors were developed, the Vault Robo Advisor and the Treasury Robo Advisor.  These advisors were trained and backtested specifically with DAO's in mind, taking into account the unique issues in DAO financial management.  While asset prices move quickly, DAO governance does not, which can lead to serious issues. &#x20;
    * The vault robo advisor was designed with MakerDAO and the Maker Protocol in mind.  This advisor manages the portfolio of a CDP protocol by controlling the debt ceilings of several vaults within the protocol.  This is meant to incentivize/disincentivize deposits and withdrawals to vaults in the portfolio, and to target and drive towards an optimized portfolio in accordance with advanced financial calculations and the application of financial theory.  This is meant to balance growth and stability for CDP protocols. &#x20;
    * The treasury robo advisor was developed for direct portfolio rebalancing, allowing the DAO to control key parameters such as selection of assets to choose from, rebalancing frequency, and portfolio bounds for an asset, enabling hybrid risk management. &#x20;
  * **Methodology**: Explanation of Mean-Variance Optimization (MVO), forecasting, and Reinforcement Learning (RL) techniques used.
    * At the core of these models are Mean-Variance Optimization (MVO) and reinforcement learning (RL).  Mean-Variance Optimization is utilized to target an optimal portfolio allocation, specifically by targeting a portfolio with an optimal Sortino Ratio, which prioritizes reducing portfolio downside risk.  Reinforcement Learning enables the ML model to learn from its actions and dynamically tweak its strategy given the results of prior actions.  The Vault Robo Advisor uses a custom built RL model utilizing Q-Table learning, whereas the Treasury Advisor combines OpenAI's Gym.env environment with a Proximal Policy Optimization (PPO) RL model. &#x20;
    * The Vault Robo Advisor specifically utilizes a forecasting model as the backbone of a simulator to simulate the results of debt ceiling changes on the respective vaults of the portfolio.  This enables robust backtesting of the model and to compare the historical results to the robo advisor managed results. &#x20;
  * **Performance Metrics**:&#x20;
    * Backtesting for the robo advisors showed improved portfolio returns and lower downside risk, as demonstrated by higher returns and Sortino Ratio metrics compared to the historical data. &#x20;
    * Treasury Advisor
      * Averaging the results of 10 runs over 10 different seeds, the Treasury Robo Advisor achieved an average cumualtive return of 120% over the period of March 22, 2023 through May 15, 2025, with a average Sortino Ratio of 3.45.  Compared to the backtested DAO, PanamaDAO, which had a allocation of 99% ETH during the same time period and achieved a cumulative return of 61.80% and Sortino ratio of 1.81.  The treasury advisor also achieved a better Market risk adjusted strategy, with a Beta of 2.7 but a compound annual growth rate of 145%, compared to the DAO Beta of 1.74 and CAGR of 63.39%.  Several DAO Treasury indices were created to allow for comparison to DAO benchmarks; the average RL portfolio outperformed all but one index in terms of returns and market risk.
    * Vault Advisor
      * Also averaging the results of 10 runs, the vault advisor similarly achieved outsized returns and lower downside risk.  Over the test period of May 20, 2022 through March 20, 2024, The RL average cumulative return was -19%, Sortino Ratio was -0.22, and Total Value Locked for the portfolio was $10,629,002,211.  Compared to Maker Protocol historical scores during the same period with a cumulative return of -34%, Sortino Ratio of -0.55, and TVL of $7,342,533,784\
        &#x20;&#x20;
* **Liquid Staking Token (LST) Index**
  * **Overview**: Introduction to the LST index fund.
    * This project was developed out of StarkHack 2024, with the goal of simplifying and streamlining the process to gain the best exposure to Ethereum liquid staking tokens.  The index fund is managed by a ML, which uses Value at Risk/Conditional Value at Risk (VaR/CVaR), time series forecasting, and RL to chose an optimal portfolio of liquid staking tokens.  VaR/CVaR is used to inform the model of the potential losses associated with a portfolio, whereas forecasting is used to anticipate future asset prices, in a bid to reduce portfolio losses.  This info is fed to the RL model, which makes an optimal portfolio allocation given these results and calculations.  The RL model is able to choose from wstETH, rETH, and sfrxETH, considered to be the LSTs with adequate liquidity and least custody risk.  &#x20;
  * **Technology Stack**: Details on Flask backend, JavaScript frontend, and machine learning models used.
    * The ML model is housed in OpenAI's gym.env envioronment where a PPO RL model is informed from the VaR/CVaR and forecasting results to make a portfolio allocation.  The model takes in several parameters, principally rebalancing frequency, and outputs an action representing the target portfolio composition for the period. &#x20;
    * The model and environment is imported into a Flask app which receives hourly price data for the LSTs via Flipside API, and rebalances given the rebalance frequency parameter.  The model is connected to a wallet on the Starknet Sepolia testnet using the Starknet.py Python SDK; once the model makes the action, the script translates that action into a new target balance, given the current balance of the Starknet wallet, and affects the necessary swaps to achieve the target composition.  Once the new composition is achieved for the fund, the data is captured and visualized on the Javascript front end.  This includes hourly composition, rewards, normalized comparison to LSTs, forecasted prices, fund value, and excess returns over the LSTs. &#x20;
  * **Performance Results**: Highlights of performance metrics and comparison with other LSTs.
    * Averaging 10 runs with 10 different random seeds, starting from January 10, 2023 through June 18, 2024, the index cumulative weighted daily return achieved an average excess return of 43% over rETH, 36% over wstETH, and 35% over sfrxETH.  At the end of the period, the index attained a CAGR of 125% compared to 103% for rETH, 107% for wstETH, and 107% for sfrxETH.  &#x20;
* **Domain Valuator**
  * **Overview**: Introduction to the domain valuator tool.
    * The domain valuator tool comes as a result of preliminary data analysis on the 3DNS domains market.  Given that data, and the thesis that on chain domains are optimal RWA, the goal of the domain valuator is to provide a fair value for a domain.  This is to enable and increase liquidity for these domains, by giving buyers and sellers an estimate of how much a domain is worth.  The end user simply inputs the domain name they want to value, and the model provides an estimate.
  * **Integration**: Combining web2 and web3 domain sales data.
    * The specific ML model used currently is linear regression with Ridge hypertuning.  A dataset of web2 domain sales from 1994, containing hundreds of thousands of domain sales, was used for training the model, in addition to the sales of 3DNS domains.  Given this historical data, the model estimates the value for a given domain based on its characteristics, such as length and domain ending. &#x20;
  * **Current Progress**: Status of the Python script and Dash app.
    * The model is currently being used to value .Box domains specifically, but has wider reaching implications.  The ability to automatically detect the 3DNS domains in a given wallet, and estimate the worth of the wallet's portfolio, is in progress.  Further development to increase its accuracy scores on historical data should optimize the estimations.  Once the model is performing optimally, there is potential to use it as a price reference for on chain domains to enable its use in DeFi applications, such as collateralized loans/CDPs.  This would also enable on chain domains use in DAO treasuries, furthering the thesis of on chain domains as optimal RWAs.     &#x20;

#### 5. Technical Architecture

* **DAO Robo Advisors**
  * **Architecture**: Technical details on the Streamlit app.
    * The current iteration is live in the form of a Streamlit app which allows a user to configure their own robo advisor and compare results to historical data and benchmarks.  An on chain iteration could be used as a stand alone fund in which a DAO would buy a share, or integrated to rebalance a specific DAO Treasury wallet address. &#x20;
  * **Data Handling**: Explanation of data processing and model training.
    * Vault Robo Advisor
      * The Vault Robo Advisor utilizes a simulation portion to backtest the model's strategy.  This simulator utilizes multiple linear regression with ridge hypertuning, as well as other stochastic variables such as moving average volatility, to simulate vault balances changes as a result of debt ceiling adjustments.  This forecasting model was trained on tens of thousands of data points obtained from onchain data analysis of the Maker core accounting system (VAT), existing dashboards and queries aggregating protocol data, as well as crypto market and macroeconomic data such as risk-free rates, CPI, crypto market volume, etc.&#x20;
      * The vault robo advisor works on a 24 day rebalance strategy; every 24 days the model calculates mean variance optimization target weights, portfolio return and Sortino Ratio, which is translated into a reward.  Given that reward, the model chooses a debt ceiling adjustment strategy which targets an optimal portfolio composition.  For example, the target weights may signify less capital in the ETH vault and more capital in the BTC vault, as a result of Sortino ratio calculations for each vault.  As a result, the model will reduce the ETH vault and increase the BTC vault by a certain amount over the 24 day period. &#x20;
      * The custom RL model trains by making random actions for the first few 24 day cycles, and from then on uses the results of those actions to inform an optimal policy, continuously learning from its actions. &#x20;
    * Treasury Robo Advisor&#x20;
      * The Treasury Robo Advisor is more direct in rebalancing a portfolio.  DAO Treasury indicies and benchmarks were created by calculating the weighted daily returns of the treasury assets for a variety of DAOs by sector, and those returns were aggregated to represent a sector index.  Regarding the model itself, in an attempt to smooth over cash flows which would impact the DAO treasury balance, the model targets specific portfolio compositions, and returns are calculated in the same manner as the DAO treasury indicies.  Given the rebalance parameter, the model generates an action given a combined Sortino ratio and portfolio return reward as feedback.  Unlike the Vault Robo Advisor, we are able to directly swap into the target portfolio composition, removing the need for a simulation model. &#x20;
      * After the model runs for the specified start and end date, the ending portfolio return and sortino ratio are calculated, as well as normalized returns.  This is used for comparison with the DAO treasury indicies.  Furthermore, a security market line visualization is created to also compare the portfolio performance in terms of market risk/return.     &#x20;
      * The model is first trained and fitted on historical data to develop an optimal policy for the environment.  Once a model which performs well on historical data is fitted, the model is deployed in a test run. &#x20;
* **LST Index**
  * **Environment Setup**: Description of the RL environment.
    * This model is a customized extension of the Treasury Robo Advisor.  Instead of focusing on and being backtested to DAO treasury performance, the model targets an optimal portfolio of LSTs, designed to provide the best exposure to the asset class.  Hourly data is fed to the model, with rewards and forecasts generated accordingly.  The model rebalances given the rebalance frequency parameter. &#x20;
    * The model was trained and fitted to historical data, from January 2023 through June 2024, to develop an optimal policy for the environment.  This optimized model was then deployed on live data.  From initial backtesting, a 24 hour rebalance frequency performed best. &#x20;
  * **Forecasting and Blockchain Integration**: Use of Prophet library and Starknet Sepolia blockchain.
    * The index fund was deployed on the Starknet Sepolia testnet and rebalances a wallet address given testnet ERC20 tokens representing wstETH, rETH, and sfrxETH.  Hourly data is received from a Flipside API, and model actions are translated into on chain swaps.  A second flask app and wallet address was deployed to represent a DEX which holds the balances for the testnet ERC20 tokens.  The RL flask app sends the logical amount of tokens to the DEX, and the DEX sends back the logical amount to reach the target balance.  This utilizes price feeds from Flipside API.   &#x20;
    * A Prophet library univariate forecasting model was backtested to predict the prices for respective LSTs.  This fitted model was then deployed in the live RL model environment.  &#x20;
  * **Flask API**: Details on the API endpoints and background tasks.
    * Every hour the Flask app updates, which then sends the new data to a Javascript front end for visualization.  The data is cached hourly, ensuring data synchronization between the two scripts. &#x20;
* **Domain Valuator**
  * **Script and App**: Technical details on the Python script and Dash app.
  * **Data Integration**: Methods for integrating web2 and web3 data.

#### 6. Revenue Model

* **DAO Robo Advisors**: Performance and management fees.
* **LST Index**: Potential fee structures for the index fund.
* **Domain Valuator**: Possible monetization strategies.

#### 7. Roadmap and Future Work

* **Short-term Goals**: Upcoming features and developments.
* **Long-term Vision**: Expansion plans and future offerings.

#### 8. Team

* **Founders and Developers**: Introduction to the team behind Optimizer Finance.
* **Advisors and Partners**: List of advisors and strategic partners.

#### 9. Contact Information

* **Website**: Link to optimizerfinance.com.
* **Email**: Contact email address.
* **Social Media**: Links to GitHub and other relevant profiles.

#### 10. Appendices

* **DAO Robo Advisor Results**: Detailed performance results.
* **LST Index Results**: Comprehensive results and comparisons.
* **Technical References**: Additional technical documentation and resources.

