---
layout: post
title:  "Comping to Python from Perl: What I like, dislike, and find strange!"
date:   2023-02-28 13:45:00 -0000
categories: python perl programming syntax
---

I have been codong in Perl for well over a decade at this point. The reason I got into Perl was because of its widespread use in bioinformatics. Therefore, I used Perl a lot, spanning the time I spent doing my master's, PhD, and PostDoc. However, even during my PhD, the transition towards Python was already underway. This is now mostly complete owing to the rise of machine learning and artificial intelligence, which mostly uses Python and the massive amounts of biological data available. Hence, learning Python is no longer a choice. Having done a fair amount of coding in Python, I would like to reflect on my journey into this language. Obviously, this a cary personal take on the matter. It will be very different for someone else.

## The Good

### $, @, and %
In Perl, variables start with the $, @ and % signs depending on whether they are scalars, arrays, or hashes. Thankfully, variables in Python don't come with this unnecessary overhead. In Python, you can just create a variable using the proper syntax and the Python intrepeter will assign it the correct type. You can just focus on your problem and not spend time prefixing variable names with the correct symbols.

Related to this, there are other Perl symbols which are unnecessary, like the ";" at the end of each statement.

### Pointers
Whaen a Perl code returns a variable, the entire variable is passed to the calling command. Obviously, this is not viable for large arrays and hashes. Therefore, one has to pass a reference to the variable.

In Perl, one would do this,

    @numbers = [1, 2; 3; 4; 5];
    return \@numbers;

Whereas, in Python, it is quite simple

    numbers = [1, 2, 3, 4, 5]
        return numbers


It could be quite difficult for a new programmer to learn this detail. Hence, unless it causes a problem, someone could end up doing bad programming for ever. In Python, this is all taken care of by the language, which is very convenient to say the least. As a new Python programmer, I spent some time checkinghow to pass references before realizing that it was unnecessary because in Python every variable is a reference to an object!

### Installation
Fortunately, systems versions of both Perl and Python are available in UNIX-like systems. However, one might need to work with different versions of these programs, or install modules, all of which can interfere with the system Perl or Python. 

For Perl, I have used [PerlBrew](https://perlbrew.pl/), which makes it easy to use and switch between different versions of Perl.

Python achieves this whith the help of a virtual environment, which can additionally also contain packages and their dependencies. This strikes me as a better way of organizing and distributing programs.
### Virtual environments
As mentioned above, virtual environments are cool. The ability of contenarize all the dependencies of a project is indeed powerful and convenient. Virtual environments can be implemented in Python using three different tools:
- venv
-pyenv
- pyenv-virtualenv

`venv` commands for creating, activating, and deactivating new environments are:
    $ python3 -m venv directory-name
    $ source directory-name/bin/activate
    $ deactivate

Packages and dependencies can be installed via **pip**, usually by including a requirements.txt file, and using `pip install -r requirements.txt`. 

When additional versions of python are needed, `pyenv` can be used. I haven't used it yet, so can't comment. `pyenv-virtualenv` is a tool to create virtual environments integrated with `pyenv`. It also works with the Anaconda and Miniconda environments.

### Machine Learning and AI

## The Bad

### Regex

## The Strange

### Indentation