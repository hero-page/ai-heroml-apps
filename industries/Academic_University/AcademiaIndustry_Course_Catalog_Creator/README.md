# Academia-Industry Course Catalog Creator

Academia-Industry Course Catalog Creator is a user-friendly application that harnesses AI to produce bespoke, high-quality content for academic universities. Users can specify variables in prompts to create a detailed course catalog, including an introduction, course listings, department outlines, and more. Notably, this app incorporates industry elements in course descriptions, linking academia and industry relevance. This unique feature elevates the catalog from merely academic to a career-oriented guidance tool.

To run this app online: [Academia-Industry Course Catalog Creator Online](https://hero.page/app/academia-industry-course-catalog-creator-linking-academia-industry-via-courses/Xomz4kPxELmhm6iRZiYF)

[![Run Academia-Industry Course Catalog Creator Online](/assets/run.svg)](https://hero.page/app/academia-industry-course-catalog-creator-linking-academia-industry-via-courses/Xomz4kPxELmhm6iRZiYF)

To learn more about AI Apps for Administrator use-cases in the Academic & University industry, read [How to Streamline Academic Administration with AI Tools](https://hero.page/blog/ai/academic-and-university/how-to-streamline-academic-administration-with-ai-tools/170702)

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
npx hero run ./academia_industry_course_catalog_creator.heroml
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
hero run ./academia_industry_course_catalog_creator.heroml
```

You can provide initial variable values as command-line options. For example, if your script expects a variable named `number_of_colors`, you can provide its value as follows:

```bash
hero run --number_of_colors 4 ./academia_industry_course_catalog_creator.heroml
```

If you do not provide a value for a variable, the HeroML CLI tool will prompt you to enter it interactively.

### Output Options

You can specify the output directory and the filename of the output file using command-line options:

- The `-o` or `--output-dir` option allows you to specify the output directory. By default, it is `./outputs/`.

```bash
hero run --output-dir /custom/output/directory ./academia_industry_course_catalog_creator.heroml
```

- The `-f` or `--filename` option allows you to specify the filename of the output file. By default, it is `response_TIMESTAMP.json`.

```bash
hero run --filename custom_filename.json ./academia_industry_course_catalog_creator.heroml
```

The CLI tool writes the output to a JSON file in the specified directory. It will print the path of the output file to the console:

```bash
Success! Output written to /custom/output/directory/custom_filename.json
```


## HeroML AI Steps for Academia-Industry Course Catalog Creator
```
Your task is to write a course catalog for the Academic & University industry, specifically for an Administrator. Let's start by crafting a comprehensive introduction for the course catalog which will include the name of the institution and academic year, as well as a brief overview of the school’s mission and vision.

Here's some more context about the Course Catalog:
Institution Name: {{institution_name}}
Academic Year: {{academic_year}}
Course Title: {{course_title}}
Prerequisites: {{prerequisites}}
Department Name: {{department_name}}
Industry Trends: {{industry_trends}}

->>>>

Here is our course catalog introduction:

Institution Name:
{{institution_name}}

Academic Year:
{{step_1}}

Moving forward, based on introduction, we need to list each course in the course catalog by providing specific details. The details should include course title, a brief description of the course, any applicable course credits, prerequisite courses if there are any, and the learning outcomes of the course.

->>>>

Now, we have the course details:

Course Details:
{{step_2}}

Next, divide these courses into section-based departments for logical arrangement and easy following. Make sure the information is presented in a hierarchical way.

->>>>

We have divided the courses into department sections:

Department Sections:
{{step_3}}

For each of these departments, create an outline that will include an introduction of the department, key faculty, and the listed courses for respective departments. This will enable readers to navigate easily to the relevant department.

->>>>

We have our department outline:

Department Outline:
{{step_4}}

Now, using this outline, let's incorporate the specific elements of the Academic & University industry into the course descriptions. Consulting faculty members to ensure the accuracy of course descriptions and the reflection of current industry trends can be a profitable choice.

->>>>

We have created our industry-oriented course descriptions:

Course Descriptions:
{{step_5}}

Next, let's add onto our catalog all the necessary policies and regulations related to course registration, credit hours, grading systems, and academic schedule. This will provide students and advisors all the mandatory information they might need.

->>>>

We now have a policy and regulation section in our course catalog:

Policy and Regulation Section:
{{step_6}}

Finally, let's conclude the catalog by providing the contact details for each academic department for further queries. This section should include the department name, contact person, email address, and phone number.


```

