[*pypi*](https://pypi.org/project/dorkify)

# dorkify
dorkify is a Python library for searching Google, easily. dorkify uses requests and BeautifulSoup4 to scrape Google. 

## Installation
To install, run the following command:
```bash
python3 -m pip install dorkify
```

## usage
To get results for a search term, simply use the search function in dorkify. For example, to get results for "Google" in Google, just run the following program:
```python
from dorkify import search
search("Google")
```

## Additional options
dorkify supports a few additional options. By default, dorkify returns 10 results. This can be changed. To get a 100 results on Google for example, run the following program.
```python
from dorkify import search
search("exploit-db", num_results=100)
```
In addition, you can change the language google searches in. For example, to get results in French run the following program:
```python
from dorkify import search
search("exploit-db", lang="en")
```
## dorkify.search
```python
dorkify.search(str: term, int: num_results=10, str: lang="en") -> list
```
## In the new version of dorkify you can search on a specified site:

```python
from dorkify import search

search("site:exploit-db.com "gmail"")
