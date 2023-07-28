# Detailed Story Critique for Editors

Detailed Story Critique for Editors, an AI-powered flash fiction analysis tool, lets you specify customization variables. Harness the AI's ability to create high-quality content such as the in-depth critique of a flash fiction piece meant for editors. The app uses AI to assess narrative structure, character development, language style, theme, and effectiveness of the ending. Moreover, it provides encouragement to the author, highlighting positive aspects while suggesting improvements. Tailor-made for editors, this app offers a comprehensive analysis of each story while maintaining a constructive approach.

To run this app online: [Detailed Story Critique for Editors Online](https://hero.page/app/detailed-story-critique-for-editors-ai-powered-tailored-flash-fiction-analysis/iohYlP1zubyKgPNtgKkB)

[![Run Detailed Story Critique for Editors Online](/assets/run.svg)](https://hero.page/app/detailed-story-critique-for-editors-ai-powered-tailored-flash-fiction-analysis/iohYlP1zubyKgPNtgKkB)

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
npx hero run ./detailed_story_critique_for_editors.heroml
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
hero run ./detailed_story_critique_for_editors.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./detailed_story_critique_for_editors.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./detailed_story_critique_for_editors.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./detailed_story_critique_for_editors.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

