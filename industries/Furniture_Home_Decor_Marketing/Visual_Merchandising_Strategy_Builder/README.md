# Visual Merchandising Strategy Builder

The Visual Merchandising Strategy Builder app is an AI-powered planner tool specialized for the furniture and home decor industry. Users can specify variable prompts to create customized content, offering detailed merchandising strategies. This unique app crafts tailored strategies that encompass a clear goal, customer profile, product mix analysis, visual presentation plan, store layout, signage, display elements, and a future-oriented merchandise refresh plan. It also includes an innovative customer feedback mechanism. The app provides a detailed implementation plan which reveals timelines, budget, and key performance indicators. Its prime feature is its emphasis on visual aspects of marketing, making it an ultimate tool for visual merchandisers.

To run this app online: [Visual Merchandising Strategy Builder Online](https://hero.page/app/visual-merchandising-strategy-builder-ai-powered-decor-merchandising-planner/NbLeYLWGyyzGwwY65IKV)

[![Run Visual Merchandising Strategy Builder Online](/assets/run.svg)](https://hero.page/app/visual-merchandising-strategy-builder-ai-powered-decor-merchandising-planner/NbLeYLWGyyzGwwY65IKV)

To learn more about AI Apps for Visual Merchandiser use-cases in the Furniture & Home Decor Marketing industry, read [How to Elevate Furniture Marketing with AI-Enhanced Display Strategies](https://hero.page/blog/ai/furniture-and-home-decor-marketing/how-to-elevate-furniture-marketing-with-ai-enhanced-display-strategies/170896)

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
npx hero run ./visual_merchandising_strategy_builder.heroml
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
hero run ./visual_merchandising_strategy_builder.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./visual_merchandising_strategy_builder.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./visual_merchandising_strategy_builder.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./visual_merchandising_strategy_builder.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

