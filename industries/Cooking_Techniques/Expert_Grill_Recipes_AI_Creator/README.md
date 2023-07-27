# Expert Grill Recipes AI Creator

Unlock the world of gourmet grilling with Expert Grill Recipes AI Creator. This unique app harnesses AI power to offer you bespoke, advanced-level BBQ recipes, based on your preferences. Enter variables like preferred ingredients or cooking techniques, and let our AI generate an incredibly detailed and professional-standard BBQ sauce recipe for you. Each recipe comes with an engaging introduction, precise ingredients and quantities, a thorough step-by-step guide, innovative variations, helpful usage suggestions, and exact timings. Notably, our BBQ sauce recipes showcase intricate cooking techniques and unique ingredients, perfect for the seasoned grilling expert who seeks sophisticated grilling ventures. From start to finish, let this app be your personal digital chef.

To run this app online: [Expert Grill Recipes AI Creator Online](https://hero.page/app/expert-grill-recipes-ai-creator-ai-generated-advanced-bbq-recipes/WjRY2S76WJCyJDSV8rXl)

[![Run Expert Grill Recipes AI Creator Online](/assets/run.svg)](https://hero.page/app/expert-grill-recipes-ai-creator-ai-generated-advanced-bbq-recipes/WjRY2S76WJCyJDSV8rXl)

To learn more about AI Apps for Grilling Expert use-cases in the Cooking Techniques industry, read [How to Craft Perfect Grilled Delicacies using AI-powered Techniques](https://hero.page/blog/ai/cooking-techniques/how-to-craft-perfect-grilled-delicacies-using-ai-powered-techniques/170816)

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
npx hero run ./expert_grill_recipes_ai_creator.heroml
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
hero run ./expert_grill_recipes_ai_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./expert_grill_recipes_ai_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./expert_grill_recipes_ai_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./expert_grill_recipes_ai_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

