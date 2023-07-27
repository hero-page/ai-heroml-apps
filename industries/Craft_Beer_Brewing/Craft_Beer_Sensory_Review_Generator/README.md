# Craft Beer Sensory Review Generator

Craft Beer Sensory Review Generator uses AI to provide custom, detailed reviews of craft beers. Users input variables and the app delivers precise descriptions of appearance, aroma, flavor, and feel. Furthermore, it provides a review and comparison to style expectations along with the beer's alcohol and bitterness levels. This rich information is perfect for Brewmasters and people knowledgeable about beer, offering not just an overview, but a sensory journey.

To run this app online: [Craft Beer Sensory Review Generator Online](https://hero.page/app/craft-beer-sensory-review-generator-ai-powered-detailed-craft-beer-reviews/dN8Yhao6hgw1BYJWTuA5)

[![Run Craft Beer Sensory Review Generator Online](/assets/run.svg)](https://hero.page/app/craft-beer-sensory-review-generator-ai-powered-detailed-craft-beer-reviews/dN8Yhao6hgw1BYJWTuA5)

To learn more about AI Apps for Brewmaster use-cases in the Craft Beer & Brewing industry, read [How to Revolutionize Brewery Workflow with AI Brewing Guide, Beer Review, and Story Creation](https://hero.page/blog/ai/craft-beer-and-brewing/how-to-revolutionize-brewery-workflow-with-ai-brewing-guide-beer-review-and-story-creation/170824)

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
npx hero run ./craft_beer_sensory_review_generator.heroml
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
hero run ./craft_beer_sensory_review_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./craft_beer_sensory_review_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./craft_beer_sensory_review_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./craft_beer_sensory_review_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

