# Comparing `tmp/arxiv-astro-summarizer-1.1.tar.gz` & `tmp/arxiv-astro-summarizer-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arxiv-astro-summarizer-1.1.tar", last modified: Fri May 19 19:05:38 2023, max compression
+gzip compressed data, was "arxiv-astro-summarizer-1.2.tar", last modified: Mon May 22 00:36:35 2023, max compression
```

## Comparing `arxiv-astro-summarizer-1.1.tar` & `arxiv-astro-summarizer-1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-19 19:05:38.108250 arxiv-astro-summarizer-1.1/
--rwxr-xr-x   0 daniel     (501) staff       (20)    35141 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-1.1/LICENSE.txt
--rw-r--r--   0 daniel     (501) staff       (20)        0 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-1.1/MANIFEST.in
--rw-r--r--   0 daniel     (501) staff       (20)      663 2023-05-19 19:05:38.107942 arxiv-astro-summarizer-1.1/PKG-INFO
--rwxr-xr-x   0 daniel     (501) staff       (20)     1029 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-1.1/README.md
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-19 19:05:38.103844 arxiv-astro-summarizer-1.1/arxiv_astro_summarizer/
--rwxr-xr-x   0 daniel     (501) staff       (20)       26 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-1.1/arxiv_astro_summarizer/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)    20092 2023-05-19 18:47:06.000000 arxiv-astro-summarizer-1.1/arxiv_astro_summarizer/astroph_summarizer.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-19 19:05:38.107542 arxiv-astro-summarizer-1.1/arxiv_astro_summarizer.egg-info/
--rw-r--r--   0 daniel     (501) staff       (20)      663 2023-05-19 19:05:38.000000 arxiv-astro-summarizer-1.1/arxiv_astro_summarizer.egg-info/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)      366 2023-05-19 19:05:38.000000 arxiv-astro-summarizer-1.1/arxiv_astro_summarizer.egg-info/SOURCES.txt
--rw-r--r--   0 daniel     (501) staff       (20)        1 2023-05-19 19:05:38.000000 arxiv-astro-summarizer-1.1/arxiv_astro_summarizer.egg-info/dependency_links.txt
--rw-r--r--   0 daniel     (501) staff       (20)      119 2023-05-19 19:05:38.000000 arxiv-astro-summarizer-1.1/arxiv_astro_summarizer.egg-info/requires.txt
--rw-r--r--   0 daniel     (501) staff       (20)       23 2023-05-19 19:05:38.000000 arxiv-astro-summarizer-1.1/arxiv_astro_summarizer.egg-info/top_level.txt
--rw-r--r--   0 daniel     (501) staff       (20)      337 2023-05-19 17:17:05.000000 arxiv-astro-summarizer-1.1/pyproject.toml
--rw-r--r--   0 daniel     (501) staff       (20)       38 2023-05-19 19:05:38.108344 arxiv-astro-summarizer-1.1/setup.cfg
--rwxr-xr-x   0 daniel     (501) staff       (20)     1100 2023-05-19 17:17:26.000000 arxiv-astro-summarizer-1.1/setup.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 00:36:35.354260 arxiv-astro-summarizer-1.2/
+-rwxr-xr-x   0 daniel     (501) staff       (20)    35141 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-1.2/LICENSE.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        0 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-1.2/MANIFEST.in
+-rw-r--r--   0 daniel     (501) staff       (20)      663 2023-05-22 00:36:35.353994 arxiv-astro-summarizer-1.2/PKG-INFO
+-rwxr-xr-x   0 daniel     (501) staff       (20)     1029 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-1.2/README.md
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 00:36:35.351372 arxiv-astro-summarizer-1.2/arxiv_astro_summarizer/
+-rwxr-xr-x   0 daniel     (501) staff       (20)       26 2023-05-18 22:04:20.000000 arxiv-astro-summarizer-1.2/arxiv_astro_summarizer/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)    22758 2023-05-22 00:15:13.000000 arxiv-astro-summarizer-1.2/arxiv_astro_summarizer/astroph_summarizer.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 00:36:35.353543 arxiv-astro-summarizer-1.2/arxiv_astro_summarizer.egg-info/
+-rw-r--r--   0 daniel     (501) staff       (20)      663 2023-05-22 00:36:35.000000 arxiv-astro-summarizer-1.2/arxiv_astro_summarizer.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)      366 2023-05-22 00:36:35.000000 arxiv-astro-summarizer-1.2/arxiv_astro_summarizer.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2023-05-22 00:36:35.000000 arxiv-astro-summarizer-1.2/arxiv_astro_summarizer.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (501) staff       (20)      119 2023-05-22 00:36:35.000000 arxiv-astro-summarizer-1.2/arxiv_astro_summarizer.egg-info/requires.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       23 2023-05-22 00:36:35.000000 arxiv-astro-summarizer-1.2/arxiv_astro_summarizer.egg-info/top_level.txt
+-rw-r--r--   0 daniel     (501) staff       (20)      337 2023-05-19 17:17:05.000000 arxiv-astro-summarizer-1.2/pyproject.toml
+-rw-r--r--   0 daniel     (501) staff       (20)       38 2023-05-22 00:36:35.354349 arxiv-astro-summarizer-1.2/setup.cfg
+-rwxr-xr-x   0 daniel     (501) staff       (20)     1099 2023-05-21 23:23:58.000000 arxiv-astro-summarizer-1.2/setup.py
```

### Comparing `arxiv-astro-summarizer-1.1/LICENSE.txt` & `arxiv-astro-summarizer-1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arxiv-astro-summarizer-1.1/PKG-INFO` & `arxiv-astro-summarizer-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxiv-astro-summarizer
-Version: 1.1
+Version: 1.2
 Summary: Scrapes arXiv astro-ph paper, summarizes the abstract, and returns relavant papers according to a user input.
 Home-page: https://github.com/Professor-G/arxiv-astro-summarizer
 Author: Daniel Godines
 Author-email: danielgodinez123@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `arxiv-astro-summarizer-1.1/README.md` & `arxiv-astro-summarizer-1.2/README.md`

 * *Files identical despite different names*

