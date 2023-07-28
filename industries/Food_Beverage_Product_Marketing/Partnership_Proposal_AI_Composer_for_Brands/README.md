# Partnership Proposal AI Composer for Brands

The Partnership Proposal AI Composer for Brands app enables you to generate highly personalized partnership proposals. Use variables to guide AI in crafting content just for you. The final output is a comprehensive proposal, designed for the food & beverage product marketing industry, ensuring the interests a brand manager align with yours. The unique attribute? An in-depth, tailored approach that aims to define, present, and implement clear benefits to boost market visibility, expand customer base, and encourage innovation.

To run this app online: [Partnership Proposal AI Composer for Brands Online](https://hero.page/app/partnership-proposal-ai-composer-for-brands-ai-powered-personalized-partnership-proposals/wEsDp1ZSbz2yLI25sKtE)

[![Run Partnership Proposal AI Composer for Brands Online](/assets/run.svg)](https://hero.page/app/partnership-proposal-ai-composer-for-brands-ai-powered-personalized-partnership-proposals/wEsDp1ZSbz2yLI25sKtE)

To learn more about AI Apps for Brand Manager use-cases in the Food & Beverage Product Marketing industry, read [How to Innovate Food & Beverage Marketing with AI Tools](https://hero.page/blog/ai/food-and-beverage-product-marketing/how-to-innovate-food-and-beverage-marketing-with-ai-tools/170884)

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
npx hero run ./partnership_proposal_ai_composer_for_brands.heroml
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
hero run ./partnership_proposal_ai_composer_for_brands.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./partnership_proposal_ai_composer_for_brands.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./partnership_proposal_ai_composer_for_brands.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./partnership_proposal_ai_composer_for_brands.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

