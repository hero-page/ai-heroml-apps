# Brand Strategist Guidelines Maker

Maximize your brand's potential with the Brand Strategist Guidelines Maker app, powered by AI. Define your variables to get an in-depth, tailored branding strategy that includes integral details about your brand, such as name, logo, color, typography, and ethos. Receive detailed strategic branding data, usage rules, and concrete guidelines about your brand's representation across different platforms. Experience the advantage of having meticulous content that dives deep into your brand's voice and target audience, providing a clear positioning strategy while ensuring brand consistency and adaptability in various contexts.

To run this app online: [Brand Strategist Guidelines Maker Online](https://hero.page/app/brand-strategist-guidelines-maker-ai-powered-customized-branding-strategy/HDxm1XbtYWiSaxhQeZNg)

[![Run Brand Strategist Guidelines Maker Online](/assets/run.svg)](https://hero.page/app/brand-strategist-guidelines-maker-ai-powered-customized-branding-strategy/HDxm1XbtYWiSaxhQeZNg)

To learn more about AI Apps for Brand Strategist use-cases in the Brand Consultancies industry, read [How to Innovate Brand Strategy with AI Workflow Apps](https://hero.page/blog/ai/brand-consultancies/how-to-innovate-brand-strategy-with-ai-workflow-apps/170763)

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
npx hero run ./brand_strategist_guidelines_maker.heroml
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
hero run ./brand_strategist_guidelines_maker.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./brand_strategist_guidelines_maker.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./brand_strategist_guidelines_maker.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./brand_strategist_guidelines_maker.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Brand Strategist Guidelines Maker
```
Your task is to write a "Brand Guidelines" for the "Brand Consultancies" industry, specifically for a "Brand Strategist". 
Begin by drafting an introduction that defines the scope, rationale, and importance of having clear "Brand Guidelines".

Here's some more context about the Brand Guidelines:
Reason For Brand Guidelines: {{reason_for_brand_guidelines}}
Brand Identity: {{brand_identity}}
Brand Ethos: {{brand_ethos}}
Brand Voice: {{brand_voice}}
Target Audience: {{target_audience}}
Brand Positioning: {{brand_positioning}}
Brand Usage: {{brand_usage}}
Brand Representation: {{brand_representation}}

->>>>

The first part of our "Brand Guidelines" document is now ready:

Introduction:
{{step_1}}

Next, elaborate on the brand identity, including features like the brand name, logo, typography, and color scheme that form the visual appearance of the brand.

->>>>

So far, we have developed the following sections for our "Brand Guidelines" document:

Introduction:
{{step_1}}

Brand Identity:
{{step_2}}

Now go on to describe the brand ethos, which encapsulates the brand’s values, mission, vision and persona.

->>>>

We have now included the brand ethos in our "Brand Guidelines" document:

Introduction:
{{step_1}}

Brand Identity:
{{step_2}}

Brand Ethos:
{{step_3}}

Next, draft a section dedicated to the brand voice, detailing the style, tone, and language to be used when communicating as the brand.

->>>>

Our "Brand Guidelines" document is shaping up well:

Brand Identity:
{{step_2}}

Brand Ethos:
{{step_3}}

Brand Voice:
{{step_4}}

Now, discuss the target audience. Clearly define the demographic, psychographic, and behavioral traits of the consumers the brand aims to attract and retain.

->>>>

So far, the "Brand Guidelines" document includes:

Brand Ethos:
{{step_3}}

Brand Voice:
{{step_4}}

Target Audience:
{{step_5}}

Next, outline the brand positioning strategy that differentiates this brand in the market against competing brands.

->>>>

Our "Brand Guidelines" document now includes a robust brand positioning strategy:

Brand Voice:
{{step_4}}

Target Audience:
{{step_5}}

Brand Positioning:
{{step_6}}

Please provide a set of dos and don'ts that instruct both the internal team and external parties on how to use the brand elements.

->>>>

With the addition of the dos and don'ts for brand usage, our "Brand Guidelines" document now includes:

Target Audience:
{{step_5}}

Brand Positioning:
{{step_6}}

Brand Usage:
{{step_7}}

Finally, write a brief on how the brand should be represented in various channels and circumstances. 


```

