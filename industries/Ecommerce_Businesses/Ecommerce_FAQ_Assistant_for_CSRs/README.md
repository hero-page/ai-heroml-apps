# E-commerce FAQ Assistant for CSRs

E-commerce FAQ Assistant for CSRs is an AI-powered tool that equips Customer Service Reps with comprehensive FAQ guidelines. Users can define variables in prompts for specialized content. This app's AI generates rich content, such as detailed responses for common customer inquiries about ordering, payment, shipping, delivery etc. Features also include troubleshooting guidelines for the platform, insight on company's return/refund policy, and contact information. Tailored to assist CSRs in e-commerce sector, the content is not only informative but also friendly to guide them in their interaction with customers. Updates are provided regularly to keep up with evolving customer concerns.

To run this app online: [E-commerce FAQ Assistant for CSRs Online](https://hero.page/app/e-commerce-faq-assistant-for-csrs-ai-powered-e-commerce-faq-guide/jwUYZepHVDaiAbm2jS2d)

[![Run E-commerce FAQ Assistant for CSRs Online](/assets/run.svg)](https://hero.page/app/e-commerce-faq-assistant-for-csrs-ai-powered-e-commerce-faq-guide/jwUYZepHVDaiAbm2jS2d)

To learn more about AI Apps for Customer Service Rep use-cases in the E-commerce Businesses industry, read [How to Transform E-commerce Customer Service with AI Tools](https://hero.page/blog/ai/e-commerce-businesses/how-to-transform-e-commerce-customer-service-with-ai-tools/170845)

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
npx hero run ./e_commerce_faq_assistant_for_csrs.heroml
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
hero run ./e_commerce_faq_assistant_for_csrs.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./e_commerce_faq_assistant_for_csrs.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./e_commerce_faq_assistant_for_csrs.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./e_commerce_faq_assistant_for_csrs.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

