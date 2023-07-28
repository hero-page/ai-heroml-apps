# Merchandising Strategy AI planner

Merchandising Strategy AI Planner is an AI-powered app providing tailor-made merchandising solutions. You can define variables and the app generates optimum business strategies, with particular focus on the fashion and apparel industry. The AI offers you a comprehensive plan that includes audience analysis, product selection, store layout, promotion tactics, and trend incorporation. The unique approach of intertwining industry trends and innovation in strategies adds a competitive edge and helps to stay relevant in this fast-paced market.

To run this app online: [Merchandising Strategy AI planner Online](https://hero.page/app/merchandising-strategy-ai-planner-ai-driven-innovative-merchandising-solutions/ISmwevZAKQHF7tLQrEoy)

[![Run Merchandising Strategy AI planner Online](/assets/run.svg)](https://hero.page/app/merchandising-strategy-ai-planner-ai-driven-innovative-merchandising-solutions/ISmwevZAKQHF7tLQrEoy)

To learn more about AI Apps for Visual Merchandiser use-cases in the Fashion & Apparel Marketing industry, read [How to Elevate Fashion Store Layout, Strategy and Moodboard with AI](https://hero.page/blog/ai/fashion-and-apparel-marketing/how-to-elevate-fashion-store-layout-strategy-and-moodboard-with-ai/170869)

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
npx hero run ./merchandising_strategy_ai_planner.heroml
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
hero run ./merchandising_strategy_ai_planner.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./merchandising_strategy_ai_planner.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./merchandising_strategy_ai_planner.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./merchandising_strategy_ai_planner.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

