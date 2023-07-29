# Historical Figure Bio-Study Guide

The Historical Figure Bio-Study Guide app utilizes AI innovation to produce personalized, quality content about your chosen historical figure. Delve into their life events, beliefs, legacy, and controversies. It's also a high school study guide, offering balanced discussions on the figure's impact. The app presents an in-depth reading list, turning it into a profound source of information for those eager to explore history further.

To run this app online: [Historical Figure Bio-Study Guide Online](https://hero.page/app/historical-figure-bio-study-guide-ai-powered-bio-analysis-and-study-guide/EuWm3POzHRV2CbHBkRrH)

[![Run Historical Figure Bio-Study Guide Online](/assets/run.svg)](https://hero.page/app/historical-figure-bio-study-guide-ai-powered-bio-analysis-and-study-guide/EuWm3POzHRV2CbHBkRrH)

To learn more about AI Apps for History Club Member use-cases in the High School Students - Social Sciences industry, read [How to Craft Historical Content with AI for High School History Clubs](https://hero.page/blog/ai/high-school-students-social-sciences/how-to-craft-historical-content-with-ai-for-high-school-history-clubs/170968)

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
npx hero run ./historical_figure_bio_study_guide.heroml
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
hero run ./historical_figure_bio_study_guide.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./historical_figure_bio_study_guide.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./historical_figure_bio_study_guide.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./historical_figure_bio_study_guide.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

