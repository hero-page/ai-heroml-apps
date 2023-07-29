# Grant Writer's Literature Review AI

Grant Writer's Literature Review AI is a powerful solution for researchers and institutions engaged in grant writing. By allowing users to specify variables, it generates tailored, high-quality content for literature reviews that elegantly aligns the research topic with grant objectives. It uses smart AI capabilities to provide detailed and critical analysis of existing literature, highlighting research gaps that your project aims to fill and the potential impact. The focus is not just on academic comprehension, but also on making a compelling case for funding necessity. Furthermore, the app incorporates industry-specific terminology and procedures, as well as details of previously funded similar projects. Thus, this tool is not only a research aid but a strategic ally in securing research funding.

To run this app online: [Grant Writer's Literature Review AI Online](https://hero.page/app/grant-writer's-literature-review-ai-strategic-grant-focused-literature-reviews/l4BsKTKxUSQgwpUxJuBL)

[![Run Grant Writer's Literature Review AI Online](/assets/run.svg)](https://hero.page/app/grant-writer's-literature-review-ai-strategic-grant-focused-literature-reviews/l4BsKTKxUSQgwpUxJuBL)

To learn more about AI Apps for Grant Writer use-cases in the Grant Writing - Research Institutions industry, read [How to Elevate Grant Proposals with AI for Research Project Success](https://hero.page/blog/ai/grant-writing-research-institutions/how-to-elevate-grant-proposals-with-ai-for-research-project-success/170929)

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
npx hero run ./grant_writers_literature_review_ai.heroml
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
hero run ./grant_writers_literature_review_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./grant_writers_literature_review_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./grant_writers_literature_review_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./grant_writers_literature_review_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

