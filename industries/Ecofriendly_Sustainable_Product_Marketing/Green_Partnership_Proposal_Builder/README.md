# Green Partnership Proposal Builder

Harness the power of AI with Green Partnership Proposal Builder, designed specifically for creating customized and engaging eco-friendly brand collaboration proposals. This intuitive app enables the user to enter specific variables resulting in personalized, high-quality content. The final result is a comprehensive proposal that vividly describes the environmental impact, sustainability goals, and unique green features of your brand. It smartly aligns your brand's green initiatives with those of potential partners, resulting in a persuasive proposal that encourages further discussion. Exceptional in its focus on promoting sustainability, this app showcases your commitment to our planet and the mutual benefits of an eco-consistent partnership.

To run this app online: [Green Partnership Proposal Builder Online](https://hero.page/app/green-partnership-proposal-builder-eco-friendly-brand-collaboration-builder/hiv4RRtFqpkV66NM4Ran)

[![Run Green Partnership Proposal Builder Online](/assets/run.svg)](https://hero.page/app/green-partnership-proposal-builder-eco-friendly-brand-collaboration-builder/hiv4RRtFqpkV66NM4Ran)

To learn more about AI Apps for Brand Manager use-cases in the Eco-friendly & Sustainable Product Marketing industry, read [How to Amplify Your Eco-friendly Brand Strategy with AI](https://hero.page/blog/ai/eco-friendly-and-sustainable-product-marketing/how-to-amplify-your-eco-friendly-brand-strategy-with-ai/170848)

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
npx hero run ./green_partnership_proposal_builder.heroml
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
hero run ./green_partnership_proposal_builder.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./green_partnership_proposal_builder.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./green_partnership_proposal_builder.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./green_partnership_proposal_builder.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

