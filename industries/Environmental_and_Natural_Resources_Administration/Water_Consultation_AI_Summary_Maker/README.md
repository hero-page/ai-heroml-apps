# Water Consultation AI Summary Maker

Water Consultation AI Summary Maker is a revolutionary tool that enhances your ability to generate comprehensive reports on public consultations for water resource management. Utilizing AI technology, this app allows you to define variables to create tailored, high-quality content that provides an accurate summary of the consultation's purpose, background, objectives, methodology, and key findings. The app aims for transparency, inclusivity and balance in presentation, catering to both technical and non-technical audiences. Its uniqueness lies in its focus on water resource management within public consultations. It gives comprehensive output, outlining detailed management plans, and determining future steps.

To run this app online: [Water Consultation AI Summary Maker Online](https://hero.page/app/water-consultation-ai-summary-maker-ai-powered-water-resource-consultation/MPsttmL2xaZDB3t9BZbI)

[![Run Water Consultation AI Summary Maker Online](/assets/run.svg)](https://hero.page/app/water-consultation-ai-summary-maker-ai-powered-water-resource-consultation/MPsttmL2xaZDB3t9BZbI)

To learn more about AI Apps for Water Resource Specialist use-cases in the Environmental and Natural Resources Administration industry, read [How to Enhance Water Management with AI Tools](https://hero.page/blog/ai/environmental-and-natural-resources-administration/how-to-enhance-water-management-with-ai-tools/170860)

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
npx hero run ./water_consultation_ai_summary_maker.heroml
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
hero run ./water_consultation_ai_summary_maker.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./water_consultation_ai_summary_maker.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./water_consultation_ai_summary_maker.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./water_consultation_ai_summary_maker.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```

