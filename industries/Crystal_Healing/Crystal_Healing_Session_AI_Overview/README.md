# Crystal Healing Session AI Overview

Experience a guided walkthrough of crystal healing through the Crystal Healing Session AI Overview app. Powered by AI, this app generates rich, chronological narratives of crystal healing sessions, from preparation to reflection. Adjust variables to personalize content, delve into healing techniques, observe client reactions, and receive AI recommendations on the following steps. Read engaging narratives that merge informative content and conversational style, creating a unique, immersive healing journey.

To run this app online: [Crystal Healing Session AI Overview Online](https://hero.page/app/crystal-healing-session-ai-overview-ai-powered-crystal-healing-narrative/ewPyDuMW5fClQCoPbEGP)

[![Run Crystal Healing Session AI Overview Online](/assets/run.svg)](https://hero.page/app/crystal-healing-session-ai-overview-ai-powered-crystal-healing-narrative/ewPyDuMW5fClQCoPbEGP)

To learn more about AI Apps for Crystal Healer use-cases in the Crystal Healing industry, read [How to Generate Informative Crystal Guides and Testimonials with AI](https://hero.page/blog/ai/crystal-healing/how-to-generate-informative-crystal-guides-and-testimonials-with-ai/170830)

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
npx hero run ./crystal_healing_session_ai_overview.heroml
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
hero run ./crystal_healing_session_ai_overview.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./crystal_healing_session_ai_overview.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./crystal_healing_session_ai_overview.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./crystal_healing_session_ai_overview.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

