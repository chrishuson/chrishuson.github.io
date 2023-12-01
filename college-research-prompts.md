# College Research Prompts

**help me research colleges near new york city by querying public data sources and using pandas to analyze them. I am interested in demographic breakdown of the student bodies as well as SAT scores of students admitted. Let's go step by step. Outline the steps and how they would be written in Jupyter notebook cells. Discuss the data sources. Then help me write the code.**

Sure, let's break this down into steps:

Identify Data Sources: We need to find public data sources that provide information about colleges, their demographics, and SAT scores. The National Center for Education Statistics (NCES) is a good starting point. They provide a College Navigator tool that allows you to search for colleges and download data. Another source could be the Integrated Postsecondary Education Data System (IPEDS), which provides detailed data files that you can download and analyze.

Download and Import Data: Once we've identified the data sources, we need to download the data files (usually in CSV or Excel format) and import them into our Jupyter notebook using pandas.

Data Cleaning: The raw data files might contain a lot of information that we don't need, or they might be in a format that's not easy to analyze. We'll need to clean the data by removing unnecessary columns, handling missing values, and converting data types if necessary.

Data Analysis: After cleaning the data, we can use pandas to analyze it. We might want to calculate statistics like the mean and median SAT scores, or the percentage of students in different demographic groups.

Data Visualization: Finally, we can use libraries like matplotlib and seaborn to create visualizations of our data, which can make it easier to understand and interpret.

Here's a rough outline of how this might look in a Jupyter notebook:

    # Cell 1: Import necessary libraries
    import pandas as pd
    import matplotlib.pyplot as plt
    import seaborn as sns

    # Cell 2: Load the data
    df = pd.read_csv('path_to_your_file.csv')

    # Cell 3: Inspect the data
    df.head()

    # Cell 4: Clean the data (this will depend on what the data looks like)
    # df = df.drop(columns=['unnecessary_column1', 'unnecessary_column2'])
    # df['column'] = df['column'].astype('new_type')

    # Cell 5: Analyze the data
    # mean_sat = df['sat_scores'].mean()
    # median_sat = df['sat_scores'].median()

    # Cell 6: Visualize the data
    # plt.hist(df['sat_scores'])
    # plt.show()

Please note that the above is a very general outline and the actual code will depend on what the data looks like. Once you've downloaded the data, I can help you write more specific code to clean and analyze it.

**Ok. Let's follow that plan. Let's start with the two data sources you recommend. Let's start with just two colleges: SUNY New Paltz and Hunter College (CUNY). If you can, write the queries as code**

Unfortunately, as an AI, I don't have the ability to directly access or query external databases or APIs. However, I can guide you on how to do it.

The National Center for Education Statistics (NCES) and the Integrated Postsecondary Education Data System (IPEDS) provide data files that you can download manually, but they don't provide a public API that you can query directly from your code.

Here's how you can get the data:

Visit the NCES College Navigator website (https://nces.ed.gov/collegenavigator/).
Enter "SUNY New Paltz" and "Hunter College" in the search box and click on the search button.
Click on the name of the college in the search results to view its details.
Click on the "Download PDF" button to download a PDF with detailed information about the college.
For IPEDS:

Visit the IPEDS Data Center website (https://nces.ed.gov/ipeds/datacenter/Default.aspx).
Click on "Download Data Files".
Select the data files you're interested in and download them.
Once you've downloaded the data, you can import it into your Jupyter notebook using pandas. For example, if you've downloaded a CSV file, you can import it like this:

    df = pd.read_csv('path_to_your_file.csv')

If the data is in a PDF file, you'll need to use a library like tabula-py or PyPDF2 to extract the data from the PDF. Here's an example using tabula-py:

import tabula

    # Read pdf into list of DataFrame
    dfs = tabula.read_pdf("path_to_your_file.pdf", pages='all')

    # Now you can treat dfs as a normal DataFrame

Remember to replace 'path_to_your_file.csv' and 'path_to_your_file.pdf' with the actual paths to your files.
