# Brand Visual Identity Analyzer

Our Brand Visual Identity Analyzer app leverages AI technology to deliver custom insights into your brand's visual identity. Specify variables, and the app will generate a detailed report analyzing your brand's visual traits, logo, color palette, typography, and imagery alignment. Gain in-depth knowledge on how your brand sets itself apart visually, contributing to a unique and strong identity in the Brand Consultancies industry. The app's unique feature is its ability to align visual elements with brand's image and traits, enhancing brand recognizability.

To run this app online: [Brand Visual Identity Analyzer Online](https://hero.page/app/brand-visual-identity-analyzer-ai-powered-brand-identity-analysis/IMU1Eq8WSYQTrlpaGgVf)

[![Run Brand Visual Identity Analyzer Online](/assets/run.svg)](https://hero.page/app/brand-visual-identity-analyzer-ai-powered-brand-identity-analysis/IMU1Eq8WSYQTrlpaGgVf)

To learn more about AI Apps for Graphic Designer use-cases in the Brand Consultancies industry, read [How to Streamline Brand Design Workflow with AI Tools](https://hero.page/blog/ai/brand-consultancies/how-to-streamline-brand-design-workflow-with-ai-tools/170765)

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
npx hero run ./brand_visual_identity_analyzer.heroml
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
hero run ./brand_visual_identity_analyzer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./brand_visual_identity_analyzer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./brand_visual_identity_analyzer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./brand_visual_identity_analyzer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Brand Visual Identity Analyzer
```
Your task is to write a "Visual Identity Description" for the "Brand Consultancies" industry, specifically for a "Graphic Designer". 

Let's start by writing an introduction that overviews the brand traits: {{brand_traits}}.

Here's some more context about the Visual Identity Description:
Brand Traits: {{brand_traits}}
Visual Elements: {{visual_elements}}
Color Palette: {{color_palette}}
Typography Details: {{typography_details}}
Imagery Standard: {{imagery_standard}}

->>>>

We have an introduction for our "Visual Identity Description":

Introduction Overviewing Brand Traits:
{{step_1}}

Now, introduce the visual elements of the brand which includes the logo, color palette, typography, and imagery. Make sure each one is described uniquely: {{visual_elements}}.

->>>>

We have an introduction and unique descriptions for the visual elements of our brand:

Introduction Overviewing Brand Traits:
{{step_1}}

Described Visual Elements:
{{step_2}}

Next, delve into a detailed description of the primary logo of the brand. Explain how it represents the brand traits: {{brand_traits}}.

->>>>

Our "Visual Identity Description" now includes an introduction, described visual elements, and a description of the primary logo:

Introduction Overviewing Brand Traits:
{{step_1}}

Described Visual Elements:
{{step_2}}

Primary Logo Description representing Brand Traits:
{{step_3}}

Now, describe the color palette used in the brand's visuals. Highlight the chosen hues and any symbolism they carry in respect to the brand: {{color_palette}}.

->>>>

So far, the "Visual Identity Description" contains an introduction, described visual elements, a primary logo description, and a color palette description:

Introduction Overviewing Brand Traits:
{{step_1}}

Described Visual Elements:
{{step_2}}

Primary Logo Description representing Brand Traits:
{{step_3}}

Color Palette Description:
{{step_4}}

Next, provide a detailed description of the typography used. This should include details about the font styles, sizes, and spacing, and also how these elements align with the brand's image: {{typography_details}}.

->>>>

The  "Visual Identity Description" we are creating has an introduction, described visual elements, a primary logo description, a color palette description, and a detailed description of typography:

Introduction Overviewing Brand Traits:
{{step_1}}

Described Visual Elements:
{{step_2}}

Primary Logo Description Representing Brand Traits:
{{step_3}}

Color Palette Description:
{{step_4}}

Typography Description:
{{step_5}}

Now, discuss the imagery used in relation to the brand. Describe how it exemplifies the brand's visual standards and what it stands for: {{imagery_standard}}.


```

