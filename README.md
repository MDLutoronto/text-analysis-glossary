<img align="left" src="./images/CC_BY.png" alt="Left aligned icon"><br /><br />
Created by [Nathan Kelber](http://nkelber.com) for [JSTOR Labs](https://labs.jstor.org/) under [Creative Commons CC BY License](https://creativecommons.org/licenses/by/4.0/)<br />
Adapted by [Neil Aitken](https://neil-aitken.com) for [Map & Data Library at the University of Toronto](https://mdl.library.utoronto.ca/) <br />
For questions/comments/improvements, email neil.aitken@utoronto.ca.<br />
___

# Text Analysis Glossary

A set of common text analysis terms with their definitions. This notebook does not contain executable code.

<a id="api"></a>
## Application Programming Interface (API)
A protocol that defines communication between a client and server, often used to request data. APIs can help retrieve data from remote repositories, anything from weather to social media data.

<a id="argument"></a>
## Argument (in Python)
An input that is passed into a function. For example,

`print('Hello World')`

passes the argument `'Hello World'` (a string variable) into a `print()` function.

## Artificial Intelligence
The science of making intelligent machines, especially machines that react to input data in a way similar to a human being. Historically, artificial intelligence has tended to rely on simple if-then statements (e.g. if the user mentions their mother, ask how she is doing), but recent advancements in artificial intelligence have focused on machine learning and generative content.

## Assignment Statement (in Python)

A statement that creates and/or changes a variable. For example,

`new_variable = 7`

Note that assignment statements use a single `=` sign. They should not be confused with the equality comparison operator `==`, which compares whether two values are equal and returns a boolean value, either **True** or **False**.

## Bag of Words (Model)
A model of texts that counts individual words without regard to grammatical location or phrases. Just as the letters of a Scrabble game are tossed into a bag without order, a "bag of words" model gathers all the words of a text into a "bag" with no regard to where a particular word occurs within the document. In this model, the reader knows every word and its frequency within the text but does not have the context of the word's use.

## Bibliographic Metadata
Also known as "descriptive metadata," informational metadata that describes a published item such as a book or journal article.  Bibliographic metadata contains data elements to help users identify and retrieve the published items.   It often has a formalized bibliographic format.

## Bigram
An n-gram with a length of two. For example, "chicken stock" is a word bigram.

## Bayesian Classification
A classification method based on [Bayes' Theorem](https://en.wikipedia.org/wiki/Bayes%27_theorem) that describes the probability of an event based on available prior knowledge. For example, given a dataset of the historical weather conditions (temperature, humidity, windspeed) from December 25th for every year over the last century, will it snow on December 25th, 2027?

## Boolean Operator
The operators:
* and
* or
* not
which are used in flow control statements to connect or separate expressions that evaluate to Boolean values.

Assuming two expressions are connected by **and**, the combination will evaluate to **True** only if both individual expressions are **True**. 

|Expression|Evaluation|
|---|---|
|True and True|True|
|True and False|False|
|False and True|False|
|False and False|False|

Assuming two expressions are connected by **or**, the combination will evaluate to **False** only if both individual expressions are **False**

|Expression|Evaluation|
|---|---|
|True or True|True|
|True or False|True|
|False or True|True|
|False or False|False|

## Boolean Value (in Python)
A value of **True** or **False** (first letter must be capitalized) that is assigned to a variable, usually for the purpose of guiding a flow control statement. 

## Cell (in a Jupyter Notebook)
See Code Cell (in a Jupyter Notebook) and Markdown Cell (in a Jupyter Notebook). 

## Clean Data
Data that has been standardized and corrected for accurate results. This phrase can also be used as a verb such as "to clean data" or "cleaning data." (Data cleaning is sometimes called "munging.") In practice, data cleaning makes up the bulk of text analysis work. 

## Clustering
The statistical process of grouping together similar items. For example, topic analysis may cluster together sets of words that commonly co-occur, genre analysis may attempt to cluster similar genres, or authorship attribution may attempt to cluster novels by the same author. The clusters can be:

* Hard Clusters (mutually exclusive groups)
* Soft/Fuzzy Clusters (items may be in multiple groups)
* Hierarchal Clusters (part of hierarchy)

![visualization of cluster types](./images/clustering_types.png)

## Code Block (in Python)
A snippet of code that begins with an indentation. A code block can be a single line or many lines long. Blocks can contain other blocks forming a hierarchal structure. In such a case, the second block is indented an additional degree. Any given block ends when the number of indentations in the current line is less than the number that started the block. 

![Visualization of code block indentations](./images/code_block_indentation.png)

## Code Cell (in a Jupyter Notebook)
A cell in a Jupyter notebook that is executable. They can be distinguished by the presence of a set of brackets and a colon to the left of the cell. [ ]: 

See also, Markdown Cell (in a Jupyter Notebook). 

## Comparison Operator (in Python)

A way to compare two values in Python to see if they are equal, greater than, or less than. 

|Operator|Meaning|
|---|---|
|==|Equal to|
|!=|Not equal to|
|<|Less than|
|>|Greater than|
|<=|Less than or equal to|
|>=|Greater than or equal to|

Note that the equality comparison operator is `==`, whereas a variable assignment statement is `=`. An expression using a comparison operator will evaluate to a boolean value, either **True** or **False**. Comparison operators are used within flow control statements to determine which code should be executed next.

## Concordance
A text analysis method for creating a list of all the occurences of a particular word or phrase. 

## Concatenation (of strings in Python)

The joining of two or more strings such as with the addition operator.

> 'Hello ' + 'World' + '!'

evaluates to

> 'Hello World!'
> 

## Content Words
As opposed to function words (e.g. articles, pronouns, conjuctions), content words (e.g. nouns, verbs, and adjectives) carry greater lexical meaning. Word frequency analysis typically attempts to filter out function words, in order to make content words more prominent. This filtering is accomplished with a stop words list.

## Co-occurrence
When two words occur close to one another, usually within the same sentence. 

## Corpus
A large (and often structured) collection of texts used for analysis. For example, all of the plays written by Shakespeare. A simple example might be a set of plain text files in a folder on your computer. A more complicated example may use JSON, XML, or another form of markup, to allow for deeper analysis. The plural form is corpora.

See also TEI XML. 

## Counter (in Python)
A data type similar to a Python dictionary with a few key differences:
* A counter object with a value of zero or less, always returns 0
* When a key is called that doesn't exist in the counter, it returns 0 instead of an error like in a dictionary
* A counter object has additional methods for counting including `.most_common(x)` that returns the x most common values.
* Counter objects can be added, subtracted, as well as being modified through unions (&) and intersections (|)

## CSV (file)
A .csv file, or Comma-Separated Value file, is a simple format for storing structured data where each entry in the file is separated by a comma. Similarly, a TSV file uses tabs to separate individual data entries. 

## Dataframe (in Pandas)
The primary data structure for analysis, manipulation, and presentation of data with the Pandas library.

## Dataset
A collection of information, usually computer files, used for statistical analysis. Most datasets are digital text (either numbers, words, or both), but they can also be other formats such as image, audio, and/or video content. Datasets are usually referred to as structured, semi-structured, or unstructured.
* Structured data fits into a predetermined format and can usually be represented by a table, spreadsheet, or relational database. 
* Unstructured data is more freeform. For example, longform texts, audio, or video content are unstructured. 
* Semi-structured data uses tags or elements to mark out structures within an unstructured data set. Email files, for example, have both structured aspects (Sender, Subject, etc.), but the body of an email is usually unstructured.

## Descriptive Metadata
See bibliographic metadata.

## Dictionary (in Python)
A variable in Python that stores data in key/value pairs. This differs from a Python list which stores data in numberical order beginning with item 0.

## Dictionary (gensim)
A list created by gensim of all the words in a corpus. The command for creating a gensim dictionary:
>gensim.corpora.Dictionary(documents)

Each word in the corpus is assigned a unique gensim dictionary ID starting from 0. 

<a id="expression"</a>
## Expression (in Python)

A combination of values and operators in Python that evaluate to a single value. 

> 2 + 3

is an expression using the addition operator (+) that evaluates to 5.

## Floating-point number (float)
A float is a data type that contains a decimal number that can assigned to a variable as a value. (Other kinds of data types in Python include strings and integers.) 

|  Data type             | Examples                                      |
| -----------------------|:---------------------------------------------:|
| Integers               | -5, -3, 0, 5, 201                             |
| Floating-point numbers | -3.74, -3.14, 0.0, 503.4, 506                 | 
| Strings                | 'potatoes', 'Hello world!, 'no', '24 pizzas'  |

## Flow Control Statement (in Python)
A flow control statement guides the actions of a program, helping decide what code should be executed next depending on a series of tests such as:

* `if` statements
* `else` statements
* `elif` statements
* `while` loops
* `for` loops

## Function (in Python)
A small snippet of code that can be referenced and run easily without having to be rewritten over again. There are three kinds of functions in Python:

* Native functions built into Python
* Functions others have written that can be imported
* Functions a programmer defines themself

Functions often take an input, in the form of an argument, and return an output. 

## Function Words
The words in a sentence that have little lexical meaning and express grammatical relationships. Function words include articles, pronouns, and conjunctions. When using a word frequency approach, function words are often filtered out in favor of content words using a stopwords list. 

## Gensim
A python library for implementing various natural language processing methods, such as TF-IDF, Word2Vec, and Topic Modeling.

## git
A method for saving versions of your computer code that enables many people to work on a single project. The code is stored in a repository (or "repo"). The git software is often used with a cloud service, such as [GitHub](http://github.com) and [GitLab](http://gitlab.com). 

## Global Scope (in Python)
The entire scope of a program, not just the local scope of a particular function. A variable created in the global scope is a global variable that can be read from anywhere in the program. A global variable can be read within a local scope, but a local variable cannot be read at global scope.

## Global Statement (in Python)
A statement in the local scope of a function that declares a variable is a global variable. Without a global statement, the variable will be assumed to be a local variable during an assignment statement (even if there is a global variable with the same name). 

## Global Variable (in Python)
A variable created in the global scope of a program. A global variable can be read within a local scope, but a local variable cannot be read at global scope.

## Index Number (in Python)
The items contained in a Python List are kept in a strict numerical order by index number, starting from 0. 

## Integer
An integer is a data type that contains a whole number that can assigned to a variable as a value. (Other kinds of data types in Python include strings and floating point numbers.) 

|  Data type             | Examples                                      |
| -----------------------|:---------------------------------------------:|
| Integers               | -5, -3, 0, 5, 201                             |
| Floating-point numbers | -3.74, -3.14, 0.0, 503.4, 506                 | 
| Strings                | 'potatoes', 'Hello world!, 'no', '24 pizzas'  |

## JavaScript (Programming Language)
An object-oriented computer programming language often used to create interactive effects within webbrowsers.  Learn more at [w3schools](https://www.w3schools.com/js/default.asp).

## JSON (JavaScript Object Notation)
An open-standard file format for storing and exchanging data that is intended to be easy to read and write humans and machines. Like XML, JSON is often used by APIs to transmit data from a remote repository (say weather data or Twitter data) to a local machine. 

## JSON Lines
Also called newline-delimited JSON, JSON Lines (file extension .jsonl) is structured so it may be processed one record at a time. Each line is a valid value. The file extension for JSON Lines is ".jsonl".

## json (Python library)
A library for interpreting and converting JSON into Python code.

## JupyterHub
A multi-user version of The Jupyter Notebook, ideal for teaching environments.

## JupyterLab
The newest software from Project Jupyter, intended to replace The Jupyter Notebook, for executing and editing Jupyter notebook files.

## Jupyter Notebook, The (software)
A single-user web application for executing and editing Jupyter notebook files. Will be replaced by JupyterLab.

## Jupyter notebook (file)
A file with extension .ipynb that contains computer code (e.g. Python or R) alongside other explanatory media (text, images, video).

## Jupyter Server
A server with the appropriate software environment (e.g. JupyterHub, JupyterLab) for running and editing Jupyter notebooks.

## Key/Value Pair
A key/value pair is a data organizational structure where a key is associated with a unique value or set of values. For example, the user could supply the key **Age** and receive a value **58 years**. 

In Python, Key/Value pairs are a key organizational structure for dictionaries and Counters.

JSON also encodes key/value pairs, such as:

>"title": "The Souls of Black Folk"

where the key is "title" and the value is "The Souls of Black Folk". 

## Latent Dirichlet Allocation (LDA)
An algorithm commonly used for topic modeling. Pronounced (lay-tent deer-ish-lay al-lo-cay-shun).

## Lemmatization
The process of grouping together the conjugated forms of a word into a base form. For example, "jumping," "jumped," and "jumps" could be combined into "jump," the base form or *lemma*.

## Library (in Python)
A large collection of methods and functions for achieving certain tasks (e.g. image manipulation, web scraping). This saves time since the code can be added quickly and all at once around a specific group of tasks. The Natural Language Toolkit (NLTK) is a common library used in natural language processing.

## List (in Python)
A variable data type that stores items in numbered order beginning with item 0. The number for each item is called its index number. A list is different than a Python dictionary variable which stores data in key/value pairs. 

## List Comprehensions (in Python)
A short way to create a Python list. For example, if you have:
`list = [1,2,3,4,5,6,7,8,9,10]`
A list comprehension could help generate a smaller list that only contains the even numbers.
`evens_list = [x for x in list if x % 2 == 0]`
Each item in the original list is checked to see if `x % 2 == 0` (if there is no remainder after being divided by 2). The resulting value of `evens_list` is `[2, 4, 6, 8, 10].`

Alternatively, you could use a list comprehension to generate the evens_list from scratch. 

`evens_list = [x for x in range(11) if x % 2 == 0]`

This would create a list, using the range from 0-11, where the number (called x here) is divisble by 2. Note that this list would include the number 0 since it is in the range from 0-11 and has a remainder of 0 when divided by 2.

See also [documention on list comprehensions from python.org](https://docs.python.org/3/tutorial/datastructures.html#list-comprehensions).

## Local Scope (in Python)
The scope of a function where a local variable can be created and used without conflicting with higher-order, global variables. A global variable can be read within a local scope, but a local variable cannot be read at global scope.

## Local Variable (in Python)
A variable created in the local scope of a function. The variable name is erased after the function executes and is not accessible in the larger global scope of the program. A global variable can be read within a local scope, but a local variable cannot be read at global scope.

## Machine Learning
A subset of artificial intelligence that focuses on a machine algorithms that improve accuracy when exposed to additional data without being explicitly reprogrammed by a human.

## Markdown Cell (in a Jupyter Notebook)

A cell in a Jupyter notebook that contains explanatory information such as text, images, and links.

See also Code Cell (in a Jupyter Notebook), which can contain executable code. 

## Metadata
Data that describes data. In the humanities and library contexts, this often refers to bibliographic metadata that describes information such as author, publication date, medium, etc. It may also describe other kinds of data like files, for example "date created" or "file size."

## Method (in Python)
Like a function, a method executes a set of pre-written code but on a particular object like a list. 

## Module (in Python)
A set of functions that can be imported for use in a Python program. Modules can be gathered into even larger groups, such as a package or library.

## Modulo (in Python)
Notated as "%", an arithmetic operation that gives the remainder of a division. 34 % 6 = 4

## N-gram
A sequence of n items from a given sample of text or speech. Most often, this refers to a sequence of words, but it can also be used to analyze text at the level of syllables, letters, or phonemes. N-grams are often described by their length. For example, word n-grams might include:
* stock (a 1-gram, or unigram)
* chicken stock (a 2-gram, or bigram)
* homemade chicken stock (a 3-gram, or trigram)
A text analysis approach that looks only at unigrams at the word level will not be able to differentiate between the "stock" in "stock market" and "chicken stock."

One of the most popular examples of text analysis with n-grams is the [Google N-Gram Viewer](https://books.google.com/ngrams).

## Named Entity Recognition (NER)
A text analysis technique that seeks to identify and extract entities from a document. Entities could include things like:

* Person
* Organization
* Date
* Time
* Location

The Natural Language Toolkit, a suite of libraries in Python, can be used for Named Entity Recognition.

## Natural Language Processing (NLP)
The study of how computers can understand and manipulate natural human language whether in spoken or written forms. This includes areas such as:

* Text Analysis
* Natural Language Generation
* Speech recognition
* Transcription
* Translation

Natural Language Processing is a subfield that connects linguistics, computer science, information engineering, digital humanities, and data science.

## Natural Language Toolkit (NLTK)
A suite of libraries and programs for Natural Language Processing written in python. NLTK includes libraries for tokening, collocation, n-grams, Part of Speech (POS) Tagging, and Named Entity Recognition (NER).

See the [project documentation](https://www.nltk.org/) and book [Natural Language Processing with Python](http://www.nltk.org/book/).

## Neural Network (in Artificial Intelligence)
In artificial intelligence (as opposed to biology), a neural network refers to a simplified model of brain neurons that enables machines to complete tasks through methods such as machine learning. Neural networks are commonly used on problems that involve data classification (Who is in this image?) and prediction (What price should this house sell for?). 

## Non-consumptive Research
Non-consumptive research allows analysts to do text analysis without displaying or reading substantial portions of copyrighted materials. In practice, this usually means giving analysts a bag of words that describes the frequency of every word in a text but not the order in which they occur. 

<a id="operator"></a>
## Operator (in Python)

Changes a value through operations such as addition, multiplication, and concatenation.

|Operator| Operation| Example | Evaluation |
|---|----|---|---|
|\*\*| Exponent/Power| 3 ** 3 | 27 |
|%| Modulus/Remainder| 34 % 6 | 4 |
|/| Division | 30 / 6 | 5|
|\*| Multiplication | 7 * 8 | 56 |
|-| Subtraction | 18 - 4| 14|
|+| Addition | 4 + 3 | 7 |

## Optical Character Recognition (OCR)
The process of turning printed text into machine-readable digital text. Physical materials are scanned into digital images then specialized software attempts to turn the image into text. Two popular examples of OCR software are [Tesseract (Open Source)](https://github.com/tesseract-ocr/tesseract) and [ABBYY Finereader (Proprietary)](https://www.abbyy.com/en-us/finereader/).

## Package (in Python)
A group of modules that contain functions that can be imported and used within a Python program. Packages can be gathered into a larger group called a library.

## Pandas (in Python)
A library for visualizing, analyzing, and manipulating data in Python. Learn more about [Pandas at pydata.org](https://pandas.pydata.org/pandas-docs/version/0.15/tutorials.html).

## Parameter (in Python)
A variable in a function definition statement. The actual value or variable passed during execution is called an argument.

## Part of Speech (POS) Tagging
The act of marking the grammatical part of speech (such as nouns, verbs, and adjectives) for each word in a document. The linguistic models for POS tagging can be very complex, often using over 100 separate parts of speech. 

POS Tagging can be accomplished using the Natural Language Toolkit in Python.

## Plain text
A file that only contains text and can be easily read in a text editor (as opposed to a binary or executable file)

## Project Jupyter
A non-profit that develops open-source software, open standards, and services across many programming languages. They are most well-known for software such as The Jupyter Notebook, JupyterLab, and JupyterHub. All three of these programs are used to create, edit, and share programming notebooks, known as Jupyter notebooks.

## Python (Programming Language)
A highly-flexible, easy-to-learn programming language that is widely-used in the digital humanities and data science.

## R (Programming Language)
A programming language that is widely-used for statistical analysis and data mining, commonly in the areas of digital humanities and data science.

## Repository (for git, GitHub, GitLab, etc)
Also known as a "repo". A repository is a place to store all the versions of the code for a computer programming project.

See also git.

## Sentiment Analysis
A text analysis method that attempts to discover the emotions expressed in a sample of writing. Depending on the complexity of the method, it may discover simple distinctions (positive vs. negative) or more nuanced concepts (gratitude, anger, sadness, frustation, etc.).

## Slice (in Python)
A subset of items created from a list using index numbers.

> example_list[2:4]

The slice above creates a new list from `example_list` that contains the items at index 2 and 3 (but not 4).

## Stemming
Stemming is a method in text processing that eliminates prefixes and suffixes from words, transforming them into their fundamental or root form. For example, "chocolates", after stemming, will be turned into "chocolate". Many natural language processing packages provide stemmers to do automated stemming. For example, NLTK has a stemmer -- the Porter Stemmer -- which stems "immigrant", "immigrants" and "immigrantion" into "immigr". 

## Stop Words (List)
A stop words list is a set of words or phrases that are ignored in word frequency analysis. It is common for a researcher who is interested in prominent nouns and verbs to remove function words (e.g. the, and, I, to, of, a). A stop word list may also include other common words, such as character ids which are usually the most common words in a play text.

## String (in Python)
A string is a data type that contains a set of characters that can assigned to a variable as a value. (Other kinds of data types in Python include integers and floating point numbers.) 

|  Data type             | Examples                                      |
| -----------------------|:---------------------------------------------:|
| Integers               | -5, -3, 0, 5, 201                             |
| Floating-point numbers | -3.74, -3.14, 0.0, 503.4, 506                 | 
| Strings                | 'potatoes', 'Hello world!, 'no', '24 pizzas'  |  

## Tag Cloud (or Word Cloud)
A tag cloud is a visualization of the relative word frequencies in a corpus. The relative size of each word in a tag cloud depends on its frequency within a text. Larger words occur more frequently.

![Word Cloud of the content of journal African American Review](../All-sample-files/wordcloud.jpeg)

**A Tag Cloud of the journal *African American Review* (and its precursors *Black American Literature Forum* and *Negro American Literature Forum*).** 

## TEI XML
A form of XML Markup, or tagging, created by the [Text Encoding Initiative](https://tei-c.org/) to describe digital documents. This markup can help computers recognize particular aspects of the text. Text analysis often requires explicit marking, even for textual aspects that a human reader can easily pick out:
* Title
* Author Name
* Name of the speaker in a play
* A paragraph
* The speaker in a play
* Stage directions
* A stanza

See also Parts of Speech Tagging, Lemmatization, Tokenization.

## Term Frequency-Inverse Document Frequency (TFIDF)
A statistical method that intends to reflect how important a particular word is within a corpus. A simple measurement of "term frequency" is divided by inverse document frequency, limiting the weight of common words like "the", "of", and "to".

## Token
A chunk or string of text, most often a single word. The process of separating tokens in a document is called "tokenization."

## Topic Modeling (or Topic Analysis)

A machine learning text analysis method that attempts to discover a group of words that cluster together in a set of documents. One of the most common algorithms for topic modeling is Latent Dirichlet Allocation (LDA). 

## Trigram
An n-gram with a length of three. For example, "homemade chicken stock" is a word trigram.

## TSV (file)
A .tsv file, or Tab-Separated Value file, is a simple format for storing structured data where each entry in the file is separated by a tab. Similarly, a CSV file uses commas to separate individual data entries.

## Tuple (in Python)
A data type similar to a Python list, except that tuples are:

1. Notated with parentheses
>list = [1, 'monkey', 33.3234]
>tuple = (1, 'monkey', 33.3234)

2. Immutable. Like a string, the elements of a tuple cannot be changed. 

## Unigram
An n-gram with a length of one. For example, "chicken" is a unigram.

## Variable (in Python)
A named object that stores a value in Python, such as an integer, float, or string. 

Variables are created with an assignment statement.

## Voyant
A flexible, web-based platform for text analysis that can also be run locally. [Voyant](https://voyant-tools.org/) has many kinds of visualizations, supports saving, and creates embeddable html objects. To learn more, see [the documentation](https://voyant-tools.org/docs/#!/guide/start). 

## Word2vec
An algorithm that uses a neural network to create word embeddings.

## Word Cloud
See Tag Cloud.

## Word Co-Occurrence Matrix
A matrix that describes how often words co-occur. Co-occurrence usually means the words occur within the same sentence, but it could also mean within a set distance (such as within 3 words.)

## Word Embedding
A collective name for Natural Language Processing techniques that map words to vectors of real numbers using neural networks and dimensionality reduction on a word co-occurence matrix. Word2vec is a common model for producing word embeddings. 

## Word Frequency
A text analysis method that counts the number of occurences of individual words within a particular text. Word frequency uses a bag of words model where the order of words is not significant. Just as the letters of a Scrabble game are tossed into a bag without order, word frequency merely records the number of occurences with no regard to where a particular word occurs within a document. 

An alternative to this approach is using n-grams which can capture phrases in addition to individual words.

## XML
Short for (eXtensible markup language), XML uses tags to identify parts of a document for a machine to understand. Like HTML, these tags have an opening tag (e.g. <l>) and a closing tag marked by a forward slash (e.g. </l>). Unlike HTML, these tags can be freely created according to whatever standard the creator needs. One prominent example is the [Text Encoding Initiative](https://tei-c.org/). The example below uses TEI-XML to describe Shakespeare's Sonnet 130 by labeling lines, quatrains, and the final couplet. This kind of markup enables computers to do complex analysis quickly such as comparing every couplet, quatrain, or line in Shakespeare's sonnets.
```
<text>
 <body>
  <lg>
   <lg type="quatrain">
    <l>My Mistres eyes are nothing like the Sunne,</l>
    <l>Currall is farre more red, then her lips red</l>
    <l>If snow be white, why then her brests are dun:</l>
    <l>If haires be wiers, black wiers grown on her head:</l>
   </lg>
   <lg type="quatrain">
    <l>I have seene Roses damaskt, red and white,</l>
    <l>But no such Roses see I in her cheekes,</l>
    <l>And in some perfumes is there more delight,</l>
    <l>Then in the breath that from my Mistres reekes.</l>
   </lg>
   <lg type="quatrain">
    <l>I love to heare her speake, yet well I know,</l>
    <l>That Musicke hath a farre more pleasing sound:</l>
    <l>I graunt I never saw a goddesse goe,</l>
    <l>My Mistres when shee walkes treads on the ground.</l>
   </lg>
  </lg>
  <lg type="couplet">
   <l>And yet by heaven I think my love as rare,</l>
   <l>As any she beli'd with false compare.</l>
  </lg>
 </body>
</text>
```
