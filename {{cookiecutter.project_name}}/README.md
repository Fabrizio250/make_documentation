# {{cookiecutter.project_name}}

**Author**: {{cookiecutter.author_name}}

**Email**: {{cookiecutter.author_email}}

**Version**: {{cookiecutter.project_version}}

{{cookiecutter.project_description}}

## Repository structure
```
│── .github                      <- directory containing configurations for Github Actions 
│   └── workflows         
├── data
│   ├── external                 <- Data from third party sources.
│   ├── interim                  <- Intermediate data that has been transformed.
│   ├── processed                <- The final, canonical data sets for modeling.
│   └── raw                      <- The original, immutable data dump.
├── docs                         <- Directory for documentation.
│   ├── maker_documentation      <- Directory for creating documents
│   ├── md_docs                  <- Directory containing documentation in Markdown format(created post)
│   └── source                   <- Directory containing documentation template              
│       └── template_docs         
├── example                      <- Directory for test scripts and src.
├── models                       <- Trained and serialized models, model predictions, or model summaries.
├── notebooks                    <- Directory with Jupyter notebooks.
├── references                   <- Directory containing project references.
├── reports                      <- Generated HTML, PDF, LaTeX, etc. reports.
│   └── figures                  <- Graphs and figures generated to use in reports.
├── src                          <- Project source code.
│   ├── data                     <- Scripts to download or generate data.
│   ├── features                 <- Scripts to turn raw data into features.
│   ├── models                   <- Scripts to train and use models.        
│   └── visualization            <- Scripts to create visualizations.
├── test                         <- Project test code.
│   ├── data           
│   ├── features       
│   ├── models             
│   └── visualization  
├── Makefile                     <- Makefile with `make install_requirements` command.
├── README.md                    <- Project markdown file created.
└── requirements.txt             <- Txt file containing all requirements to install in venv.
```