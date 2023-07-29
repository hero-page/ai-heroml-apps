# Animal Rescue Grant Proposal Generator

The Animal Rescue Grant Proposal Generator, an AI-powered app, allows users to input specific variables to generate tailored proposals. It utilizes advanced AI to create high-quality content that encompasses an executive summary, organization introduction, detailed animal welfare analysis, defined project proposal, strategic action plan, well-structured budgetary needs, and an enticing conclusion. The standout feature is the in-depth, well-organized rescue project proposal, reflecting a comprehensive understanding of the issue and a clear plan-of-action. The app ensures alignment with funder's objectives and professionalism throughout the document, promoting potential funding success.

To run this app online: [Animal Rescue Grant Proposal Generator Online](https://hero.page/app/animal-rescue-grant-proposal-generator-ai-powered-animal-rescue-proposal-writer/k6ZdmiNbV6IAxEHotWur)

[![Run Animal Rescue Grant Proposal Generator Online](/assets/run.svg)](https://hero.page/app/animal-rescue-grant-proposal-generator-ai-powered-animal-rescue-proposal-writer/k6ZdmiNbV6IAxEHotWur)

To learn more about AI Apps for Grant Writer use-cases in the Grant Writing - Animal Welfare industry, read [How to Streamline Animal Welfare Grants with AI Tools](https://hero.page/blog/ai/grant-writing-animal-welfare/how-to-streamline-animal-welfare-grants-with-ai-tools/170903)

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
npx hero run ./animal_rescue_grant_proposal_generator.heroml
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
hero run ./animal_rescue_grant_proposal_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./animal_rescue_grant_proposal_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./animal_rescue_grant_proposal_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./animal_rescue_grant_proposal_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

