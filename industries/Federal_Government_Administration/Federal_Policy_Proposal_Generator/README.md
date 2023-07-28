# Federal Policy Proposal Generator

Boost your policy creation skills with the Federal Policy Proposal Generator. This comprehensive app employs AI to craft tailored policies for the Federal Government Administration. Simply input your variables and watch as the high-quality content unfolds - from an executive summary and thorough economic background to clearly defined goals and in-depth problem analysis. Assure relevance with proposed solutions, justify your proposal, and witness a realistic implementation plan come to life. Finished with an impactful conclusion and an accurate reference list, this is your tool for engaging, informative, well-structured policy proposals.

To run this app online: [Federal Policy Proposal Generator Online](https://hero.page/app/federal-policy-proposal-generator-comprehensive-federal-policy-crafting/WYKTd9S0xwAp1nQvfeob)

[![Run Federal Policy Proposal Generator Online](/assets/run.svg)](https://hero.page/app/federal-policy-proposal-generator-comprehensive-federal-policy-crafting/WYKTd9S0xwAp1nQvfeob)

To learn more about AI Apps for Economic Advisor use-cases in the Federal Government Administration industry, read [How to Elevate Economic Analysis, Policy-Making and Budget Review with AI](https://hero.page/blog/ai/federal-government-administration/how-to-elevate-economic-analysis-policy-making-and-budget-review-with-ai/170872)

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
npx hero run ./federal_policy_proposal_generator.heroml
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
hero run ./federal_policy_proposal_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./federal_policy_proposal_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./federal_policy_proposal_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./federal_policy_proposal_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

