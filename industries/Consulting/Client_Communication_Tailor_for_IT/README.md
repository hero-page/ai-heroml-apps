# Client Communication Tailor for IT

Client Communication Tailor for IT revolutionizes the way IT consultants communicate with their clients. Offering personalized communication tools powered by AI, this app lets users specify variables for the generation of high-quality, bespoke content. Whether it's professional emails detailing proposed IT services, technology updates or discussing their benefits, the app crafts the perfect message for you. The standout feature uniquely tailors technical language to suit your client's understanding level, facilitating engagement and comprehension, turning complex IT lingo into easily digestible content.

To run this app online: [Client Communication Tailor for IT Online](https://hero.page/app/client-communication-tailor-for-it-personalized-it-solutions-communication/A0LGLnYNAGKpoqjfMFb7)

[![Run Client Communication Tailor for IT Online](/assets/run.svg)](https://hero.page/app/client-communication-tailor-for-it-personalized-it-solutions-communication/A0LGLnYNAGKpoqjfMFb7)

To learn more about AI Apps for IT Consultant use-cases in the Consulting industry, read [How to Streamline IT Consulting with AI Tools for Audit, Proposals and Client Communication](https://hero.page/blog/ai/consulting/how-to-streamline-it-consulting-with-ai-tools-for-audit-proposals-and-client-communication/170812)

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
npx hero run ./client_communication_tailor_for_it.heroml
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
hero run ./client_communication_tailor_for_it.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./client_communication_tailor_for_it.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./client_communication_tailor_for_it.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./client_communication_tailor_for_it.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

