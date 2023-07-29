# Cultural Grant Proposal Generator

The Cultural Grant Proposal Generator, an AI-powered writer creating high-quality, custom content, offers a platform for generating comprehensive proposals for cultural events. Users can input variables for AI to formulate seamless content including event significance, demographics, schedules, marketing strategies, and detailed budgeting. It notably provides an outstanding justification for grant funding, demonstrating not only the event's value but also a wise and practical investment, thereby boosting your proposal's credibility and chances of success.

To run this app online: [Cultural Grant Proposal Generator Online](https://hero.page/app/cultural-grant-proposal-generator-ai-powered-grant-proposal-writer/k5EjizhDGa81pec4UHo1)

[![Run Cultural Grant Proposal Generator Online](/assets/run.svg)](https://hero.page/app/cultural-grant-proposal-generator-ai-powered-grant-proposal-writer/k5EjizhDGa81pec4UHo1)

To learn more about AI Apps for Grant Writer use-cases in the Grant Writing - Cultural Organizations industry, read [How to Innovate Grant Writing with AI for Cultural Events](https://hero.page/blog/ai/grant-writing-cultural-organizations/how-to-innovate-grant-writing-with-ai-for-cultural-events/170909)

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
npx hero run ./cultural_grant_proposal_generator.heroml
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
hero run ./cultural_grant_proposal_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./cultural_grant_proposal_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./cultural_grant_proposal_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./cultural_grant_proposal_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

