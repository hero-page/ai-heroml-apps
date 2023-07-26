# Vehicle Review Blog Post Creator

Vehicle Review Blog Post Creator, driven by AI, delivers comprehensive vehicle analysis in blog-style posts. Users control variables to customize content, ensuring robust details are included, such as features, performance, fuel efficiency, pricing, and value for money. Besides providing precise, valuable data for readers, the app distinguishes itself by creating engaging narratives to stimulate discussions among readers, boosting engagement, and fostering an active online community.

To run this app online: [Vehicle Review Blog Post Creator Online](https://hero.page/app/vehicle-review-blog-post-creator-ai-powered-comprehensive-vehicle-analysis/Zi6cfOc2dOh5C4bcyXFo)

To learn more about AI Apps for Content Creator use-cases in the Automotive Product Marketing industry, read [How to Craft AI-Driven Automotive Content for Stellar Reviews and Social Media Impact](https://hero.page/blog/ai/automotive-product-marketing/how-to-craft-ai-driven-automotive-content-for-stellar-reviews-and-social-media-impact/170746)

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
npx hero run ./vehicle_review_blog_post_creator.heroml
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
hero run ./vehicle_review_blog_post_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./vehicle_review_blog_post_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./vehicle_review_blog_post_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./vehicle_review_blog_post_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Vehicle Review Blog Post Creator
```
Your task is to write a "Vehicle Review Blog Post" for the "Automotive Product Marketing" industry, specifically for a "Content Creator". 

First, let's craft an engaging introduction for the review, provide a brief overview of the vehicle, capturing the core essence of it and the purpose of the review.

Here's some more context about the Vehicle Review Blog Post:
Vehicle Brand: {{vehicle_brand}}
Vehicle Type: {{vehicle_type}}
Body Color: {{body_color}}
Engine Spec: {{engine_spec}}
Type Of Terrain: {{type_of_terrain}}
Mpg: {{mpg}}
Real World Mpg: {{real_world_mpg}}
Price: {{price}}
Similar Vehicle: {{similar_vehicle}}
Price Difference Reasoning: {{price_difference_reasoning}}

->>>>

Now we have an engaging introduction:

Introduction:
{{step_1}}

Next, provide a detailed description of the vehicle. This should encompass all key features like the body structure, engine specifications, interiors, safety features, technology, comfort, and more.

->>>>

We have both a captivating introduction and a detailed description of the vehicle: 

Introduction:
{{step_1}}

Vehicle Description:
{{step_2}}

Now, give a thorough evaluation of the vehicle's performance. Include driving experience on different terrains, task performance for SUVs and trucks, or speed and acceleration data for sports cars.

->>>>

So far, we have an introduction, vehicle description, and a thorough performance evaluation:

Introduction:
{{step_1}}

Vehicle Description:
{{step_2}}

Performance Evaluation:
{{step_3}}

Next, discuss the vehicle's fuel efficiency. Provide the manufacturer's declared mpg figures and real-life testing results (using the most relevant metrics in your market, such as miles per gallon (mpg), liters per 100km, etc.).

->>>>

We have an introduction, a detailed description, performance evaluation, and fuel efficiency details:

Introduction:
{{step_1}}

Vehicle Description:
{{step_2}}

Performance Evaluation:
{{step_3}}

Fuel Efficiency:
{{step_4}}

Moving on, discuss the vehicle's pricing and value for money aspect. Compare its price with other vehicles in its class and discuss the reasoning behind the price differences.

->>>>

We now have an introduction, detailed description of the vehicle, performance evaluation, fuel efficiency details, and a pricing discussion:

Introduction:
{{step_1}}

Vehicle Description:
{{step_2}}

Performance Evaluation:
{{step_3}}

Fuel Efficiency:
{{step_4}}

Price and Value Discussion:
{{step_5}}

Next, create a conclusive summary. Balance the strong and weak points of the vehicle, provide an overall impression, and mention whether you would recommend it and to whom it might be particularly advantageous.

->>>>

So far, we have an introduction, detailed description, performance evaluation, fuel efficiency details, a pricing discussion, and a conclusive summary:

Introduction:
{{step_1}}

Vehicle Description:
{{step_2}}

Performance Evaluation:
{{step_3}}

Fuel Efficiency:
{{step_4}}

Price and Value Discussion:
{{step_5}}

Conclusive Summary:
{{step_6}}

Lastly, write a captivating conclusion where you remind the reader why this review is important and invite them to comment or share their thoughts on the vehicle. 


```

