# Car Sales Deal Summary AI

Explore the world of automotive sales with Car Sales Deal Summary AI. With the power to specify variables, you can master sales analysis from all angles. Utilize AI technology to generate high-quality summaries outlining every aspect of a deal, from car details to customer needs, negotiations, final terms, and more. With a focus on both the customer and salesperson's experience, the app promises a unique perspective. Both parties' feelings and input are taken into account, not just the car sold or deal terms - delivering an insightful, multi-dimensional analysis.

To run this app online: [Car Sales Deal Summary AI Online](https://hero.page/app/car-sales-deal-summary-ai-comprehensive-multi-dimensional-sales-analysis/8rsxWulRdEJs8mTVLBq5)

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
npx hero run ./car_sales_deal_summary_ai.heroml
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
hero run ./car_sales_deal_summary_ai.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./car_sales_deal_summary_ai.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./car_sales_deal_summary_ai.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./car_sales_deal_summary_ai.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Car Sales Deal Summary AI
```
Your task is to write a "Deal Summary" for the "Automotive Sales & Services" industry, specifically for a "Car Salesperson". 

Let's start by crafting an introduction explaining the specific deal context: {{deal_context}}. This introduction will detail key information such as the make and model of the car, its unique features, what attracted the customer, and its selling points.

Here's some more context about the Deal Summary:
Deal Context: {{deal_context}}
Customer Profile: {{customer_profile}}
Deal Terms: {{deal_terms}}
Deal Experience: {{deal_experience}}
Sales Objectives: {{sales_objectives}}

->>>>

We now have an introduction to our deal:

Introduction:
{{step_1}}

Next, let's elaborate on different aspects of the deal. 
 
We'll start with creating a customer profile: {{customer_profile}}. Please include details on their car needs, budget, preferences, and unique requirements, if any.

->>>>

We now have an introduction and customer profile:

Introduction:
{{step_1}}

Customer Profile:
{{step_2}}

Now, describe the negotiation process. Specifically provide details on how the car's features, price, dealer incentives, and financing options were discussed, aligned, and agreed upon. Ensure you focus on meeting {{customer_profile}}'s needs.

->>>>

We now have a customer profile and information on the negotiation process:

Customer Profile:
{{step_2}}

Negotiation Process:
{{step_3}}

Let's now detail the final terms of the deal: {{deal_terms}}. Include information on the agreed price and any additional services or extras included in the deal. Also provide details on any post-sale obligations like scheduled servicing and warranty coverage.

->>>>

We have detailed information on the negotiation process and the final terms of the deal:

Negotiation Process:
{{step_3}}

Final Deal Terms:
{{step_4}}

Now, let's portray the overall experience of the deal from both the customer and the car salesperson perspective. In this {{deal_experience}}, include customer's satisfaction level, the salesperson's learning, and the benefits to the company, if any.

->>>>

We have detailed information about the final terms of the deal and the complete deal experience:

Final Deal Terms:
{{step_4}}

Deal Experience:
{{step_5}}

Finally, conclude by highlighting the positive aspects of the deal and sharing any valuable learnings that could be applied to future deals. The conclusion should also touch on how the deal allows the car salesperson to fulfil their sales objectives: {{sales_objectives}}.


```

