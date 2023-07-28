# Eco-Market Analysis Expert AI

Eco-Market Analysis Expert AI, with subtitle Sustainable Product Market AI Insights, is a sophisticated application empowering users to initiate advanced variable prompts for custom content creation. Users get detailed, high-level market reports specifically focused on the eco-friendly and sustainable product market. The AI provides comprehensive market environment reviews, in-depth customer and competitor studies, product analysis, potential market opportunities, and green marketing strategies. The produced content highlights essential findings and their impact on marketing strategies, supported by trusted data presented in a clear, digestible format. This tool uniquely zeroes in on the eco-friendly market rather than general market analysis and delivers practical insights to existing or potential businesses in this sector.

To run this app online: [Eco-Market Analysis Expert AI Online](https://hero.page/app/eco-market-analysis-expert-ai-sustainable-product-market-ai-insights/Nik5HDVznE5XA2j5KFHp)

[![Run Eco-Market Analysis Expert AI Online](/assets/run.svg)](https://hero.page/app/eco-market-analysis-expert-ai-sustainable-product-market-ai-insights/Nik5HDVznE5XA2j5KFHp)

To learn more about AI Apps for Product Marketer use-cases in the Eco-friendly & Sustainable Product Marketing industry, read [How to Amplify Eco-Friendly Product Marketing with AI Tools](https://hero.page/blog/ai/eco-friendly-and-sustainable-product-marketing/how-to-amplify-eco-friendly-product-marketing-with-ai-tools/170846)

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
npx hero run ./eco_market_analysis_expert_ai.heroml
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
hero run ./eco_market_analysis_expert_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./eco_market_analysis_expert_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./eco_market_analysis_expert_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./eco_market_analysis_expert_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

