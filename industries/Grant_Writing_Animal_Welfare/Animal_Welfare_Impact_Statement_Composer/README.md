# Animal Welfare Impact Statement Composer

Animal Welfare Impact Statement Composer is a user-friendly, AI-driven tool designed to generate high-quality, customized content for animal welfare project proposals. This time-saving app allows users to specify various variables in prompts, leading to a detailed explanation of the project's purpose, methodology, and anticipated effects on animal welfare. Its unique attribute is the inclusion of an evaluation plan, offering a practical assessment of your project's outcomes, metrics, and alignment with project goals. Plus, it strengthens your proposal by citing references, enhancing credibility.

To run this app online: [Animal Welfare Impact Statement Composer Online](https://hero.page/app/animal-welfare-impact-statement-composer-ai-driven-animal-welfare-evaluation-tool/B2mTiAO8k2NtfUTm7HXi)

[![Run Animal Welfare Impact Statement Composer Online](/assets/run.svg)](https://hero.page/app/animal-welfare-impact-statement-composer-ai-driven-animal-welfare-evaluation-tool/B2mTiAO8k2NtfUTm7HXi)

To learn more about AI Apps for Grant Writer use-cases in the Grant Writing - Animal Welfare industry, read [How to Streamline Animal Welfare Grants with AI Tools](https://hero.page/blog/ai/grant-writing-animal-welfare/how-to-streamline-animal-welfare-grants-with-ai-tools/170903)

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
npx hero run ./animal_welfare_impact_statement_composer.heroml
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
hero run ./animal_welfare_impact_statement_composer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./animal_welfare_impact_statement_composer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./animal_welfare_impact_statement_composer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./animal_welfare_impact_statement_composer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

