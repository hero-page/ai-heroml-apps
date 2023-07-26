# Essential Oil Descriptor for Aromatherapists

Experience an advanced AI-powered essential oil app designed for aromatherapists. Essential Oil Descriptor lets users specify variables in prompts to generate a custom, in-depth guide for any oil. Uncover aroma profiles, physical features, extraction methods, health benefits, usage, and safety details. It equips users with research-backed, compelling data for professional use, giving it a unique edge over general essential oil apps.

To run this app online: [Essential Oil Descriptor for Aromatherapists Online](https://hero.page/app/essential-oil-descriptor-for-aromatherapists-ai-powered-essential-oil-encyclopedia/mZjdlb4sdatZrLYtdTBo)

[![Run Essential Oil Descriptor for Aromatherapists Online](/assets/run.svg)](https://hero.page/app/essential-oil-descriptor-for-aromatherapists-ai-powered-essential-oil-encyclopedia/mZjdlb4sdatZrLYtdTBo)

To learn more about AI Apps for Aromatherapist use-cases in the Aromatherapy & Essential Oils industry, read [How to Enhance Aromatherapy with AI-Driven Essential Oil Descriptions](https://hero.page/blog/ai/aromatherapy-and-essential-oils/how-to-enhance-aromatherapy-with-ai-driven-essential-oil-descriptions/170729)

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
npx hero run ./essential_oil_descriptor_for_aromatherapists.heroml
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
hero run ./essential_oil_descriptor_for_aromatherapists.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./essential_oil_descriptor_for_aromatherapists.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./essential_oil_descriptor_for_aromatherapists.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./essential_oil_descriptor_for_aromatherapists.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Essential Oil Descriptor for Aromatherapists
```
Your task is to write an "Oil Description" for the "Aromatherapy & Essential Oils" industry, specifically for an "Aromatherapist". Let's start by creating an eye-catching headline that names the oil: {{oil_name}}.

Here's some more context about the Oil Description:
Oil Name: {{oil_name}}
Physical Characteristics: {{physical_characteristics}}
Source Plant: {{source_plant}}
Oil Therapeutic Benefits: {{oil_therapeutic_benefits}}

->>>>

Now, we have a catchy headline for our oil description:

Headline:
{{step_1}}

Next, craft an introduction that provides an overview of the oil, including its origin and first impressions of its scent notes.

->>>>

At this point, for our oil description we have headline and introduction:

Headline:
{{step_1}}

Introduction:
{{step_2}}

Moving on, let's create a detailed aroma profile for the oil by describing top, middle and base notes. Include any unique characteristics. Accompany this with a physical description of the {{oil_name}} which includes its color and consistency.

->>>>

Now, we have our aroma and physical profile:

Introduction:
{{step_2}}

Aroma and Physical profile:
{{step_3}}

Next, let's describe the oil's extraction process. Put emphasis on the method used (such steam distillation, cold press, etc.) and on the source plant {{source_plant}} from which the oil is derived.

->>>>

With our oil description so far:

Aroma and Physical Profile:
{{step_3}}

Extraction Process:
{{step_4}}

Now, let's detail the primary therapeutic benefits and uses of the {{oil_name}}, connected with specific ailments or conditions they could help in.

->>>>

Our oil description so far:

Extraction Process:
{{step_4}}

Therapeutic Benefits and Uses:
{{step_5}}

Next, provide instructions on how to incorporate {{oil_name}} into an aromatherapy practice or routine. This should include any blending suggestions with other oils that could enhance the therapeutic benefits.

->>>>

The oil description has the following sections so far:

Therapeutic Benefits and Uses:
{{step_5}}

Integration into Practice:
{{step_6}}

Now, let's add any safety considerations or contraindications associated with the use of the {{oil_name}}. This will help the aromatherapist ensure that it is used responsibly and effectively. 


```

