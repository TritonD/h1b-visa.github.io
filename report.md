H-1B Visa Project Report
================

**Group Member**

Xingyuan Chen, Xin He, Yunzhi Qian, Stephanie Zhen and Katie Gao

**Background**

The H-1B is the most common visa U.S. employers use to bring skilled
foreign workers to the states. Laws limit the maximum distribution of
new H-1B visas each year and the selection process involves random
computer generation from an eligible application pool, also known as the
“H-1B lottery” by some. The standard duration of stay with H-1B visa is
three years, but can be extended up to six years.

Since 2017, as part of its efforts to “hire American,” the Trump
administration has planned to further restrict access to H-1B visas,
which has caused U.S. Citizenship and Immigration Services to more
strictly regulate and review H-1B applications. This may explain the
decreasing number of approved H-1B visa applications in 2018, even as
the number of filed H-1B petitions has risen.

Since the number of H-1B petitions filed each year is directly shaped by
employer demand for work, which is influenced by the strength of the
economy, the increasing number of yearly H-1B visa applicants may
indicate that the current political environment has not had a large
influence on employer’s interests to sponsor alien workers.

**Motivation**

As immigration policies are changing in the U.S., many international
students are concerned about their eligibility to work in the states. We
as international students and friends of international students are
interested in learning more about H-1B sponsorship opportunities and how
H-1B visa applications will affect or dictate our job-seeking potential
after graduate school.

**Data and Methods**

Data was obtained from the U.S. Department of Labor’s Office of Foreign
Labor Certification via Enigma, an open source website with the largest
publicly available government-related data. The dataset contained
details of the employer requesting temporary labor certification as well
as H-1B applicants’ employment information.

For this project, we specifically focused on the data for 2018, with
some skimming of the data from 2010-2017 due to the large file and
sample sizes for each individual year. We filtered the data to only
include certified H-1B cases and employers located within the US. Of the
52 variables, only 19 variables had information that was most pertinent
to our exploratory analysis so we focused on those and filtered out the
rest. These variables included: case number, visa type, case status,
company name, employer’s location (city, state, country), business code,
occupation code, occupation name, number of applicants employers
expected to hire, employee’s contracted date (start date, end date),
employee’s wages (amount, unit), employee’s worksite (city, state), H-1B
dependency, and full time positions.

**Research Questions**

  - Which states hire the most H-1B workers?

  - For companies that hire H-1B workers, where are they located?

  - What cities in California hire the most H-1B workers?

  - What are the top companies that hire the most H-1B workers?

  - What industries hire the most H-1B workers and what is the average
    wage?

**Exploratory Analysis & Findings**

1.  2018 US H-1B Applications by State

We screened out the H-1B applicants whose worksites and/or employer
headquarters were located outside of the U.S. In addition, we combined
the states where the numbers of applicants were under 2,000 together as
“Others.” To better show the distribution of H-1B visas by state, we
created a bar chart and gradient maps of the U.S.

We ranked the number of H-1B applicants by worksite state in ascending
order as well as number of company headquarters within the state. We
noticed that the worksite locations for many H-1B applicants differed
from the actual company headquarter locations, so we were careful to
differentiate between the two variables for clarity.

In 2018, the top 5 states that had the most H-1B applications in
descending order were California, Texas, New York, New Jersey, and
Illinois. It is interesting to note, however, that there were more
companies with headquarters in New Jersey wanting to sponsor H-1B
applicants compared to in New York and Texas. Comparing the top three
states, California had a total of 128,447 applicants, Texas had a total
of 64,506, and New York had a total of 58,296. Apart from the top five,
other states that had more than 10,000 H-1B applicants included
Washington, Arizona, Minnesota, Michigan, Ohio, Massachusetts,
Pennsylvania, Virginia, North Carolina, Georgia, and Florida. The
remaining states had less than 10,000 H-1B applicants. From the map, we
can see that a majority of the states with more than 10,000 H-1B cases
were located on the East coast.

