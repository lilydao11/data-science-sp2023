COVID-19
================
Lily Dao
2022-03-06

- <a href="#grading-rubric" id="toc-grading-rubric">Grading Rubric</a>
  - <a href="#individual" id="toc-individual">Individual</a>
  - <a href="#due-date" id="toc-due-date">Due Date</a>
- <a href="#the-big-picture" id="toc-the-big-picture">The Big Picture</a>
- <a href="#get-the-data" id="toc-get-the-data">Get the Data</a>
  - <a href="#navigating-the-census-bureau"
    id="toc-navigating-the-census-bureau">Navigating the Census Bureau</a>
    - <a
      href="#q1-load-table-b01003-into-the-following-tibble-make-sure-the-column-names-are-id-geographic-area-name-estimatetotal-margin-of-errortotal"
      id="toc-q1-load-table-b01003-into-the-following-tibble-make-sure-the-column-names-are-id-geographic-area-name-estimatetotal-margin-of-errortotal"><strong>q1</strong>
      Load Table <code>B01003</code> into the following tibble. Make sure the
      column names are
      <code>id, Geographic Area Name, Estimate!!Total, Margin of Error!!Total</code>.</a>
  - <a href="#automated-download-of-nyt-data"
    id="toc-automated-download-of-nyt-data">Automated Download of NYT
    Data</a>
    - <a
      href="#q2-visit-the-nyt-github-repo-and-find-the-url-for-the-raw-us-county-level-data-assign-that-url-as-a-string-to-the-variable-below"
      id="toc-q2-visit-the-nyt-github-repo-and-find-the-url-for-the-raw-us-county-level-data-assign-that-url-as-a-string-to-the-variable-below"><strong>q2</strong>
      Visit the NYT GitHub repo and find the URL for the <strong>raw</strong>
      US County-level data. Assign that URL as a string to the variable
      below.</a>
- <a href="#join-the-data" id="toc-join-the-data">Join the Data</a>
  - <a href="#q3-process-the-id-column-of-df_pop-to-create-a-fips-column"
    id="toc-q3-process-the-id-column-of-df_pop-to-create-a-fips-column"><strong>q3</strong>
    Process the <code>id</code> column of <code>df_pop</code> to create a
    <code>fips</code> column.</a>
  - <a
    href="#q4-join-df_covid-with-df_q3-by-the-fips-column-use-the-proper-type-of-join-to-preserve-only-the-rows-in-df_covid"
    id="toc-q4-join-df_covid-with-df_q3-by-the-fips-column-use-the-proper-type-of-join-to-preserve-only-the-rows-in-df_covid"><strong>q4</strong>
    Join <code>df_covid</code> with <code>df_q3</code> by the
    <code>fips</code> column. Use the proper type of join to preserve
    <em>only</em> the rows in <code>df_covid</code>.</a>
- <a href="#analyze" id="toc-analyze">Analyze</a>
  - <a href="#normalize" id="toc-normalize">Normalize</a>
    - <a
      href="#q5-use-the-population-estimates-in-df_data-to-normalize-cases-and-deaths-to-produce-per-100000-counts-3-store-these-values-in-the-columns-cases_per100k-and-deaths_per100k"
      id="toc-q5-use-the-population-estimates-in-df_data-to-normalize-cases-and-deaths-to-produce-per-100000-counts-3-store-these-values-in-the-columns-cases_per100k-and-deaths_per100k"><strong>q5</strong>
      Use the <code>population</code> estimates in <code>df_data</code> to
      normalize <code>cases</code> and <code>deaths</code> to produce per
      100,000 counts [3]. Store these values in the columns
      <code>cases_per100k</code> and <code>deaths_per100k</code>.</a>
  - <a href="#guided-eda" id="toc-guided-eda">Guided EDA</a>
    - <a
      href="#q6-compute-the-mean-and-standard-deviation-for-cases_per100k-and-deaths_per100k"
      id="toc-q6-compute-the-mean-and-standard-deviation-for-cases_per100k-and-deaths_per100k"><strong>q6</strong>
      Compute the mean and standard deviation for <code>cases_per100k</code>
      and <code>deaths_per100k</code>.</a>
    - <a
      href="#q7-find-the-top-10-counties-in-terms-of-cases_per100k-and-the-top-10-in-terms-of-deaths_per100k-report-the-population-of-each-county-along-with-the-per-100000-counts-compare-the-counts-against-the-mean-values-you-found-in-q6-note-any-observations"
      id="toc-q7-find-the-top-10-counties-in-terms-of-cases_per100k-and-the-top-10-in-terms-of-deaths_per100k-report-the-population-of-each-county-along-with-the-per-100000-counts-compare-the-counts-against-the-mean-values-you-found-in-q6-note-any-observations"><strong>q7</strong>
      Find the top 10 counties in terms of <code>cases_per100k</code>, and the
      top 10 in terms of <code>deaths_per100k</code>. Report the population of
      each county along with the per-100,000 counts. Compare the counts
      against the mean values you found in q6. Note any observations.</a>
  - <a href="#self-directed-eda" id="toc-self-directed-eda">Self-directed
    EDA</a>
    - <a
      href="#q8-drive-your-own-ship-youve-just-put-together-a-very-rich-dataset-you-now-get-to-explore-pick-your-own-direction-and-generate-at-least-one-punchline-figure-to-document-an-interesting-finding-i-give-a-couple-tips--ideas-below"
      id="toc-q8-drive-your-own-ship-youve-just-put-together-a-very-rich-dataset-you-now-get-to-explore-pick-your-own-direction-and-generate-at-least-one-punchline-figure-to-document-an-interesting-finding-i-give-a-couple-tips--ideas-below"><strong>q8</strong>
      Drive your own ship: You’ve just put together a very rich dataset; you
      now get to explore! Pick your own direction and generate at least one
      punchline figure to document an interesting finding. I give a couple
      tips &amp; ideas below:</a>
    - <a href="#ideas" id="toc-ideas">Ideas</a>
    - <a href="#aside-some-visualization-tricks"
      id="toc-aside-some-visualization-tricks">Aside: Some visualization
      tricks</a>
    - <a href="#geographic-exceptions"
      id="toc-geographic-exceptions">Geographic exceptions</a>
