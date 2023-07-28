# Event CSR Policy AI Builder

Event CSR Policy AI Builder, an AI-powered tool, allows users to set specific variables in prompts to generate premium, customized content. Aimed to form an exhaustive policy manual for Customer Service Representatives in the Event Management & Promotion industry—it provides clear outlines for policy objectives, scope, details, roles, and responsibilities. With unique focus on industry-specific elements, comprehending consequences of non-compliance, resources, support, and the necessity of employee acknowledgment—this app ensures industry-centric compliance and the highest-quality service delivery.

To run this app online: [Event CSR Policy AI Builder Online](https://hero.page/app/event-csr-policy-ai-builder-ai-powered-event-csr-policy-builder/7b9KpBuW5xgdN8j53cd5)

[![Run Event CSR Policy AI Builder Online](/assets/run.svg)](https://hero.page/app/event-csr-policy-ai-builder-ai-powered-event-csr-policy-builder/7b9KpBuW5xgdN8j53cd5)

To learn more about AI Apps for Customer Service Representative use-cases in the Event Management & Promotion industry, read [How to Innovate Event Management with AI for Ticket Info and FAQs](https://hero.page/blog/ai/event-management-and-promotion/how-to-innovate-event-management-with-ai-for-ticket-info-and-faqs/170863)

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
npx hero run ./event_csr_policy_ai_builder.heroml
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
hero run ./event_csr_policy_ai_builder.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./event_csr_policy_ai_builder.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./event_csr_policy_ai_builder.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./event_csr_policy_ai_builder.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

