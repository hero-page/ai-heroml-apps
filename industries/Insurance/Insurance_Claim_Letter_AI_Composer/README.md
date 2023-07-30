# Insurance Claim Letter AI Composer

Use the Insurance Claim Letter AI Composer to generate customized, high-quality insurance claim letters. The app, powered by AI, lets users specify multiple variables for personalized content. The final output will be a comprehensive insurance claim letter including personal and policy information. It offers a clear account of the insured event, articulating losses or expenses, and details of supporting documents provided. Specifically, the app’s uniqueness lies in detailing the insured event and associated losses, presenting credible claim. The letter concludes elegantly, affirms readiness to share more details, and includes a signature and contact details.

To run this app online: [Insurance Claim Letter AI Composer Online](https://hero.page/app/insurance-claim-letter-ai-composer-ai-powered-detailed-claims-composer/SsiEIj9X6RMMmdvN3ytJ)

[![Run Insurance Claim Letter AI Composer Online](/assets/run.svg)](https://hero.page/app/insurance-claim-letter-ai-composer-ai-powered-detailed-claims-composer/SsiEIj9X6RMMmdvN3ytJ)

To learn more about AI Apps for Insurance Agent use-cases in the Insurance industry, read [How to Revolutionize Insurance Documentation with HeroML AI Apps](https://hero.page/blog/ai/insurance/how-to-revolutionize-insurance-documentation-with-heroml-ai-apps/171000)

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
npx hero run ./insurance_claim_letter_ai_composer.heroml
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
hero run ./insurance_claim_letter_ai_composer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./insurance_claim_letter_ai_composer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./insurance_claim_letter_ai_composer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./insurance_claim_letter_ai_composer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

