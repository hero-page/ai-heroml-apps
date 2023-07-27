# AI Cosmetic Brand Strategy Creator

AI Cosmetic Brand Strategy Creator is a revolutionary app built for crafting unique cosmetics brand strategies. Users can input specific variables and depend on its AI power to generate detailed, high-quality content. The app provides strategies involving defining brand purpose, creating a persona, and identifying target audience. It also assists in product outlining, pricing, distribution, and promotional strategies. The standout aspect is its dedicated focus on the cosmetics industry, with strategies tailored for the market. It ensures continuity, adapting to market fluctuations and customer feedback, portraying a dynamic and engaging approach.

To run this app online: [AI Cosmetic Brand Strategy Creator Online](https://hero.page/app/ai-cosmetic-brand-strategy-creator-tailored-cosmetic-brand-strategizing/CsbCNNhjuUJ8n00NfNi7)

[![Run AI Cosmetic Brand Strategy Creator Online](/assets/run.svg)](https://hero.page/app/ai-cosmetic-brand-strategy-creator-tailored-cosmetic-brand-strategizing/CsbCNNhjuUJ8n00NfNi7)

To learn more about AI Apps for Brand Manager use-cases in the Cosmetics & Beauty Product Marketing industry, read [How to Elevate Cosmetics Marketing with AI-Powered Strategy, Minutes and Outreach](https://hero.page/blog/ai/cosmetics-and-beauty-product-marketing/how-to-elevate-cosmetics-marketing-with-ai-powered-strategy-minutes-and-outreach/170823)

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
npx hero run ./ai_cosmetic_brand_strategy_creator.heroml
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
hero run ./ai_cosmetic_brand_strategy_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./ai_cosmetic_brand_strategy_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./ai_cosmetic_brand_strategy_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./ai_cosmetic_brand_strategy_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

