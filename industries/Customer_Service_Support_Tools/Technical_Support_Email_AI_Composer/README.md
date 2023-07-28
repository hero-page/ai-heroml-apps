# Technical Support Email AI Composer

The Technical Support Email AI Composer aids in creating custom tech support emails. This innovative app uses AI to craft professional and courteous responses to your customers’ technical issues. Input your specifics and watch it work! Whether you need to detail a resolution process, give instructions, request more info, or express gratitude, this app has it covered. Noteworthy feature? It personalizes messages with details of problem-solving steps, assuring high-level expertise from the support specialist. No more generic emails, make your customers feel valued and ensure their loyalty.

To run this app online: [Technical Support Email AI Composer Online](https://hero.page/app/technical-support-email-ai-composer-ai-crafted-custom-tech-support-emails/F2QO5BYZPHPWtbJhnedc)

[![Run Technical Support Email AI Composer Online](/assets/run.svg)](https://hero.page/app/technical-support-email-ai-composer-ai-crafted-custom-tech-support-emails/F2QO5BYZPHPWtbJhnedc)

To learn more about AI Apps for Technical Support Specialist use-cases in the Customer Service & Support Tools industry, read [How to Automate Troubleshooting Guide, Knowledge Base, and Email with AI](https://hero.page/blog/ai/customer-service-and-support-tools/how-to-automate-troubleshooting-guide-knowledge-base-and-email-with-ai/170837)

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
npx hero run ./technical_support_email_ai_composer.heroml
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
hero run ./technical_support_email_ai_composer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./technical_support_email_ai_composer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./technical_support_email_ai_composer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./technical_support_email_ai_composer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

