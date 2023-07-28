# Bank Teller Procedure Generator

Introducing Bank Teller Procedure Generator, an AI-driven app that enhances the efficiency of banking procedures. Users can input variables to generate a detailed, tailored guide for bank tellers. The content includes teller roles, responsibilities, banking operations such as deposits, withdrawals, and currency exchange, cash and non-cash transaction handling, and customer service pointers. It also offers strategies for identifying and dealing with suspicious transactions. The app's prowess lies in its detailed insight into the financial services industry, offering tellers explicit steps to enhance their job performance.

To run this app online: [Bank Teller Procedure Generator Online](https://hero.page/app/bank-teller-procedure-generator-ai-powered-teller-operations-guide/Z6oUdvuOx89F6YQwyCvB)

[![Run Bank Teller Procedure Generator Online](/assets/run.svg)](https://hero.page/app/bank-teller-procedure-generator-ai-powered-teller-operations-guide/Z6oUdvuOx89F6YQwyCvB)

To learn more about AI Apps for Bank Teller use-cases in the Financial Services industry, read [How to Streamline Banking Tasks with AI-Generated Solutions](https://hero.page/blog/ai/financial-services/how-to-streamline-banking-tasks-with-ai-generated-solutions/170878)

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
npx hero run ./bank_teller_procedure_generator.heroml
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
hero run ./bank_teller_procedure_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./bank_teller_procedure_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./bank_teller_procedure_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./bank_teller_procedure_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