### Comparing `arxiv-astro-summarizer-1.1/arxiv_astro_summarizer/astroph_summarizer.py` & `arxiv-astro-summarizer-1.2/arxiv_astro_summarizer/astroph_summarizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from progress import bar
 
 import arxivscraper
 import numpy as np 
 import pandas as pd
 from pathlib import Path
 from PyPDF2 import PdfReader
-from datetime import datetime
+from datetime import datetime, timedelta
 from sklearn.feature_extraction.text import TfidfVectorizer
 from sklearn.metrics.pairwise import cosine_similarity
 from transformers import pipeline
 logging.getLogger("transformers").setLevel(logging.ERROR)
 import os; os.environ['TOKENIZERS_PARALLELISM'] = 'false'
 from textract.exceptions import MissingFileError
 
@@ -37,42 +37,26 @@
 from nltk.stem import WordNetLemmatizer
 
 class Scraper:
     """
     Class object to scrape, read, and analyze arXiv papers published on a given date.
 
     Args:
-        date (str): The initial date to consider for scraping, in the following format: YYYY-MM-DD, e.g. '2022-05-12'.
+        date (str): The date to consider for scraping, in the following format: YYYY-MM-DD, e.g. '2022-05-12'.
         user_input (str, optional): A short excerpt describing the kind of papers the user is interested in. Defaults to None.
         path (str, optional): The path where the file should be saved. Defaults to None, which saves the files to the local home directory.
 
     Attributes:
         df (pandas.DataFrame): DataFrame containing the metadata of the scraped arXiv papers.
         text (str): Processed abstract text extracted from a PDF file.
         raw_text (str): Raw abstract text extracted from a PDF file.
         filenames (list): List of saved file names.
 
     Raises:
         ValueError: If the input date is not a string or if user_input is not a string when provided.
-
-    Examples:
-        Initialize the Scraper object with a date and user input:
-        >>> scraper = Scraper('2022-05-12', user_input='black hole')
-
-        Scrape arXiv papers for the given date:
-        >>> scraper.scrape_arxiv()
-
-        Save a specific paper using its index in the scraped metadata, or set to 'all' to save all papers:
-        >>> scraper.save_paper(0)
-
-        Summarize the saved papers and score the relevance between the summary and the user_input:
-        >>> scraper.summarize()
-
-        Remove papers with similarity scores less than or equal to the specified similarity_threshold (defaults to 0)
-        >>> scraper.remove_irrelevant_papers(similarity_threshold=0)
     """
 
     def __init__(self, date, user_input=None, path=None):
         self.date = date
         self.user_input = user_input
         self.path = path
         
