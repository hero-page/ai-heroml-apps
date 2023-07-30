# Claims Adjuster Letter Tailor

Claims Adjuster Letter Tailor leverages AI to generate highly customized insurance claim correspondence. Tailor each letter to your client's unique circumstances, complete with detailed claims information, technical term explanations, support, and contact details. Experience the unique blend of factual claim details and empathic communication in industry-specific language. This app ensures client comprehension and satisfaction throughout the claims process.

To run this app online: [Claims Adjuster Letter Tailor Online](https://hero.page/app/claims-adjuster-letter-tailor-personalized-ai-insurance-claim-correspondence/mjtCqF2QjUORnABOtQTa)

[![Run Claims Adjuster Letter Tailor Online](/assets/run.svg)](https://hero.page/app/claims-adjuster-letter-tailor-personalized-ai-insurance-claim-correspondence/mjtCqF2QjUORnABOtQTa)

To learn more about AI Apps for Claims Adjuster use-cases in the Insurance Agencies industry, read [How to Automate Insurance Claim Workflow using AI Apps](https://hero.page/blog/ai/insurance-agencies/how-to-automate-insurance-claim-workflow-using-ai-apps/171004)

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
npx hero run ./claims_adjuster_letter_tailor.heroml
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
hero run ./claims_adjuster_letter_tailor.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./claims_adjuster_letter_tailor.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./claims_adjuster_letter_tailor.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./claims_adjuster_letter_tailor.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