When looking at mean annual wages, California, Washington, and Maine
were the top 3 worksite states with the highest mean annual wages.
Amongst the three states, California’s mean annual wage was $102,054,
Washington’s mean annual wage was $99,153, and Maine’s mean annual wage
was $90,434 in 2018. Tennessee and Louisiana were the only states that
had mean annual wages less than $70,000. The other states had mean
annual wages between $70,000-90,000.

2.  2018 US H-1B Applications by City

The Shiny tab is an interactive platform that shows the number of H-1B
applicants from the top ten cities in each US state. Users are able to
choose the state and wage range for H-1B applicants as they like. The
wage range varies between a minimum of $15,080 and a maximum of
$624,000. Using California as an example, the top ten cities for H-1B
applicants with a wage range between $20,000 and $200,000 include San
Francisco, San Jose, Sunnyvale, Mountainview, Santa Clara, Los Angeles,
Palo Alto, San Diego, Irvine, and Fremont.

3.  2018 US H-1B Applications by Industry and Occupation

To determine the types of occupations that have the most H-1B
applicants, the wage distribution across occupation groups, and the top
companies that hire the most H-1B applicants, we created a boxplot,
barchart, and treemap, respectively, to better view the data.

The Standard Occupation Classification system (SOC code) was used to
reveal specific and detailed information on the occupation of the
applicant. However, one drawback was that the code was too specific to
be efficiently categorized. To better handle the data, we decided to
look at just the first two numbers of the SOC code that indicated the
applicant’s major occupation group (BLS website). Since only 10 of the
22 groups categorized contained a significant amount of people, the
remaining 12 groups were collapsed together into a “Others” group.
Applicants without a SOC code were dropped from the analysis. A bar
chart was used to show the resulting number of applicants for each
occupational field. There was a total of approximately 570,000 certified
H-1B applicants, and the math and technology occupational fields had the
largest number of H-1B applicants (397,562) followed by business and
finance (46,055).

To analyze the wage distribution amongst all occupations, wages were
standardized to yearly annual wages. We decided to use a boxplot to
represent the median, 25th and 75th percentile of annual wages by
occupation since it revealed more information than simply displaying
average wage. We wanted to show more than just average wage so that we
could take into account any kind of potential skew that could occur due
to the influence of outliers (e.g. positions of seniority and other high
wage jobs) for occupational groups, especially those comprised of fewer
individuals. Boxplots can portray a wider range of wages and the median
is more resistant to the influence of outliers. The top 3 occupational
fields with the highest median wage were management ($118,144), sales
($102,232), and healthcare ($84,760). A tree map was used to show the
Top 15 companies that hired the most H-1B applicants. This was done for
the sake of simplicity and also to look at the types of companies that
hired the most applicants compared to the occupational fields that
contained the most applicants. The companies that hired the most
certified H-1B applicants were, in descending order, Deloitte Consulting
(15,596 applicants), Tata Consultancy Services (14,489 applicants),
Infosys (11,547 applicants), and Cognizant Technology Solutions Corp
(10,189 applicants). The remaining companies hired less than 10,000
applicants.

**Discussion**

In a nutshell, our analysis of H-1B data revealed two important things:
1) popular locations that employ the most H-1B applicants, and 2) the
kinds of companies that are willing to sponsor H-1B applicants. The top
states that employ the most H-1B applicants, such as California, Texas,
and New York, are attractive to foreign workers for a variety of
reasons. These reasons could include having a larger initial population
size, being good places to settle down or further one’s professional
career, increased networking opportunities, and better access to
higher-paying jobs.

It is interesting to note that these findings also correlate with the
popularity of states for immigration. According to Pew Research,
California, New York, and New Jersey were the states with the highest
ratio of foreign-born immigrants in 2017. Our data also revealed that
the tech industry most heavily employs H-1B applicants, which just
further goes to show how rapidly the tech field is growing.