@@ -93,14 +77,17 @@
         print(f"Files will be saved in: {self.path}")
 
     def format_date(self):
         """
         Converts a date string from 'YYYY-MM-DD' format to 'DD Month YYYY' format.
         This will be used to keyword search the paper, to ensure that the publication 
         times are consistent with the input date.
+        
+        Args:
+            None 
 
         Returns:
             str: The date string in 'DD Month YYYY' format.
         """
         
         formatted_date = datetime.strptime(self.date, '%Y-%m-%d')
         formatted_date = formatted_date.strftime('%d %B %Y')
@@ -190,27 +177,33 @@
 
         return full_path
 
     def scrape_arxiv(self):
         """
         Compiles the metadata of the arxiv papers uploaded on a given day. Scraping
         date ranges is not currently supported!
+
+        Args:
+            None
     
         Returns:
             Pandas dataframe with the following meta-data: 'id', 'title', 'categories', 'abstract', 'doi', 'created', 'updated', 'authors'
         """
         
         if not isinstance(self.date, str):
             raise ValueError('date should be a string in the format YYYY-MM-DD')
 
         scraper = arxivscraper.Scraper(category='physics:astro-ph', date_from=self.date, date_until=self.date)
         output = scraper.scrape()
-        
-        self.df = pd.DataFrame(output, columns=('id', 'title', 'categories', 'abstract', 'doi', 'created', 'updated', 'authors'))
-        
+
+        try:
+            self.df = pd.DataFrame(output, columns=('id', 'title', 'categories', 'abstract', 'doi', 'created', 'updated', 'authors'))
+        except ValueError:
+            print('No papers available on this date.')
+
         return
 
     def save_paper(self, index):
         """
         Function to download and save a pdf given the DOI number. The file 
         is saved to the specified directory, or the local home directory if path is not provided.
         
@@ -472,32 +465,107 @@
         return similarity
 
     def remove_irrelevant_papers(self, similarity_threshold=0):
         """
         Removes the papers that have similarity scores less than or equal to the specified similarity_threshold.
 
         Args:
