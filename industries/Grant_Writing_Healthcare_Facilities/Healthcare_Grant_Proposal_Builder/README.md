# Healthcare Grant Proposal Builder

Healthcare Grant Proposal Builder is your AI-powered guide for crafting superior healthcare grant proposals. This app allows users to specify variables based on specific healthcare realm, be it pediatrics, public health, cancer research or geriatrics. Its AI technology generates a full-fledged proposal with a summary, background, research purpose, detailed methodology, team information, comprehensive budget, risk prevention methods, project timeline and a concrete conclusion. It also embeds relevant industry statistics, citations, and professional language to demonstrate strong healthcare knowledge. A unique feature is its explicit instructions to structure a persuasive grant proposal.

To run this app online: [Healthcare Grant Proposal Builder Online](https://hero.page/app/healthcare-grant-proposal-builder-comprehensive-ai-powered-grant-builder/aKwfuWPPe4VqLBw7lUhQ)

[![Run Healthcare Grant Proposal Builder Online](/assets/run.svg)](https://hero.page/app/healthcare-grant-proposal-builder-comprehensive-ai-powered-grant-builder/aKwfuWPPe4VqLBw7lUhQ)

To learn more about AI Apps for Grant Writer use-cases in the Grant Writing - Healthcare Facilities industry, read [How to Optimize Grant Writing in Healthcare with AI Tools](https://hero.page/blog/ai/grant-writing-healthcare-facilities/how-to-optimize-grant-writing-in-healthcare-with-ai-tools/170915)

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
npx hero run ./healthcare_grant_proposal_builder.heroml
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
hero run ./healthcare_grant_proposal_builder.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./healthcare_grant_proposal_builder.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./healthcare_grant_proposal_builder.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./healthcare_grant_proposal_builder.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

