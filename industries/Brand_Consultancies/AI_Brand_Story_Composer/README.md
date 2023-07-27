# AI Brand Story Composer

Explore the magic of AI with the app AI Brand Story Composer, your tool for personalized brand story creation. Offering you control over variables, it crafts customized and high-quality content. The app paints a comprehensive picture of your brand's unique value and origin, imbibes your mission, vision, and values, and presents an engaging case study. The focus lies not just on attracting potential clients but retaining their interest too through a creative and relatable brand narrative. Dive into the future of brand storytelling with our unique approach and create a compelling brand character.

To run this app online: [AI Brand Story Composer Online](https://hero.page/app/ai-brand-story-composer-personalized-brand-story-creation/U1j54m5YZpRDpJu7eJQB)

[![Run AI Brand Story Composer Online](/assets/run.svg)](https://hero.page/app/ai-brand-story-composer-personalized-brand-story-creation/U1j54m5YZpRDpJu7eJQB)

To learn more about AI Apps for Copywriter use-cases in the Brand Consultancies industry, read [How to Harness AI for Dynamic Brand Storytelling, Engaging Taglines, and Persuasive Product Descriptions](https://hero.page/blog/ai/brand-consultancies/how-to-harness-ai-for-dynamic-brand-storytelling-engaging-taglines-and-persuasive-product-descriptions/170764)

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
npx hero run ./ai_brand_story_composer.heroml
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
hero run ./ai_brand_story_composer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./ai_brand_story_composer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./ai_brand_story_composer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./ai_brand_story_composer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for AI Brand Story Composer
```
Your task is to write a "Brand Story" for the "Brand Consultancies" industry, specifically for a "Copywriter". Let's start by writing a solid introduction that clearly defines what your brand is and what it stands for in the industry. Use the dynamic variable {{brand_value}} to emphasize the unique value of your copywriting brand.

Here's some more context about the Brand Story:
Brand Value: {{brand_value}}
Brand Origin: {{brand_origin}}
Brand Mission And Values: {{brand_mission_and_values}}
Success Case Studies: {{success_case_studies}}
Brand Future: {{brand_future}}

->>>>

Our brand's story begins with this introduction:

Introduction:
{{step_1}}

Next, let's delve into the origins of your brand. Share why the brand was created, what motivated its establishment, and the significant milestones that have shaped the brand's journey. Use the dynamic variable {{brand_origin}} to capture these aspects.

->>>>

The origins and evolution of our brand are as follows:

Origin and Evolution:
{{step_2}}

Moving on, let's explain your brand's core mission, vision, and values. These largely define why you do what you do and how you operate. Use the dynamic variable {{brand_mission_and_values}} to describe these.

->>>>

The core mission, vision and values of our brand have been defined as:

Mission, Vision and Values:
{{step_3}}

Now, let's highlight how you have delivered value to your clients through your copywriting skills. Discuss how you've overcome challenges and achieved success. You can capture this in the dynamic variable {{success_case_studies}}.

->>>>

The success we've had in delivering value to our clients is outlined as:

Success Case Studies:
{{step_4}}

Lastly, we need to conclude the brand story by painting a picture of what the future holds for your brand. This section should highlight what clients can expect from engaging with your brand in the foreseeable future. Use the dynamic variable {{brand_future}} to share your vision for your brand.


```