-            similarity_threshold
+            similarity_threshold (float): Papers with similarity scores below this threshold will be deleted.
+                Defaults to 0. Can be set to None to keep all papers.
+        
+        Returns:
+            None
         """
 
+        if similarity_threshold is None:
+            return 
+
         if self.df is None:
             raise ValueError('The df attribute does not yet exist, run the summarize() class method first!')
 
+        if len(np.where(self.df.Similarity > similarity_threshold)[0]) == 0:
+            print('NOTE: No papers with similarity scores above the similarity_threshold were detected! Removing all...')
+
         indices = np.where(self.df.Similarity <= similarity_threshold)[0]
 
         for index in indices:
             try:
                 os.remove(self.path+self.df.Author.iloc[index])
             except FileNotFoundError:
                 pass 
-                
+        
         print(f"Complete! The following directory now contains only relevant papers: {self.path}")
 
         return 
 
+def scrape_and_analyze(start_date_str, end_date_str, user_input=None, similarity_threshold=None, path=None):
+    """
+    Scrape and process astrophysics papers from arXiv for a range of dates (Monday to Friday only!).
+    
+    Example:
+        >>> start_date_str = '2023-04-01'
+        >>> end_date_str = '2023-04-30'
+        >>> scrape_and_analyze(start_date_str, end_date_str)
+
+    Args:
+        start_date_str (str): The start date in the format 'YYYY-MM-DD'.
+        end_date_str (str): The end date in the format 'YYYY-MM-DD'.
+        user_input (str, optional): A short excerpt describing the kind of papers the user is interested in. Defaults to None.
+        similarity_threshold (float): Papers with similarity scores below this threshold will be deleted.
+            Defaults to 0. Can be set to None to keep all papers.
+        path (str, optional): The path where the file should be saved. Defaults to None, which saves the files to the local home directory.
+
+    Returns:
+        None
+    """
+
+    # Convert the input date strings to datetime objects
+    start_date = datetime.strptime(start_date_str, '%Y-%m-%d').date()
+    end_date = datetime.strptime(end_date_str, '%Y-%m-%d').date()
+
+    # Check if the start date is after the end date
+    if start_date > end_date:
+        print("Invalid date range. The start date should be before or equal to the end date.")
+        return
+
+    # Iterate over each date in the range
+    current_date = start_date
+    while current_date <= end_date:
+        #if current_date.weekday() < 5: # Check if the current date is a weekday (Monday to Friday)
+        
+        # Convert the current date to the desired format ('YYYY-MM-DD')
+        formatted_date = current_date.strftime('%Y-%m-%d')
+        print(f"Processing date: {formatted_date}")
+
+        # Create the class object for the current date
+        scraper = Scraper(date=formatted_date, user_input=user_input, path=path)
+
+        # Scrape papers from the input date
+        scraper.scrape_arxiv()
+
+        if scraper.df is not None: #None if no papers were scraped on that date
+            # Save all papers that were scraped
+            scraper.save_paper(index='all')
+
+            # Summarize the abstract of all papers and save the similarity score
+            if len(scraper.filenames) > 0:
+                
+                # Summarize the scraped files
+                scraper.summarize()
+
+                # Remove the papers with similarity scores less than some threshold
+                scraper.remove_irrelevant_papers(similarity_threshold=similarity_threshold)
+            else:
+                print(f"No papers found on this date: {formatted_date}")
+
+        # Move to the next day
+        current_date += timedelta(days=1)
+
+    return
+
 def replace_astronomical_terms(text):
     """
     Replaces astronomical terms and abbreviations with their expanded forms or corresponding concepts.
 
     Args:
         text (str): The preprocessed text.
```

### Comparing `arxiv-astro-summarizer-1.1/arxiv_astro_summarizer.egg-info/PKG-INFO` & `arxiv-astro-summarizer-1.2/arxiv_astro_summarizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxiv-astro-summarizer
-Version: 1.1
+Version: 1.2
 Summary: Scrapes arXiv astro-ph paper, summarizes the abstract, and returns relavant papers according to a user input.
 Home-page: https://github.com/Professor-G/arxiv-astro-summarizer
 Author: Daniel Godines
 Author-email: danielgodinez123@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `arxiv-astro-summarizer-1.1/setup.py` & `arxiv-astro-summarizer-1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 @author: danielgodinez
 """
 from setuptools import setup, find_packages, Extension
 
 
 setup(
     name="arxiv-astro-summarizer",
-    version="1.01",
+    version="1.2",
     author="Daniel Godines",
     author_email="danielgodinez123@gmail.com",
     description="Scrapes arXiv astro-ph paper, summarizes the abstract, and returns relavant papers according to a user input.",
     license='GPL-3.0',
     url = "https://github.com/Professor-G/arxiv-astro-summarizer",
     classifiers=[
 		'Development Status :: 5 - Production/Stable',
```

