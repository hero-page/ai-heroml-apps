# Copywriter's Email Marketing Newsletter AI

The Copywriter's Email Marketing Newsletter AI app generates customized newsletters for email marketing copywriters, providing tailor-made content on prime industry topics, recent news, and a valuable toolkit. The app uses Artificial Intelligence to craft data-driven, high-quality content that is interactive, aids professional growth, and builds reader engagement. User-specified inputs customize each newsletter for optimized value and relevance to the reader. The output is not just generic information but detailed analysis, expert insights, and a spotlight on industry events– adding substantial worth to the reader journey.

To run this app online: [Copywriter's Email Marketing Newsletter AI Online](https://hero.page/app/copywriter's-email-marketing-newsletter-ai-ai-crafted-email-marketing-insights/1piIHCU1pmuHkx1O3hB4)

[![Run Copywriter's Email Marketing Newsletter AI Online](/assets/run.svg)](https://hero.page/app/copywriter's-email-marketing-newsletter-ai-ai-crafted-email-marketing-insights/1piIHCU1pmuHkx1O3hB4)

To learn more about AI Apps for Copywriter use-cases in the Email Marketing Services industry, read [How to Elevate Email Marketing with AI-Driven Copywriting Tools](https://hero.page/blog/ai/email-marketing-services/how-to-elevate-email-marketing-with-ai-driven-copywriting-tools/170856)

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
npx hero run ./copywriters_email_marketing_newsletter_ai.heroml
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
hero run ./copywriters_email_marketing_newsletter_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./copywriters_email_marketing_newsletter_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./copywriters_email_marketing_newsletter_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./copywriters_email_marketing_newsletter_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