We also found that average annual wage and number of H-1B applications
by state were not necessarily correlated. In contrast to California,
which had both a large number of H-1B applicants and a high average
annual wage, Washington and Maine were states that had high average
annual wages but a lower amount of applicants.

As for initial expectations, we originally thought that the
computer/math and healthcare fields would sponsor the most H-1B
applicants due to the rapid growth of these fields in the US, according
to the Bureau of Labor Statistics. We expected the median annual wage
for the computer/math fields to be around $85,000 and for the healthcare
field to be around $100,000. We also expected the top companies to be
from technology, consulting, and hospitals.

What we found was actually quite unexpected; the data results not only
met our expectations, but also exceeded them. The math and technology
fields did contain the most applicants, but it was more than we had
expected. In fact, more than two-thirds of applicants came from those
fields. Conversely, there were far fewer healthcare practitioners
applying for H-1B visas than we had initially expected; only 20,000 out
of 570,000 applicants.

Management occupations had the highest median salary of $118,000,
followed by Sales at $102,000. Originally, we did not expect management
and sales to have such high median salaries. In fact, both management
and sales had higher median salaries than healthcare and computer/math,
which had median salaries of $84,000. Although we had expected
healthcare practitioners to have a higher median salary, the
distribution of wages did skew to the higher side, so our initial
expectation of higher wages in this field is not unreasonable.
Furthermore, the top 15 companies hiring H-1B applicants consisted
mainly of consulting and technology companies, which was what we had
expected.

**Citations**

\[1\] Thrush, Glenn, et al. “Trump Signs Order That Could Lead to Curbs
on Foreign Workers.” The New York Times, The New York Times, 18
Apr. 2017,
<https://www.nytimes.com/2017/04/18/us/politics/executive-order-hire-buy-american-h1b-visa-trump.html>.
\[2\] Pierce, Sarah, and Julia Gelatt. “Evolution of the H-1B: Latest
Trends in a Program on the Brink of Reform.” Migrationpolicy.org, 2
Apr. 2018,
<https://www.migrationpolicy.org/research/evolution-h-1b-latest-trends-program-brink-reform>.
\[3\] Report on H-1B Petitions: Fiscal Year 2018 Annual Report. Homeland
Security: US Citizenship and Immigration Services, 2019, Report on H-1B
Petitions: Fiscal Year 2018 Annual Report,
<https://www.uscis.gov/sites/default/files/reports-studies/FY-2018-Annual-Report-H-1B-Petitions.pdf>.
\[4\] Report on H-1B Petitions: Fiscal Year 2014 Annual Report. Homeland
Security: US Citizenship and Immigration Services, 2014, Report on H-1B
Petitions: Fiscal Year 2014 Annual Report,
<https://www.uscis.gov/sites/default/files/USCIS/Resources/Resources%20for%20Congress/FY_2014_H-1B_Petitions_Report_SIGNED.pdf>
\[5\] Krogstad, Jens Manuel, and Michael Keegan. “15 States with the
Highest Share of Immigrants in Their Population.” Pew Research Center,
Pew Research Center, 14 May 2014,
<https://www.pewresearch.org/fact-tank/2014/05/14/15-states-with-the-highest-share-of-immigrants-in-their-population/>.
\[6\] Schwartz, Samantha Ann. “5 States Dominating Tech Employment.” CIO
Dive, 26 Mar. 2019,
<https://www.ciodive.com/news/5-states-dominating-tech-employment/551315/>.
\[7\] “Fastest Growing Occupations : Occupational Outlook Handbook.”
U.S. Bureau of Labor Statistics, U.S. Bureau of Labor Statistics, 4
Sept. 2019, <https://www.bls.gov/ooh/fastest-growing.htm>. \[8\] “2018
Standard Occupational Classification System.” U.S. Bureau of Labor
Statistics, U.S. Bureau of Labor Statistics,
<https://www.bls.gov/soc/2018/major_groups.htm>.