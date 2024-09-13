# SOUP List (Software of Unknown Provenance)

> The 62304 requires you to document your SOUP, which is short for Software of Unknown Provenance. In human
> language, those are the third-party libraries you're using in your code, typically in your
> `requirements.txt` or `Gemfile`.

| Classes | IEC 62304:2006 Section                          | Document Section |
|---------|-------------------------------------------------|------------------|
| B, C    | 5.3.3 (Functional and Performance Requirements) | 2                |
| B, C    | 5.3.4 (Hardware and Software Requirements)      | 2                |
| B, C    | 7.1.2 (Hazardous Situations)                    | 2                |
| B, C    | 7.1.3 (SOUP Anomaly Lists)                      | 2                |
| A, B, C | 8.1.2 (Identify SOUP)                           | 2                |

## 1 Risk Level Definitions

> The 62304 requires you to assess risks associated with SOUP. The simplest way to do this is to classify each
> SOUP as a certain risk level. Unless you're developing software which shoots radiation at patients, it's
> likely that your SOUP risk levels remain "low" or "medium".

| Risk Level | Definition                                                 |
|------------|------------------------------------------------------------|
| Low        | Malfunction in SOUP can't lead to patient harm.            |
| Medium     | Malfunction in SOUP can lead to reversible patient harm.   |
| High       | Malfunction in SOUP can lead to irreversible patient harm. |

## 2 SOUP List

> This is the actual SOUP list. For each third-party library you use, add an entry in the table below. The
> idea is to only have one "global" SOUP list for your medical device even though the code may actually live
> in multiple repositories. That's what the "software system" column is for; you could also mention your (git)
> repository there.

> When specifying requirements, the 62304 requires you to mention functional, performance, hard- and software
> requirements. However, you may not have to re-state certain requirements if they apply to all SOUP,
> e.g., "runs on Linux". So prefer to keep the requirements simple, in a way in which you would communicate them
> to colleagues on your development team when answering the question "why did we import this library?".

> As with all templates: It's more about the content (i.e., the columns you see below) than the tool (filling
> this out in Google sheets / markdown / wherever). Nobody says that you have to maintain this as a Google
> sheet. If you can find a way to integrate this in your workflow in a better way, e.g., in a markdown file in
> your git repository, go for it! Just keep in mind that you need to be able to export it to send it to
> auditors.

| ID | Software System | Package Name | Programming Language | Version | Website                                          | Last verified at | Risk Level | Requirements               | Verification Reasoning                                                    |
|----|-----------------|--------------|----------------------|---------|--------------------------------------------------|------------------|------------|----------------------------|---------------------------------------------------------------------------|
| 1 | OS Independent | mlflow | Python | 2.16.1 | [unknown](unknown) | 2024-09-13 | N/A | N/A | N/A |
| 2 | Unknown | dvc | Python | 3.55.2 | [unknown](unknown) | 2024-09-02 | N/A | N/A | N/A |
| 3 | OS Independent | ruff | Python | 0.6.5 | [https://docs.astral.sh/ruff](https://docs.astral.sh/ruff) | 2024-09-13 | N/A | N/A | N/A |
| 4 | Unknown | codecarbon | Python | 2.7.1 | [unknown](unknown) | 2024-09-11 | N/A | N/A | N/A |
| 5 | MacOS | pytest | Python | 8.3.3 | [unknown](unknown) | 2024-09-10 | N/A | N/A | N/A |
| 6 | Unknown | pynblint | Python | 0.1.6 | [https://pynblint.readthedocs.io/en/latest/](https://pynblint.readthedocs.io/en/latest/) | 2024-08-12 | N/A | N/A | N/A |
| 7 | MacOS X | bandit | Python | 1.7.9 | [https://bandit.readthedocs.io/](https://bandit.readthedocs.io/) | 2024-06-12 | N/A | N/A | N/A |
| 8 | Unknown | mypy | Unknown | 1.11.2 | [https://www.mypy-lang.org/](https://www.mypy-lang.org/) | 2024-08-24 | N/A | N/A | N/A |
| 9 | Unknown | deepchecks | Python | 0.18.1 | [https://github.com/deepchecks/deepchecks](https://github.com/deepchecks/deepchecks) | 2024-01-31 | N/A | N/A | N/A |
| 10 | MacOS | numpy | Python | 1.26.4 | [https://numpy.org](https://numpy.org) | 2024-09-03 | N/A | N/A | N/A |
| 11 | MacOS | scipy | Python | 1.10.1 | [https://scipy.org/](https://scipy.org/) | 2024-08-21 | N/A | N/A | N/A |
| 12 | OS Independent | seaborn | Python | 0.13.2 | [unknown](unknown) | 2024-01-25 | N/A | N/A | N/A |
| 13 | OS Independent | Jinja2 | Python | 3.1.4 | [unknown](unknown) | 2024-05-05 | N/A | N/A | N/A |
| 14 | OS Independent | pandas | Python | 2.1.4 | [https://pandas.pydata.org](https://pandas.pydata.org) | 2024-04-10 | N/A | N/A | N/A |
| 15 | OS Independent | requests | Python | 2.32.3 | [https://requests.readthedocs.io](https://requests.readthedocs.io) | 2024-05-29 | N/A | N/A | N/A |
| 16 | Unknown | matplotlib | Python | 3.9.2 | [unknown](unknown) | 2024-08-13 | N/A | N/A | N/A |



---
Template Copyright [openregulatory.com](https://openregulatory.com). See [template
license](https://openregulatory.com/template-license).

Please don't remove this notice even if you've modified contents of this template.