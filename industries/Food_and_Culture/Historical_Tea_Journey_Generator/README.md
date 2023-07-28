# Historical Tea Journey Generator

Immerse yourself in a captivating tea journey with the Historical Tea Journey Generator. Delve into the riveting cultural history of tea, tracing it from its origins to the present day. Utilize AI to generate bespoke content, exploring eras where tea evolved, its cultivation, brewing methods, and types. Discover tea's trading history, and its influence during notable historical events. Examine tea's social and cultural transformations across various societies. Make your journey as unique as you with customizable prompts, inviting an in-depth analysis of tea's historical impacts.

To run this app online: [Historical Tea Journey Generator Online](https://hero.page/app/historical-tea-journey-generator-cultural-tea-history-deep-dive/XOMckhLcHmURw6307Xpb)

[![Run Historical Tea Journey Generator Online](/assets/run.svg)](https://hero.page/app/historical-tea-journey-generator-cultural-tea-history-deep-dive/XOMckhLcHmURw6307Xpb)

To learn more about AI Apps for Food Historian use-cases in the Food and Culture industry, read [How to Uncover Food History with AI: Recipes, Pizza Evolution, Tea Journey](https://hero.page/blog/ai/food-and-culture/how-to-uncover-food-history-with-ai:-recipes-pizza-evolution-tea-journey/170888)

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
npx hero run ./historical_tea_journey_generator.heroml
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
hero run ./historical_tea_journey_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./historical_tea_journey_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./historical_tea_journey_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./historical_tea_journey_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

