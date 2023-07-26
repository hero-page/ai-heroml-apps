# Crypto Investment Recommendation Composer

Crypto Investment Recommendation Composer is your AI-powered guide to the crypto industry. Customize your analyses and generate in-depth investment suggestions for traders interested in blockchain and cryptocurrency. Get comprehensive overviews, performance history, and current context, detailed profiles of recommended cryptocurrencies including unique value propositions. Enhance your understanding with our unique attribute of detailed coin profiles packed with insightful analysis. Informed decision-making is a breeze with provided investment and potential exit strategies.

To run this app online: [Crypto Investment Recommendation Composer Online](https://hero.page/app/crypto-investment-recommendation-composer-ai-powered-custom-crypto-analysis/i8TboHrdR8qX6FiV4rKf)

[![Run Crypto Investment Recommendation Composer Online](/assets/run.svg)](https://hero.page/app/crypto-investment-recommendation-composer-ai-powered-custom-crypto-analysis/i8TboHrdR8qX6FiV4rKf)

To learn more about AI Apps for Crypto Trader use-cases in the Blockchain & Cryptocurrency industry, read [How to Amplify Crypto Trading with AI-Driven Market Analysis & Investment Tips](https://hero.page/blog/ai/blockchain-and-cryptocurrency/how-to-amplify-crypto-trading-with-ai-driven-market-analysis-and-investment-tips/170752)

### What is HeroML?
HeroML is an AI Prompt Chain/Workflow interpreter for Apps built on https://hero.page 

To see other apps, visit the [Hero Apps](https://hero.page/apps) page or explore [AI Apps for all industries](https://hero.page/blog) in the blog section

For more documentation, visit [Hero docs, and learn about AI App Workflows](https://hero.page/tutorials/introduction-to-heroml)

Download [VSCode Syntax Highlighter Ext. here](https://marketplace.visualstudio.com/items?itemName=hero-page.heroml)

## Run with HeroCLI (Requires OpenAI Token)

#### Installation

To install the HeroML CLI tool, you need to have Node.js and npm (comes with Node.js) installed on your machine. If you don't have these, please install them first. 

Then, run the following command in your terminal:

```bash
npm install -g heroml
```

This will install the HeroML CLI tool globally on your system, allowing you to use the `hero` command from any directory.

If you don't want to install it globally, you can run:

```bash
npm install heroml
```

and use it like:

```bash
npx hero run ./crypto_investment_recommendation_composer.heroml
```

We'll be using `hero run ...` in this tutorial for simplicity.

#### Configuration

Before using the HeroML CLI tool, you need to configure your OpenAI API key. 

Create a `heroconfig.json` file in your home directory with the following content:

```json
{
  "openaiApiKey": "your-openai-api-key"
}
```

Replace `"your-openai-api-key"` with your actual OpenAI API key.

#### Usage

To run a HeroML script, use the `run` command followed by the path to your script:

```bash
hero run ./crypto_investment_recommendation_composer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./crypto_investment_recommendation_composer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./crypto_investment_recommendation_composer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./crypto_investment_recommendation_composer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Crypto Investment Recommendation Composer
```
Your task is to write an "Investment Recommendation" for the "Blockchain & Cryptocurrency" industry, specifically targeting a "Crypto Trader". For the first step, let's start with crafting an executive summary. This should provide a concise overview of the cryptocurrency market and articulate the aim of this investment recommendation, which is to manage risk and maximize returns in the cryptocurrency market.

Here's some more context about the Investment Recommendation:
Market Overview: {{market_overview}}
Market Context: {{market_context}}
Crypto Profiles: {{crypto_profiles}}
Value Propositions: {{value_propositions}}
Investment Strategy: {{investment_strategy}}
Risk Factors: {{risk_factors}}
Market Forecast: {{market_forecast}}

->>>>

For a "Blockchain & Cryptocurrency" investment recommendation, we have an executive summary:

Executive Summary:
{{step_1}}

Next, compose an introduction that provides the context for the investment recommendation. Include information about the past performance of related cryptocurrencies, and the current market situation.

->>>>

In the "Blockchain & Cryptocurrency" investment recommendation, we have an introduction and executive summary:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Keeping the context in mind, now let's move on to the cryptocurrency profiles. Give detailed information about the specific cryptocurrencies we're recommending for investment. Include details like launch date, launch price, all-time high price, current price, volume, market cap, and expected future performance.

->>>>

In the "Blockchain & Cryptocurrency investment recommendation", we have executive summary, introduction and now the cryptocurrency profiles:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Cryptocurrency Profiles:
{{step_3}}

For the next step, describe the unique value proposition of each recommended cryptocurrency. This should include the problem it solves, its real-world applications, partnerships, the team behind it, and any technological advancements.

->>>>

For our "Blockchain & Cryptocurrency" investment recommendation, our portfolio consists of the following elements:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Cryptocurrency Profiles:
{{step_3}}

Unique Value Propositions:
{{step_4}}

Next, let's detail the investment strategy, which should cover the recommended portfolio distribution among these different cryptocurrencies. This recommendation should be based on their risk-reward profiles.

->>>>

In the investment recommendation, we have assembled:

Executive Summary:
{{step_1}}

Introduction:
{{step_2}}

Cryptocurrency Profiles:
{{step_3}}

Unique Value Propositions:
{{step_4}}

Investment Strategy:
{{step_5}}

Now, let's discuss potential risk factors associated with the recommended cryptocurrencies. These factors might include market volatility, regulatory uncertainties, technology risks, and competition.


```

