# radvax_experiences

# Experiences with RadVax

RadVax is an open-source vaccine, freely available for anyone to make.  Currently the vaccine is experimental, and each user taking it has chosen to do so knowing that it was designed and predicted to be safe, but that no formal studies have been undertaken (although the RaDVaC group is seeking partners for clinical trials).

The dataset here serves two purposes:
1. It lets you see what has happened with users in the past
2. It lets you submit your own experience, so future potential users can evaluate

The dataset is available in this repository in the [radvax_exp.tsv](/radvax_exp.tsv) file , and anyone is free to view or download it.  The datafile is a "tab-separated" file, which can be read by any text reader. To read it with a spreadsheet program (such as MS Excel), you may need to specify "tab" as the separator.  

If you wish to submit your own experience with using RadVax, you may do so through one of two methods:

1. Fill out the questions asked below, and email the answers to us.
2. Download the file of past experiences, add your own entry to the bottom, and then submit a Pull Request (this method is preferred, if you are capable of doing so).

As with all citizen-science projects, we're relying on you to report your results honestly.  We will do some very basic quality control (e.g. if you submit information about a previous record using a different email address, we'll want to know why), but ultimately we're counting on you.

Remember that this information is available for anyone to see, so don't submit anything you aren't comfortable with sharing publicly.  If you need help with submission, you can email us.


# Questions
To reduce hassle, we've broken the questions into 3 groups.  The first group is the most important (basically, were there any side-effects?).  The second group of questions is traits about you, which might let people learn if there are systematic variations in response (for instance, perhaps women are more likely to get headaches after taking RadVax, or mestizos are more likely to experience a stuffy nose).  The third group of questions are potentially interesting, but not critical.  Please fill them out if convenient, but don't feel bad if you're unable to.

## About side-effects
- unique ID (see below for instructions on making your own unique identifier)
- In the week after taking RadVax, did you notice physical symptoms?
- Including this dose, how many doses of RadVax have you taken?

## About you
- age at time of first RadVax dose
- gender
- ethnicity

## Other questions
- RadVax dose date (approx):  YYYY/MM/DD
- RadVax generation, if known
- Any other comments?


## Using a unique ID
To enable your data to be shared without revealing your personal information, you should submit your experience along with a unique identifier.  You may use any method to generate it, but the following method is both easy and secure.  Basically, you will just run your name through a "hash function", and use the output.  If you're interested, you can learn more [here](https://www.kalzumeus.com/essays/dropping-hashes/)

### Generating your hashed name using DuckDuckGo
- Go to the website [DuckDuckGo.com](https://duckduckgo.com/)
- enter SHA, followed by your name: `SHA "Firstname Lastname"`.  For instance, Jane Doe would enter her name as follows:
![DuckDuckGo homepage, with 'SHA "Jane Doe"' in the search box](/figs/DDG__homepage.png)

- Copy the output; that code is your unique identifier (and no one can reverse it to learn your name).  Jane's unique identifier is `cac7bbb6b67b44ea0ab997d34a88e4ea9b4d3d62`
![DuckDuckGo returns page, showing Jane's unique ID](/figs/DDG__Jane_Doe.png)

- That's it!

- If you ever need to get your identifier again, just repeat the above steps.  Be sure to spell your name exactly the same, including capitalization.  The difference of a single letter will drastically change the output of the hashing function.  For instance, if Jane forgets to capitalise her first name, and types `SHA "jane Doe"`, the output becomes:
![DuckDuckGo returns page, showing a different output when name is not capitalized](/figs/DDG__jane_Doe.png)
