# Italian Cheese Expert Guide Maker

Italian Cheese Expert Guide Maker is an interactive guide that harnesses AI to provide a comprehensive understanding of Italian cheeses. Tailor your prompts to get custom, high-quality, in-depth content on the variety and complexities of Italian cheeses. Learn about the role of cheese in Italian cuisine, the history of cheese-making, regional influences, pairing options, and serving etiquette. Immerse yourself in the authenticity of Italian culture and culinary tradition for a comprehensive learning experience.

To run this app online: [Italian Cheese Expert Guide Maker Online](https://hero.page/app/italian-cheese-expert-guide-maker-authentic-guide:-italian-cheese-mastery/Ypzgz9GkNc36NIzj3Ilk)

[![Run Italian Cheese Expert Guide Maker Online](/assets/run.svg)](https://hero.page/app/italian-cheese-expert-guide-maker-authentic-guide:-italian-cheese-mastery/Ypzgz9GkNc36NIzj3Ilk)

To learn more about AI Apps for Italian Cuisine Expert use-cases in the International Cuisine industry, read [How to Elevate Italian Cuisine with AI-Based Recipe, Cheese and Wine Guides](https://hero.page/blog/ai/international-cuisine/how-to-elevate-italian-cuisine-with-ai-based-recipe-cheese-and-wine-guides/171006)

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
npx hero run ./italian_cheese_expert_guide_maker.heroml
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
hero run ./italian_cheese_expert_guide_maker.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./italian_cheese_expert_guide_maker.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./italian_cheese_expert_guide_maker.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./italian_cheese_expert_guide_maker.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