- <a href="#notes" id="toc-notes">Notes</a>

*Purpose*: In this challenge, you’ll learn how to navigate the U.S.
Census Bureau website, programmatically download data from the internet,
and perform a county-level population-weighted analysis of current
COVID-19 trends. This will give you the base for a very deep
investigation of COVID-19, which we’ll build upon for Project 1.

<!-- include-rubric -->

# Grading Rubric

<!-- -------------------------------------------------- -->

Unlike exercises, **challenges will be graded**. The following rubrics
define how you will be graded, both on an individual and team basis.

## Individual

<!-- ------------------------- -->

| Category    | Needs Improvement                                                                                                | Satisfactory                                                                                                               |
|-------------|------------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------|
| Effort      | Some task **q**’s left unattempted                                                                               | All task **q**’s attempted                                                                                                 |
| Observed    | Did not document observations, or observations incorrect                                                         | Documented correct observations based on analysis                                                                          |
| Supported   | Some observations not clearly supported by analysis                                                              | All observations clearly supported by analysis (table, graph, etc.)                                                        |
| Assessed    | Observations include claims not supported by the data, or reflect a level of certainty not warranted by the data | Observations are appropriately qualified by the quality & relevance of the data and (in)conclusiveness of the support      |
| Specified   | Uses the phrase “more data are necessary” without clarification                                                  | Any statement that “more data are necessary” specifies which *specific* data are needed to answer what *specific* question |
| Code Styled | Violations of the [style guide](https://style.tidyverse.org/) hinder readability                                 | Code sufficiently close to the [style guide](https://style.tidyverse.org/)                                                 |

## Due Date

<!-- ------------------------- -->

All the deliverables stated in the rubrics above are due **at midnight**
before the day of the class discussion of the challenge. See the
[Syllabus](https://docs.google.com/document/d/1qeP6DUS8Djq_A0HMllMqsSqX3a9dbcx1/edit?usp=sharing&ouid=110386251748498665069&rtpof=true&sd=true)
for more information.

``` r
library(tidyverse)
```

    ## ── Attaching packages ─────────────────────────────────────── tidyverse 1.3.2 ──
    ## ✔ ggplot2 3.4.0      ✔ purrr   1.0.1 
    ## ✔ tibble  3.1.8      ✔ dplyr   1.0.10
    ## ✔ tidyr   1.2.1      ✔ stringr 1.5.0 
    ## ✔ readr   2.1.3      ✔ forcats 0.5.2 
    ## ── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
    ## ✖ dplyr::filter() masks stats::filter()
    ## ✖ dplyr::lag()    masks stats::lag()

*Background*:
[COVID-19](https://en.wikipedia.org/wiki/Coronavirus_disease_2019) is
the disease caused by the virus SARS-CoV-2. In 2020 it became a global
pandemic, leading to huge loss of life and tremendous disruption to
society. The New York Times (as of writing) publishes up-to-date data on
the progression of the pandemic across the United States—we will study
these data in this challenge.

*Optional Readings*: I’ve found this [ProPublica
piece](https://www.propublica.org/article/how-to-understand-covid-19-numbers)
on “How to understand COVID-19 numbers” to be very informative!

# The Big Picture

<!-- -------------------------------------------------- -->

We’re about to go through *a lot* of weird steps, so let’s first fix the
big picture firmly in mind:

We want to study COVID-19 in terms of data: both case counts (number of
infections) and deaths. We’re going to do a county-level analysis in
order to get a high-resolution view of the pandemic. Since US counties
can vary widely in terms of their population, we’ll need population
estimates in order to compute infection rates (think back to the
`Titanic` challenge).

That’s the high-level view; now let’s dig into the details.

# Get the Data

<!-- -------------------------------------------------- -->

1.  County-level population estimates (Census Bureau)
2.  County-level COVID-19 counts (New York Times)

## Navigating the Census Bureau

<!-- ------------------------- -->

**Steps**: Our objective is to find the 2018 American Community
Survey\[1\] (ACS) Total Population estimates, disaggregated by counties.
To check your results, this is Table `B01003`.

1.  Go to [data.census.gov](data.census.gov).
2.  Scroll down and click `View Tables`.
3.  Apply filters to find the ACS **Total Population** estimates,
    disaggregated by counties. I used the filters:

- `Topics > Populations and People > Counts, Estimates, and Projections > Population Total`
- `Geography > County > All counties in United States`

5.  Select the **Total Population** table and click the `Download`
    button to download the data; make sure to select the 2018 5-year
    estimates.
6.  Unzip and move the data to your `challenges/data` folder.

- Note that the data will have a crazy-long filename like
  `ACSDT5Y2018.B01003_data_with_overlays_2020-07-26T094857.csv`. That’s
  because metadata is stored in the filename, such as the year of the
  estimate (`Y2018`) and my access date (`2020-07-26`). **Your filename
  will vary based on when you download the data**, so make sure to copy
  the filename that corresponds to what you downloaded!

### **q1** Load Table `B01003` into the following tibble. Make sure the column names are `id, Geographic Area Name, Estimate!!Total, Margin of Error!!Total`.

*Hint*: You will need to use the `skip` keyword when loading these data!

``` r
## TASK: Load the census bureau data with the following tibble name.
df_pop <- read_csv("./data/ACSDT5Y2018.B01003-Data.csv")
```

    ## New names:
    ## Rows: 3221 Columns: 7
    ## ── Column specification
    ## ──────────────────────────────────────────────────────── Delimiter: "," chr
    ## (6): GEO_ID, NAME, B01003_001E, B01003_001EA, B01003_001M, B01003_001MA lgl
    ## (1): ...7
    ## ℹ Use `spec()` to retrieve the full column specification for this data. ℹ
    ## Specify the column types or set `show_col_types = FALSE` to quiet this message.
    ## • `` -> `...7`

``` r
names(df_pop) <- df_pop[1,]
```

    ## Warning: The `value` argument of `names<-` can't be empty as of tibble 3.0.0.
    ## ℹ Column 7 must be named.

    ## Warning: The `value` argument of `names<-` must be a character vector as of tibble
    ## 3.0.0.

``` r
df_pop <- df_pop[-1,]
df_pop
```

    ## # A tibble: 3,220 × 7
    ##    Geography      `Geographic Area Name`   Estim…¹ Annot…² Margi…³ Annot…⁴ `NA` 
    ##    <chr>          <chr>                    <chr>   <chr>   <chr>   <chr>   <lgl>
    ##  1 0500000US01001 Autauga County, Alabama  55200   null    *****   *****   NA   
    ##  2 0500000US01003 Baldwin County, Alabama  208107  null    *****   *****   NA   
    ##  3 0500000US01005 Barbour County, Alabama  25782   null    *****   *****   NA   
    ##  4 0500000US01007 Bibb County, Alabama     22527   null    *****   *****   NA   
    ##  5 0500000US01009 Blount County, Alabama   57645   null    *****   *****   NA   
    ##  6 0500000US01011 Bullock County, Alabama  10352   null    *****   *****   NA   
    ##  7 0500000US01013 Butler County, Alabama   20025   null    *****   *****   NA   
    ##  8 0500000US01015 Calhoun County, Alabama  115098  null    *****   *****   NA   
    ##  9 0500000US01017 Chambers County, Alabama 33826   null    *****   *****   NA   
    ## 10 0500000US01019 Cherokee County, Alabama 25853   null    *****   *****   NA   
    ## # … with 3,210 more rows, and abbreviated variable names ¹​`Estimate!!Total`,
    ## #   ²​`Annotation of Estimate!!Total`, ³​`Margin of Error!!Total`,
    ## #   ⁴​`Annotation of Margin of Error!!Total`

*Note*: You can find information on 1-year, 3-year, and 5-year estimates
[here](https://www.census.gov/programs-surveys/acs/guidance/estimates.html).
The punchline is that 5-year estimates are more reliable but less
current.

## Automated Download of NYT Data

<!-- ------------------------- -->

ACS 5-year estimates don’t change all that often, but the COVID-19 data
are changing rapidly. To that end, it would be nice to be able to
*programmatically* download the most recent data for analysis; that way
we can update our analysis whenever we want simply by re-running our
notebook. This next problem will have you set up such a pipeline.

The New York Times is publishing up-to-date data on COVID-19 on
[GitHub](https://github.com/nytimes/covid-19-data).

### **q2** Visit the NYT [GitHub](https://github.com/nytimes/covid-19-data) repo and find the URL for the **raw** US County-level data. Assign that URL as a string to the variable below.

``` r
## TASK: Find the URL for the NYT covid-19 county-level data
url_counties <- "https://raw.githubusercontent.com/nytimes/covid-19-data/master/us-counties.csv"
```

Once you have the url, the following code will download a local copy of
the data, then load the data into R.

``` r
## NOTE: No need to change this; just execute
## Set the filename of the data to download
filename_nyt <- "./data/nyt_counties.csv"

## Download the data locally
curl::curl_download(
        url_counties,
        destfile = filename_nyt
      )

## Loads the downloaded csv
df_covid <- read_csv(filename_nyt, col_types = "ccccdd")
```

You can now re-run the chunk above (or the entire notebook) to pull the
most recent version of the data. Thus you can periodically re-run this
notebook to check in on the pandemic as it evolves.

*Note*: You should feel free to copy-paste the code above for your own
future projects!

# Join the Data

<!-- -------------------------------------------------- -->

To get a sense of our task, let’s take a glimpse at our two data
sources.

``` r
## NOTE: No need to change this; just execute
df_pop %>% glimpse
```

    ## Rows: 3,220
    ## Columns: 7
    ## $ Geography                              <chr> "0500000US01001", "0500000US010…
    ## $ `Geographic Area Name`                 <chr> "Autauga County, Alabama", "Bal…
    ## $ `Estimate!!Total`                      <chr> "55200", "208107", "25782", "22…
    ## $ `Annotation of Estimate!!Total`        <chr> "null", "null", "null", "null",…
    ## $ `Margin of Error!!Total`               <chr> "*****", "*****", "*****", "***…
    ## $ `Annotation of Margin of Error!!Total` <chr> "*****", "*****", "*****", "***…
    ## $ `NA`                                   <lgl> NA, NA, NA, NA, NA, NA, NA, NA,…

``` r
df_covid %>% glimpse
```

    ## Rows: 2,502,832
    ## Columns: 6
    ## $ date   <chr> "2020-01-21", "2020-01-22", "2020-01-23", "2020-01-24", "2020-0…
    ## $ county <chr> "Snohomish", "Snohomish", "Snohomish", "Cook", "Snohomish", "Or…
    ## $ state  <chr> "Washington", "Washington", "Washington", "Illinois", "Washingt…
    ## $ fips   <chr> "53061", "53061", "53061", "17031", "53061", "06059", "17031", …
    ## $ cases  <dbl> 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, …
    ## $ deaths <dbl> 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, …

To join these datasets, we’ll need to use [FIPS county
codes](https://en.wikipedia.org/wiki/FIPS_county_code).\[2\] The last
`5` digits of the `id` column in `df_pop` is the FIPS county code, while
the NYT data `df_covid` already contains the `fips`.

### **q3** Process the `id` column of `df_pop` to create a `fips` column.

``` r
## TASK: Create a `fips` column by extracting the county code
df_q3 <- 
  df_pop %>%
  mutate(fips = str_extract(Geography, "[[:alpha:]]\\d+")) %>%
  mutate(fips = str_extract(fips, "\\d+"))
```

Use the following test to check your answer.

``` r
## NOTE: No need to change this
## Check known county
assertthat::assert_that(
              (df_q3 %>%
              filter(str_detect(`Geographic Area Name`, "Autauga County")) %>%
              pull(fips)) == "01001"
            )
```

    ## [1] TRUE

``` r
print("Very good!")
```

    ## [1] "Very good!"

### **q4** Join `df_covid` with `df_q3` by the `fips` column. Use the proper type of join to preserve *only* the rows in `df_covid`.

``` r
## TASK: Join df_covid and df_q3 by fips.
df_q4 <- 
  df_covid %>%
  left_join(., df_q3, by = "fips")
df_q4
```

    ## # A tibble: 2,502,832 × 13
    ##    date  county state fips  cases deaths Geogr…¹ Geogr…² Estim…³ Annot…⁴ Margi…⁵
    ##    <chr> <chr>  <chr> <chr> <dbl>  <dbl> <chr>   <chr>   <chr>   <chr>   <chr>  
    ##  1 2020… Snoho… Wash… 53061     1      0 050000… Snohom… 786620  null    *****  
    ##  2 2020… Snoho… Wash… 53061     1      0 050000… Snohom… 786620  null    *****  
    ##  3 2020… Snoho… Wash… 53061     1      0 050000… Snohom… 786620  null    *****  
    ##  4 2020… Cook   Illi… 17031     1      0 050000… Cook C… 5223719 null    *****  
    ##  5 2020… Snoho… Wash… 53061     1      0 050000… Snohom… 786620  null    *****  
    ##  6 2020… Orange Cali… 06059     1      0 050000… Orange… 3164182 null    *****  
    ##  7 2020… Cook   Illi… 17031     1      0 050000… Cook C… 5223719 null    *****  
    ##  8 2020… Snoho… Wash… 53061     1      0 050000… Snohom… 786620  null    *****  
    ##  9 2020… Maric… Ariz… 04013     1      0 050000… Marico… 4253913 null    *****  
    ## 10 2020… Los A… Cali… 06037     1      0 050000… Los An… 100980… null    *****  
    ## # … with 2,502,822 more rows, 2 more variables:
    ## #   `Annotation of Margin of Error!!Total` <chr>, `NA` <lgl>, and abbreviated
    ## #   variable names ¹​Geography, ²​`Geographic Area Name`, ³​`Estimate!!Total`,
    ## #   ⁴​`Annotation of Estimate!!Total`, ⁵​`Margin of Error!!Total`

For convenience, I down-select some columns and produce more convenient
column names.

``` r
## NOTE: No need to change; run this to produce a more convenient tibble
df_data <-
  df_q4 %>%
  select(
    date,
    county,
    state,
    fips,
    cases,
    deaths,
    population = `Estimate!!Total`
  )
```

# Analyze

<!-- -------------------------------------------------- -->

Now that we’ve done the hard work of loading and wrangling the data, we
can finally start our analysis. Our first step will be to produce county
population-normalized cases and death counts. Then we will explore the
data.

## Normalize

<!-- ------------------------- -->

### **q5** Use the `population` estimates in `df_data` to normalize `cases` and `deaths` to produce per 100,000 counts \[3\]. Store these values in the columns `cases_per100k` and `deaths_per100k`.

``` r
## TASK: Normalize cases and deaths
df_normalized <-
  df_data %>%
  mutate(
    date = lubridate::ymd(date),
    population = as.double(population)
  ) %>% 
  mutate(cases_per100k = (cases / population) * 100000) %>%
  mutate(deaths_per100k = (deaths / population) * 100000)
df_normalized
```

    ## # A tibble: 2,502,832 × 9
    ##    date       county      state      fips  cases deaths popula…¹ cases…² death…³
    ##    <date>     <chr>       <chr>      <chr> <dbl>  <dbl>    <dbl>   <dbl>   <dbl>
    ##  1 2020-01-21 Snohomish   Washington 53061     1      0   786620 0.127         0
    ##  2 2020-01-22 Snohomish   Washington 53061     1      0   786620 0.127         0
    ##  3 2020-01-23 Snohomish   Washington 53061     1      0   786620 0.127         0
    ##  4 2020-01-24 Cook        Illinois   17031     1      0  5223719 0.0191        0
    ##  5 2020-01-24 Snohomish   Washington 53061     1      0   786620 0.127         0
    ##  6 2020-01-25 Orange      California 06059     1      0  3164182 0.0316        0
    ##  7 2020-01-25 Cook        Illinois   17031     1      0  5223719 0.0191        0
    ##  8 2020-01-25 Snohomish   Washington 53061     1      0   786620 0.127         0
    ##  9 2020-01-26 Maricopa    Arizona    04013     1      0  4253913 0.0235        0
    ## 10 2020-01-26 Los Angeles California 06037     1      0 10098052 0.00990       0
    ## # … with 2,502,822 more rows, and abbreviated variable names ¹​population,
    ## #   ²​cases_per100k, ³​deaths_per100k

You may use the following test to check your work.

``` r
## NOTE: No need to change this
## Check known county data
if (any(df_normalized %>% pull(date) %>% str_detect(., "2020-01-21"))) {
  assertthat::assert_that(TRUE)
} else {
  print(str_c(
    "Date 2020-01-21 not found; did you download the historical data (correct),",
    "or just the most recent data (incorrect)?",
    sep = " "
  ))
  assertthat::assert_that(FALSE)
}
```

    ## [1] TRUE

``` r
assertthat::assert_that(
              abs(df_normalized %>%
               filter(
                 str_detect(county, "Snohomish"),
                 date == "2020-01-21"
               ) %>%
              pull(cases_per100k) - 0.127) < 1e-3
            )
```

    ## [1] TRUE

``` r
assertthat::assert_that(
              abs(df_normalized %>%
               filter(
                 str_detect(county, "Snohomish"),
                 date == "2020-01-21"
               ) %>%
              pull(deaths_per100k) - 0) < 1e-3
            )
```

    ## [1] TRUE

``` r
print("Excellent!")
```

    ## [1] "Excellent!"

## Guided EDA

<!-- ------------------------- -->

Before turning you loose, let’s complete a couple guided EDA tasks.

### **q6** Compute the mean and standard deviation for `cases_per100k` and `deaths_per100k`.

``` r
## TASK: Compute mean and sd for cases_per100k and deaths_per100k
case_mean <-
  mean(df_normalized$cases_per100k, na.rm = TRUE)
print(case_mean)
```

    ## [1] 9974.675

``` r
case_sd <-
  sd(df_normalized$cases_per100k, na.rm = TRUE)
print(case_sd)
```

    ## [1] 8448.659

``` r
death_mean <-
  mean(df_normalized$deaths_per100k, na.rm = TRUE)
print(death_mean)
```

    ## [1] 174.3095

``` r
death_sd <-
  sd(df_normalized$deaths_per100k, na.rm = TRUE)
print(death_sd)
```

    ## [1] 158.9641

### **q7** Find the top 10 counties in terms of `cases_per100k`, and the top 10 in terms of `deaths_per100k`. Report the population of each county along with the per-100,000 counts. Compare the counts against the mean values you found in q6. Note any observations.

``` r
## TASK: Find the top 10 max cases_per100k counties; report populations as well
case_top_10 <-
  df_normalized %>%
  arrange(desc(cases_per100k)) %>%
  distinct(county, .keep_all = TRUE)
case_top_10 <-
  case_top_10[0:10,]
case_top_10
```

    ## # A tibble: 10 × 9
    ##    date       county            state fips  cases deaths popul…¹ cases…² death…³
    ##    <date>     <chr>             <chr> <chr> <dbl>  <dbl>   <dbl>   <dbl>   <dbl>
    ##  1 2022-05-12 Loving            Texas 48301   196      1     102 192157.   980. 
    ##  2 2022-05-11 Chattahoochee     Geor… 13053  7486     22   10767  69527.   204. 
    ##  3 2022-05-11 Nome Census Area  Alas… 02180  6245      5    9925  62922.    50.4
    ##  4 2022-05-11 Northwest Arctic… Alas… 02188  4837     13    7734  62542.   168. 
    ##  5 2022-05-13 Crowley           Colo… 08025  3347     30    5630  59449.   533. 
    ##  6 2022-05-11 Bethel Census Ar… Alas… 02050 10362     41   18040  57439.   227. 
    ##  7 2022-03-30 Dewey             Sout… 46041  3139     42    5779  54317.   727. 
    ##  8 2022-05-12 Dimmit            Texas 48127  5760     51   10663  54019.   478. 
    ##  9 2022-05-12 Jim Hogg          Texas 48247  2648     22    5282  50133.   417. 
    ## 10 2022-05-11 Kusilvak Census … Alas… 02158  4084     14    8198  49817.   171. 
    ## # … with abbreviated variable names ¹​population, ²​cases_per100k,
    ## #   ³​deaths_per100k

``` r
## TASK: Find the top 10 deaths_per100k counties; report populations as well
death_top_10 <-
  df_normalized %>%
  arrange(desc(deaths_per100k)) %>%
  distinct(county, .keep_all = TRUE)
death_top_10 <-
  death_top_10[0:10,]
death_top_10
```

    ## # A tibble: 10 × 9
    ##    date       county            state fips  cases deaths popul…¹ cases…² death…³
    ##    <date>     <chr>             <chr> <chr> <dbl>  <dbl>   <dbl>   <dbl>   <dbl>
    ##  1 2022-02-19 McMullen          Texas 48311   166      9     662  25076.   1360.
    ##  2 2022-04-27 Galax city        Virg… 51640  2551     78    6638  38430.   1175.
    ##  3 2022-03-10 Motley            Texas 48345   271     13    1156  23443.   1125.
    ##  4 2022-04-20 Hancock           Geor… 13141  1577     90    8535  18477.   1054.
    ##  5 2022-04-19 Emporia city      Virg… 51595  1169     55    5381  21725.   1022.
    ##  6 2022-04-27 Towns             Geor… 13281  2396    116   11417  20986.   1016.
    ##  7 2022-02-14 Jerauld           Sout… 46073   404     20    2029  19911.    986.
    ##  8 2022-03-04 Loving            Texas 48301   165      1     102 161765.    980.
    ##  9 2022-02-03 Robertson         Kent… 21201   570     21    2143  26598.    980.
    ## 10 2022-05-05 Martinsville city Virg… 51690  3452    124   13101  26349.    946.
    ## # … with abbreviated variable names ¹​population, ²​cases_per100k,
    ## #   ³​deaths_per100k

**Observations**:

- The top ten counties for cases_per100k have cases_per100k values that
  are over five times the mean value for cases_per100k (9974.675). One
  important similarity to note between these counties is that they all
  have populations under 20,000. This means that one death affects this
  ratio significantly more than a more populous county like one that may
  have a population of 100,000. All of the peak weeks in these ten
  counties occurred in May of 2022. Loving County is an anomaly in this
  group of counties, nearly tripling the cases_per100k of the following
  county. We also see that Loving County has more cases than people,
  which could be due to many different reasons. Some possible reasons
  are counting reinfected people or the population not being updated for
  some time.

  In terms of the top ten counties for deaths_per100k, we have no major
  outliers in the death rate. The death rate of the top ten ranges from
  approximately 946 to 1359 deaths per 100,000 people. For reference,
  the mean deaths per 100,000 people of the dataset was about 174
  people. Similarly to before, the population for these counties is
  relatively low, the smallest county having a population of 102 and the
  largest having a population of 13,101. The weeks these peak death
  rates occurred spanned across the first half of 2022.

## Self-directed EDA

<!-- ------------------------- -->

### **q8** Drive your own ship: You’ve just put together a very rich dataset; you now get to explore! Pick your own direction and generate at least one punchline figure to document an interesting finding. I give a couple tips & ideas below:

### Ideas

<!-- ------------------------- -->

- Look for outliers.
- Try web searching for news stories in some of the outlier counties.
- Investigate relationships between county population and counts.
- Do a deep-dive on counties that are important to you (e.g. where you
  or your family live).
- Fix the *geographic exceptions* noted below to study New York City.
- Your own idea!

<!-- -->

``` r
df_report_start <-
  df_normalized %>%
  group_by(county) %>%
  mutate(report_start = min(date)) %>%
  filter(date == report_start) %>%
  mutate(state_abbreviate = state.abb[match(state,state.name)]) %>%
  drop_na(state_abbreviate)
df_report_start
```

    ## # A tibble: 1,866 × 11
    ## # Groups:   county [1,850]
    ##    date       county state fips  cases deaths popul…¹ cases…² death…³ report_s…⁴
    ##    <date>     <chr>  <chr> <chr> <dbl>  <dbl>   <dbl>   <dbl>   <dbl> <date>    
    ##  1 2020-01-21 Snoho… Wash… 53061     1      0  7.87e5 0.127         0 2020-01-21
    ##  2 2020-01-24 Cook   Illi… 17031     1      0  5.22e6 0.0191        0 2020-01-24
    ##  3 2020-01-25 Orange Cali… 06059     1      0  3.16e6 0.0316        0 2020-01-25
    ##  4 2020-01-26 Maric… Ariz… 04013     1      0  4.25e6 0.0235        0 2020-01-26
    ##  5 2020-01-26 Los A… Cali… 06037     1      0  1.01e7 0.00990       0 2020-01-26
    ##  6 2020-01-31 Santa… Cali… 06085     1      0  1.92e6 0.0520        0 2020-01-31
    ##  7 2020-02-01 Suffo… Mass… 25025     1      0  7.92e5 0.126         0 2020-02-01
    ##  8 2020-02-02 San F… Cali… 06075     2      0  8.70e5 0.230         0 2020-02-02
    ##  9 2020-02-05 Dane   Wisc… 55025     1      0  5.30e5 0.189         0 2020-02-05
    ## 10 2020-02-10 San D… Cali… 06073     1      0  3.30e6 0.0303        0 2020-02-10
    ## # … with 1,856 more rows, 1 more variable: state_abbreviate <chr>, and
    ## #   abbreviated variable names ¹​population, ²​cases_per100k, ³​deaths_per100k,
    ## #   ⁴​report_start

``` r
df_report_start_no_tx <-
  df_report_start %>%
  filter(county != "Pending County Assignment")

df_state_vs_date <-
  df_report_start %>%
  ggplot(
    mapping = aes(state_abbreviate, date)
  ) +
  geom_boxplot() +
  theme_minimal() +
  theme(axis.text.x = element_text(angle = 90, vjust = 0.4)) +
  xlab("State") +
  ylab("Starting Report Date") +
  ylim(as.Date(c("2020-01-01", "2022-06-01")))
df_state_vs_date
```

![](c06-covid19-assignment_files/figure-gfm/unnamed-chunk-1-1.png)<!-- -->

``` r
df_state_vs_date_no_tx <-
  df_report_start_no_tx %>%
  ggplot(
    mapping = aes(state_abbreviate, date)
  ) +
  geom_boxplot() +
  theme_minimal() +
  theme(axis.text.x = element_text(angle = 90, vjust = 0.4)) +
  xlab("State") +
  ylab("Starting Report Date") +
  ylim(as.Date(c("2020-01-01", "2021-01-01")))
df_state_vs_date_no_tx
```

![](c06-covid19-assignment_files/figure-gfm/unnamed-chunk-1-2.png)<!-- -->

The graph that I made is a boxplot visualizing the starting report date
across counties for each state. From the data we have, we can see that
different counties started reporting their COVID-19 data at different
times, all before 2021 except for one county. This county is shown in
the first graph and is located in Texas, having a starting reporting
date in May of 2022. The unfortunate thing about this county is that it
is pending county assignment so there isn’t a searchable way to learn
more about this county. To help see the rest of the date better, I
removed that county and made a new boxplot graph. With this graph we are
able to see that the median starting report date for a county is in
March of 2020 for most states in America. The states that span a larger
than average range are Alaska, Montana, North Dakota, Nebraska, Nevada,
and South Dakota. There are many factors that could cause these larger
ranges but one that came to mind was how long a mask mandate was
enforced in the state. This may indicate the concern of the state with
COVID-19, whether it be with wearing masks or reporting data. I noticed
that many of the states either didn’t have any mask mandate or were in
the bottom half of states in terms of length of mask mandate
(Balletopedia). The only one of these states that did not follow this
pattern was Nevada. One reason this may be is that Las Vegas is a large
tourist city where masks could be more important to have while a lot of
the rest of Nevada is not as densely populated. The more remote counties
of Nevada could be less concerned and Nevada does tend to be more of a
swing state politically. Another trend that we can see with the data is
that there are a lot out outliers, with more outliers later than the
rest of the data points rather than earlier. Despite states taking a
stance on their concern regarding COVID-19, the counties themselves have
different views and may be less concerned with COVID. Some counties
could also report later if they did not get any COVID cases until later
due to a smaller population or people not traveling in or out of the
county. The variation among counties is so large for many states due to
the different responses of counties to COVID and when counties got their
first COVID case.

<https://ballotpedia.org/State-level_mask_requirements_in_response_to_the_coronavirus_(COVID-19)_pandemic,_2020-2022>

### Aside: Some visualization tricks

<!-- ------------------------- -->

These data get a little busy, so it’s helpful to know a few `ggplot`
tricks to help with the visualization. Here’s an example focused on
Massachusetts.

``` r
## NOTE: No need to change this; just an example
df_normalized %>%
  filter(state == "Massachusetts") %>%

  ggplot(
    aes(date, cases_per100k, color = fct_reorder2(county, date, cases_per100k))
  ) +
  geom_line() +
  scale_y_log10(labels = scales::label_number_si()) +
  scale_color_discrete(name = "County") +
  theme_minimal() +
  labs(
    x = "Date",
    y = "Cases (per 100,000 persons)"
  )
```

    ## Warning: `label_number_si()` was deprecated in scales 1.2.0.
    ## ℹ Please use the `scale_cut` argument of `label_number()` instead.

    ## Warning: Removed 789 rows containing missing values (`geom_line()`).

![](c06-covid19-assignment_files/figure-gfm/ma-example-1.png)<!-- -->

*Tricks*:

- I use `fct_reorder2` to *re-order* the color labels such that the
  color in the legend on the right is ordered the same as the vertical
  order of rightmost points on the curves. This makes it easier to
  reference the legend.
- I manually set the `name` of the color scale in order to avoid
  reporting the `fct_reorder2` call.
- I use `scales::label_number_si` to make the vertical labels more
  readable.
- I use `theme_minimal()` to clean up the theme a bit.
- I use `labs()` to give manual labels.

### Geographic exceptions

<!-- ------------------------- -->

The NYT repo documents some [geographic
exceptions](https://github.com/nytimes/covid-19-data#geographic-exceptions);
the data for New York, Kings, Queens, Bronx and Richmond counties are
consolidated under “New York City” *without* a fips code. Thus the
normalized counts in `df_normalized` are `NA`. To fix this, you would
need to merge the population data from the New York City counties, and
manually normalize the data.

# Notes

<!-- -------------------------------------------------- -->

\[1\] The census used to have many, many questions, but the ACS was
created in 2010 to remove some questions and shorten the census. You can
learn more in [this wonderful visual
history](https://pudding.cool/2020/03/census-history/) of the census.

\[2\] FIPS stands for [Federal Information Processing
Standards](https://en.wikipedia.org/wiki/Federal_Information_Processing_Standards);
these are computer standards issued by NIST for things such as
government data.

\[3\] Demographers often report statistics not in percentages (per 100
people), but rather in per 100,000 persons. This is [not always the
case](https://stats.stackexchange.com/questions/12810/why-do-demographers-give-rates-per-100-000-people)
though!
