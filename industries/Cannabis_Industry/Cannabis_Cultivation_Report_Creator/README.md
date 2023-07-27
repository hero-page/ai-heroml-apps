# Cannabis Cultivation Report Creator

Cannabis Cultivation Report Creator is a holistic and adaptive app guide for cannabis farming. The AI-driven app allows users to specify details like strain, yields, and cultivation process. It provides an in-depth cultivation guide, covering variables like light, temperature, watering schedules, and pest management. It also includes info on harvesting, drying, and chemical profile testing. The app concludes with a process review and tips for future improvements, all in industry-specific terminology. The app offers comprehensive and specific insights, evolving with user experiences for continual improvement.

To run this app online: [Cannabis Cultivation Report Creator Online](https://hero.page/app/cannabis-cultivation-report-creator-holistic-adaptive-cannabis-farming-guide/KxM47CNKVMt3sAF0aOSt)

[![Run Cannabis Cultivation Report Creator Online](/assets/run.svg)](https://hero.page/app/cannabis-cultivation-report-creator-holistic-adaptive-cannabis-farming-guide/KxM47CNKVMt3sAF0aOSt)

To learn more about AI Apps for Cultivator use-cases in the Cannabis Industry industry, read [How to Elevate Cannabis Cultivation with AI Guide Apps](https://hero.page/blog/ai/cannabis-industry/how-to-elevate-cannabis-cultivation-with-ai-guide-apps/170769)

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
npx hero run ./cannabis_cultivation_report_creator.heroml
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
hero run ./cannabis_cultivation_report_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./cannabis_cultivation_report_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./cannabis_cultivation_report_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./cannabis_cultivation_report_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Cannabis Cultivation Report Creator
```
Your task is to write a "Cultivation Report" for the "Cannabis Industry". 
Start by writing an executive summary that provides an overview of the cultivation cycle: {{cultivation cycle}}. This should briefly touch on the highlights of each section in the report.

Here's some more context about the Cultivation Report:

->>>>

We have an executive summary for our Cultivation Report:

Executive Summary:
{{step_1}}

Now, write an introduction providing a clear definition of the cannabis strain being cultivated: {{cannabis strain}}. You should outline the unique qualities and potential yields of this particular strain.

->>>>

We are drafting a Cultivation Report and have written an introduction for our cannabis strain:

Introduction - Cannabis Strain:
{{step_2}}

Next, details about the growing medium used: {{growing medium}} are required. This section will explain the choice of medium and its potential benefits for the crop's growth and yield.

->>>>

In our Cultivation Report, we have specified the growing medium characteristics:

Growing Medium:
{{step_3}}

Moving on, we need to describe the cultivation process, including critical variables such as light, temperature, and watering schedules, as well as pest and disease management strategies.  Be sure to describe any specific cultivation techniques employed, such as hydroponics, aeroponics, or conventional soil-based cultivation.

->>>>

In the Cultivation Report, we have detailed the cultivation process so far:

Cultivation Process:
{{step_4}}

Let's now write about the harvesting process, focusing on the approximate age at harvest: {{age at harvest}} and the specific cues used to determine the ideal harvest time.

->>>>

We have outlined the harvesting process in our Cultivation Report:

Harvesting Process:
{{step_5}}

It's time to discuss the drying and curing process. This should include detailed descriptions of the environmental conditions (temperature, humidity, darkness), duration, and methods used for both drying and curing.

->>>>

Our Cultivation Report now includes a section on the drying and curing process:

Drying & Curing Process:
{{step_6}}

Next, we will write a section detailing the tests and results regarding the chemical profile of the harvested cannabis, primarily focusing on potency, cannabinoid profile, and contaminant testing.

->>>>

We have covered the testing of harvested cannabis in our Cultivation Report:

Cannabis Testing:
{{step_7}}

To conclude, let's provide a comprehensive review of the cultivation cycle, pointing out any challenges encountered, lessons learned, and potential improvements for future cultivation cycles. The scope for proposals regarding the next cultivation cycle changes or tweaks can be included here.


```

