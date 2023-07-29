# Education Grant Writer's AI Assistant

Experience the future of grant writing with the Education Grant Writer's AI Assistant. This remarkable app, powered by advanced AI technology, is specifically designed for the Grant Writing - Education Institutions industry. Utilize variable prompts to create a comprehensive Funding Needs Statement that vividly explains your project, asserts its alignment with educational goals, and details the financial requirements. The app generates a detailed projection of both potential benefits and consequences. Highlight the significance of your project with high-quality, persuasive content that appeals to grant providers.

To run this app online: [Education Grant Writer's AI Assistant Online](https://hero.page/app/education-grant-writer's-ai-assistant-ai-powered-grant-writing-assistance/uW0PkqaOccGbJMF34mIf)

[![Run Education Grant Writer's AI Assistant Online](/assets/run.svg)](https://hero.page/app/education-grant-writer's-ai-assistant-ai-powered-grant-writing-assistance/uW0PkqaOccGbJMF34mIf)

To learn more about AI Apps for Grant Writer use-cases in the Grant Writing - Education Institutions industry, read [How to Elevate Grant Writing for Education with AI Tools](https://hero.page/blog/ai/grant-writing-education-institutions/how-to-elevate-grant-writing-for-education-with-ai-tools/170911)

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
npx hero run ./education_grant_writers_ai_assistant.heroml
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
hero run ./education_grant_writers_ai_assistant.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./education_grant_writers_ai_assistant.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./education_grant_writers_ai_assistant.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./education_grant_writers_ai_assistant.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

