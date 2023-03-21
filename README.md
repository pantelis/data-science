# data-science

Introduction to Data Science Course Content

## Usage

### Building the book

#### HTML 
If you'd like to develop and/or build the data-science book, you should:

1. Clone this repository
2. Run `conda env update --file environment.yml`
3. Run `conda activate data-mining-book`
4. (Optional) Edit the source files located in the `data_science/` directory
5. Run `jupyter-book clean data_science/` to remove any existing builds
6. Run `poetry run sphinx-autobuild data_science/ _build/html`

A fully-rendered HTML version of the book will be built in `data_science/_build/html/`.

#### PDF 

Simply run `jb build data_science --force --builder pdflatex`
   
### Hosting the book

In this repo the book is automatically built and deployed to GitHub Pages using GitHub Actions. The workflow file is located in `.github/workflows/deploy.yml`.

Please see the [Jupyter Book documentation](https://jupyterbook.org/publish/web.html) to discover other options for deploying a book online using services such as GitHub, GitLab, or Netlify.

For GitHub and GitLab deployment specifically, the [cookiecutter-jupyter-book](https://github.com/executablebooks/cookiecutter-jupyter-book) includes templates for, and information about, optional continuous integration (CI) workflow files to help easily and automatically deploy books online with GitHub or GitLab. For example, if you chose `github` for the `include_ci` cookiecutter option, your book template was created with a GitHub actions workflow file that, once pushed to GitHub, automatically renders and pushes your book to the `gh-pages` branch of your repo and hosts it on GitHub Pages when a push or pull request is made to the main branch.


## Contributing

We welcome all pull requests that can take the form of new text suggestions or simply indicating the place where the book can be improved. Please see the [contributing guidelines](CONTRIBUTING.md) for more information.