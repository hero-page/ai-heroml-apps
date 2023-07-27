# Sous-Vide Expert Equipment Guide Creator

Sous-Vide Expert Equipment Guide Creator is a cutting-edge app that uses AI to generate a personalized guide on top sous-vide cooking equipment. Input your preferences and let the AI analyze basic components, standout features, additional accessories, hygiene essentials, and safety measures. The result? A comprehensive, expert-approved guide on sous-vide cooking equipment. The unique element is the detailed evaluation tailored specifically for experts, ensuring you make the best choice!

To run this app online: [Sous-Vide Expert Equipment Guide Creator Online](https://hero.page/app/sous-vide-expert-equipment-guide-creator-tailored-sous-vide-equipment-analysis/lVzyEZim7E6So3BvRMsC)

[![Run Sous-Vide Expert Equipment Guide Creator Online](/assets/run.svg)](https://hero.page/app/sous-vide-expert-equipment-guide-creator-tailored-sous-vide-equipment-analysis/lVzyEZim7E6So3BvRMsC)

To learn more about AI Apps for Sous-vide Expert use-cases in the Cooking Techniques industry, read [How to Excel in Sous-vide Cooking with AI Apps](https://hero.page/blog/ai/cooking-techniques/how-to-excel-in-sous-vide-cooking-with-ai-apps/170818)

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
npx hero run ./sous_vide_expert_equipment_guide_creator.heroml
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
hero run ./sous_vide_expert_equipment_guide_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./sous_vide_expert_equipment_guide_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./sous_vide_expert_equipment_guide_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./sous_vide_expert_equipment_guide_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

