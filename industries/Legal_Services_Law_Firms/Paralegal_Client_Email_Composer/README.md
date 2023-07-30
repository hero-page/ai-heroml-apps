# Paralegal Client Email Composer

The Paralegal Client Email Composer is an AI-powered tool specifically designed for the legal services and law firms industry. This app generates professional and detailed emails that address the client's legal case, providing an overview, outlining the next steps, crucial deadlines, and offering further assistance. It elevates standard communication by incorporating legal terminologies and procedures, creating content that instills confidence and commitment to the client's case.

To run this app online: [Paralegal Client Email Composer Online](https://hero.page/app/paralegal-client-email-composer-ai-powered-legal-email-composer/SbnvAOzRhHvwZgw85sO2)

[![Run Paralegal Client Email Composer Online](/assets/run.svg)](https://hero.page/app/paralegal-client-email-composer-ai-powered-legal-email-composer/SbnvAOzRhHvwZgw85sO2)

To learn more about AI Apps for Paralegal use-cases in the Legal Services & Law Firms industry, read [How to Streamline Paralegal Tasks with AI for Legal Services](https://hero.page/blog/ai/legal-services-and-law-firms/how-to-streamline-paralegal-tasks-with-ai-for-legal-services/171015)

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
npx hero run ./paralegal_client_email_composer.heroml
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
hero run ./paralegal_client_email_composer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./paralegal_client_email_composer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./paralegal_client_email_composer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./paralegal_client_email_composer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

