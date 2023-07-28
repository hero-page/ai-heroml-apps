# Flash Fiction Micro-editing Guide Creator

Experience the power of AI with Flash Fiction Micro-editing Guide Creator app: your key to mastering flash fiction micro-editing. Customize prompts, allowing the AI to craft tailored educational guides on micro-editing within flash fiction. Witness the transformation of an original piece through an easily understandable process, highlighting each edit with a corresponding rationale. Take your skills further with advanced techniques provided exclusively by this unique guide. Immerse in this one-of-a-kind learning experience, designed specifically for those specializing in flash fiction writing and micro-editing.

To run this app online: [Flash Fiction Micro-editing Guide Creator Online](https://hero.page/app/flash-fiction-micro-editing-guide-creator-ai-powered-flash-fiction-micro-editing/pAwJgJfYZnpxm732n6d8)

[![Run Flash Fiction Micro-editing Guide Creator Online](/assets/run.svg)](https://hero.page/app/flash-fiction-micro-editing-guide-creator-ai-powered-flash-fiction-micro-editing/pAwJgJfYZnpxm732n6d8)

To learn more about AI Apps for Editor use-cases in the Flash Fiction Writing industry, read [How to Enhance Flash Fiction Editing with AI-Assisted Tools](https://hero.page/blog/ai/flash-fiction-writing/how-to-enhance-flash-fiction-editing-with-ai-assisted-tools/170880)

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
npx hero run ./flash_fiction_micro_editing_guide_creator.heroml
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
hero run ./flash_fiction_micro_editing_guide_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./flash_fiction_micro_editing_guide_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./flash_fiction_micro_editing_guide_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./flash_fiction_micro_editing_guide_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

