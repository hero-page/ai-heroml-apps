# Car Sales Description Generator AI

Utilize the potential of AI with Car Sales Description Generator AI for a tailored car sales pitch. Enable the app to generate captivating content, diving into specific details like car model, year, exterior and interior traits, performance, safety, and tech advancements. Offering more than just the basic specifications, it also persuades potential buyers with an impactful call-to-action. The description it crafts is comprehensive, engaging, and adept in making your car sale offer irresistible.

To run this app online: [Car Sales Description Generator AI Online](https://hero.page/app/car-sales-description-generator-ai-ai-powered-comprehensive-car-salesmanship/15nZG7O6jWKzG5fvkwNC)

To learn more about AI Apps for Car Salesperson use-cases in the Automotive Sales & Services industry, read [How to Enhance Car Sales with AI-Driven Descriptions, Emails, and Summaries](https://hero.page/blog/ai/automotive-sales-and-services/how-to-enhance-car-sales-with-ai-driven-descriptions-emails-and-summaries/170748)

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
npx hero run ./car_sales_description_generator_ai.heroml
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
hero run ./car_sales_description_generator_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./car_sales_description_generator_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./car_sales_description_generator_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./car_sales_description_generator_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Car Sales Description Generator AI
```
Let's write a "Vehicle Description" for the "Automotive Sales & Services" industry for a "Car Salesperson". 

First, create a compelling and engaging headline for the vehicle description. Include the vehicle's model {{vehicle_model}}, its year of manufacture {{year_of_manufacture}}, and one key feature that could attract potential buyers.

Here's some more context about the Vehicle Description:
Vehicle Model: {{vehicle_model}}
Year Of Manufacture: {{year_of_manufacture}}
Exterior Color: {{exterior_color}}
Interior Color: {{interior_color}}
Engine Type: {{engine_type}}

->>>>

We have a captivating headline for our vehicle:

Vehicle Headline:
{{step_1}}

Now, let's write an introduction for the description that provides a quick overview of the car. Mention the vehicle model, its year of manufacture, and its key selling point(s) to appeal to potential buyers.

->>>>

Now, we have a compelling headline and introduction for our vehicle:

Vehicle Headline:
{{step_1}}

Vehicle Introduction:
{{step_2}}

Moving on, let's describe the vehicle's exterior in detail. Discuss or include the exterior color, condition, and any valuable exterior features.

->>>>

At this point, we have a headline, an introduction, and an exterior description for our car:

Vehicle Headline:
{{step_1}}

Vehicle Introduction:
{{step_2}}

Exterior Description:
{{step_3}}

Let's go further and describe the interior of the vehicle. Discuss the interior by mentioning the color, condition, and any noteworthy features.

->>>>

Now, we have detailed descriptions for both the exterior and the interior of the vehicle:

Exterior Description:
{{step_3}}

Interior Description:
{{step_4}}

Next up, detail the performance and specifications of the vehicle. Talk about the engine type, transmission, fuel economy, and any notable performance features.

->>>>

We have descriptions for both the interior of the car and its performance:

Interior Description:
{{step_4}}

Performance and Specifications:
{{step_5}}

Now, let's highlight key technology and safety features that increase the vehicle's appeal.


```

