# Child Craft Ad Copy Customizer

Unleash the power of AI with the Child Craft Ad Copy Customizer, your tool for creating tailored, high-quality craft ad copies for kids. Key variables let you craft engaging, industry-specific content, from introductions to calls to action. Our AI focuses on essential selling points such as safety, quality, developmental potential and price, while also incorporating popular, kid-friendly themes. Watch as it magically turns your input into enticing, highly relevant ad copies. The ultimate solution for crafting ads for the children's hobby industry.

To run this app online: [Child Craft Ad Copy Customizer Online](https://hero.page/app/child-craft-ad-copy-customizer-tailored-ad-copy-for-kids'-crafts/aPlcon15Q8mUgemNcPls)

[![Run Child Craft Ad Copy Customizer Online](/assets/run.svg)](https://hero.page/app/child-craft-ad-copy-customizer-tailored-ad-copy-for-kids'-crafts/aPlcon15Q8mUgemNcPls)

To learn more about AI Apps for Product Marketer use-cases in the Children's Crafts & Hobbies industry, read [How to Amplify Children's Crafts Marketing with AI Solutions](https://hero.page/blog/ai/children's-crafts-and-hobbies/how-to-amplify-children's-crafts-marketing-with-ai-solutions/170782)

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
npx hero run ./child_craft_ad_copy_customizer.heroml
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
hero run ./child_craft_ad_copy_customizer.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./child_craft_ad_copy_customizer.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./child_craft_ad_copy_customizer.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./child_craft_ad_copy_customizer.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Child Craft Ad Copy Customizer
```
Let's create an 'Ad Copy' for the 'Children's Crafts & Hobbies' industry for a 'Product Marketer'. Start by crafting an engaging and resonating introduction that informs the reader what the ad copy is about and introduces the children's craft or hobby product: {{product_name}}.

Here's some more context about the Ad Copy:
Product Name: {{product_name}}
Product Description: {{product_description}}
Product USP: {{product_USP}}
Product Benefits: {{product_benefits}}
Call To Action: {{call_to_action}}

->>>>

For our 'Ad Copy', the introduction has been crafted:

Introduction:
{{step_1}}

Let's move forward by providing an enticing and informative description of the product: {{product_description}} while considering children's safety & suitability, skill development, the fun factor, and the product's quality & durability.

->>>>

In our ad copy for a product in the 'Children's Crafts & Hobbies' industry, we have:

Introduction:
{{step_1}}

Product Description:
{{step_2}}

Proceed with outlining the product's unique selling proposition, also known as its USP, to distinguish it from the competition: {{product_USP}}.

->>>>

In the 'Ad Copy' for our Children's Crafts & Hobbies product, we have:

Introduction:
{{step_1}}

Product Description:
{{step_2}}

USP:
{{step_3}}

Following this, list the main benefits of the product, emphasizing how it will positively impact children's craft or hobby routines: {{product_benefits}}.


```

