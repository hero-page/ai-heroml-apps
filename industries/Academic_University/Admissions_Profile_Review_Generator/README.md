# Admissions Profile Review Generator

Use the Admissions Profile Review Generator to streamline your candidate review process with AI. Customize variables to generate detailed profiles. The app provides an in-depth assessment of an applicant's credentials, extracurriculars, recommendations, and suitability for the program applied to. The standout feature is the personalized report on the applicant's fit for the program, considering their unique abilities, experiences and potential contributions. This assists Admissions Officers in making informed decisions and improving the efficiency of the admissions process.

To run this app online: [Admissions Profile Review Generator Online](https://hero.page/app/admissions-profile-review-generator-automated-comprehensive-admissions-assessment/PDPtNibgDs7ViA1U9Hyw)

To learn more about AI Apps for Admissions Officer use-cases in the Academic & University industry, read [How to Streamline University Admissions with 3 AI Tools](https://hero.page/blog/academic-and-university/admissions-officer/how-to-streamline-university-admissions-with-3-ai-tools/170703)

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
npx hero run ./admissions_profile_review_generator.heroml
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
hero run ./admissions_profile_review_generator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./admissions_profile_review_generator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./admissions_profile_review_generator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./admissions_profile_review_generator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Admissions Profile Review Generator
```
Your task is to write an "Application Review" for the "Academic & University" industry, specifically for an "Admissions Officer". 

Let's start by creating an introductory summary that provides a brief overview of the applicant: {{applicant_overview}}. This section should also include relevant demographic details, the program applied for, and the date of the application.

Here's some more context about the Application Review:
Applicant Overview: {{applicant_overview}}
Academic Performance: {{academic_performance}}
Extracurricular Achievements: {{extracurricular_achievements}}
Recommendations: {{recommendations}}
Assessment Summary: {{assessment_summary}}

->>>>

We have an overview for the "Application Review":

Applicant Overview:
{{step_1}}

Next, let's proceed to a detailed examination of the applicant's academic qualifications. This section should discuss the applicant's performance in previous academic institutions. Include any special academic achievements or honours received by the applicant.

->>>>

In our "Application Review", we now have the applicant's academic qualifications:

Applicant Overview:
{{step_1}}

Academic Qualifications:
{{step_2}}

Continuing on, discuss the applicant's extracurricular activities and achievements: {{extracurricular_achievements}}. Indicate how these activities have contributed to the applicant's personal development, and how they align with the university’s culture and values.

->>>>

We've collected some information about the applicant's extracurricular activities for our "Application Review":

Applicant Overview:
{{step_1}}

Academic Qualifications:
{{step_2}}

Extracurricular Achievements:
{{step_3}}

Next, include the applicant's recommendation letters or references in the review. Analyze these third-party opinions on the applicant's ability and potential.

->>>>

In the "Application Review", we've included all necessary evaluations:

Applicant Overview:
{{step_1}}

Academic Qualifications:
{{step_2}}

Extracurricular Achievements:
{{step_3}}

Recommendations:
{{step_4}}

Finally, we need to assess the applicant's suitability for the program they have applied for. This should include your professional opinion of the applicant, their strengths and weaknesses, how they might contribute to the university and program, and any areas of concern.


```

