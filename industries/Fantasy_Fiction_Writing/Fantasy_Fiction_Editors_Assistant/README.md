# Fantasy Fiction Editor's Assistant

Unleash your storytelling potential with Fantasy Fiction Editor's Assistant, an AI-powered app designed to offer a comprehensive critique of your fantasy manuscript. It intelligently pinpoints key aspects like narrative premise, fantasy elements, world-building, character development, plot points, and language use. Moreover, it focuses on genre-specific factors, providing in-depth feedback for conflict resolution, general observations, and revision suggestions. An all-inclusive tool made specially for fantasy authors to enhance their work.

To run this app online: [Fantasy Fiction Editor's Assistant Online](https://hero.page/app/fantasy-fiction-editor's-assistant-ai-powered-fantasy-manuscript-critique/j7fNWg6OBxwU3qmqHnST)

[![Run Fantasy Fiction Editor's Assistant Online](/assets/run.svg)](https://hero.page/app/fantasy-fiction-editor's-assistant-ai-powered-fantasy-manuscript-critique/j7fNWg6OBxwU3qmqHnST)

To learn more about AI Apps for Editor use-cases in the Fantasy Fiction Writing industry, read [How to Enhance Editorial Feedback in Fantasy Fiction with AI](https://hero.page/blog/ai/fantasy-fiction-writing/how-to-enhance-editorial-feedback-in-fantasy-fiction-with-ai/170865)

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
npx hero run ./fantasy_fiction_editors_assistant.heroml
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
hero run ./fantasy_fiction_editors_assistant.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./fantasy_fiction_editors_assistant.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./fantasy_fiction_editors_assistant.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./fantasy_fiction_editors_assistant.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

