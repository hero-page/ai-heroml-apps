# Vendor Engagement Email Generator

Vendor Engagement Email Generator, defined by its subtitle, AI-Powered Professional Vendor Communication, simplifies your vendor outreach. Use this tool to formulate detailed, professional emails for your event planning needs. Define your context and watch as the app's AI engine produces a high-quality, tailored email. With its comprehensive framework, the final email not only introduces you but clearly articulates your needs, reasons for choosing the vendor, and requests a meeting, maintaining an optimistic tone throughout. Standout in your business communication with this distinct tool.

To run this app online: [Vendor Engagement Email Generator Online](https://hero.page/app/vendor-engagement-email-generator-ai-powered-professional-vendor-communication/YCKt60aO2RJQZPFZiYag)

[![Run Vendor Engagement Email Generator Online](/assets/run.svg)](https://hero.page/app/vendor-engagement-email-generator-ai-powered-professional-vendor-communication/YCKt60aO2RJQZPFZiYag)

To learn more about AI Apps for Event Planner use-cases in the Event Management & Promotion industry, read [How to Amplify Event Planning with Key AI Tools](https://hero.page/blog/ai/event-management-and-promotion/how-to-amplify-event-planning-with-key-ai-tools/170861)

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
npx hero run ./vendor_engagement_email_generator.heroml
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
hero run ./vendor_engagement_email_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./vendor_engagement_email_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./vendor_engagement_email_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./vendor_engagement_email_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

