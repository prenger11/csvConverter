# Make an HTML document out of a spreadsheet of new books

- This script was developed to solve a specific problem faced by our librarians: how to turn a spreadsheet of new books into an HTML document quickly and easily.

- So the script I wrote automatically produces an HTML output from a CSV file. This HTML is suitable for cutting and pasting into a LibGuide.

## To use the script


    $ git clone https://github.com/markeeaton/new-books   
    $ cd new-books   
    $ pipenv install  

Then you should have your input spreadsheet organized as follows:

|    A     |    B   |    C  |    D        |
|:--------:|:------:|:-----:|:-----------:|
| LC Class | Author | Title | Call Number |
|   ...    |   ...  |  ...  |     ...     |

- Be sure to include a row with column headers!
- The data goes below. 
- Save it as a CSV file. Place it in the `new-books/data/` directory.

Once that's set up, you can use the convert script by replacing `input.csv` and `output.html` in this command with your own filenames:

`$ pipenv run python convert.py input.csv output.html`

The output file will be in the `data/` directory.
