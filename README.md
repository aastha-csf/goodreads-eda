# Goodreads EDA

Exploratory data analysis and statistical investigation of Goodreads books, examining relationships between ratings, genres, metadata, and reader behavior.

## Status

🚧 In Progress

## Datasets

### Dataset Overview
This project uses two files from the **UCSD Goodreads Book Graph** dataset (collected in late 2017 by Mengting Wan and Julian McAuley):
* **`goodreads_books.json.gz`**: Detailed book metadata (titles, descriptions, ratings, page counts, publication details, and similar book IDs).
* **`goodreads_book_genres_initial.json.gz`**: Fuzzy genre distributions mapped to each book ID based on user shelf tags.

*Note: Per dataset redistribution guidelines, the raw `.json.gz` files are excluded from this repository. You can download them directly from the [UCSD Book Graph repository](https://cseweb.ucsd.edu/~jmcauley/datasets/goodreads.html).*

### **Goodreads Books Dataset (UCSD)**
#### Features of the dataset 
|Column | Type | Description |
|-------|------|-------------|
isbn | string | ISBN-10 identifier
text_reviews_count | string/integer | Number of written reviews |  
series | list | Series IDs the book belongs to |  
country_code | string | Country code (usually US) |  
language_code | string | Language of the book (e.g., eng) |  
popular_shelves | list of objects | Goodreads shelves and counts |  
asin | string | Amazon ASIN if available |  
is_ebook | string/boolean | Whether the book is an ebook |  
average_rating | string/float | Average Goodreads rating |  
kindle_asin | string | Kindle ASIN |  
similar_books | list | IDs of similar books |  
description | string | Book description/synopsis |  
format | string | Format (Paperback, Hardcover, Kindle, etc.) |  
link | string | Goodreads link |  
authors | list of objects | Author information |  
publisher | string | Publisher name |  
num_pages | string/integer | Number of pages |  
publication_day | string/integer | Day published |  
isbn13 | string | ISBN-13 identifier |  
publication_month | string/integer | Month published |  
edition_information | string | Edition details |  
publication_year | string/integer | Publication year |  
url | string | Goodreads URL |  
image_url | string | Cover image URL |  
book_id | string | Goodreads book ID |  
ratings_count | string/integer | Total ratings received |  
work_id | string | Goodreads work ID |  
title | string | Full title |  
title_without_series | string | Title excluding series information | 

### **Goodreads Genres Dataset (UCSD)**


## Research Questions

- Do more popular books receive better ratings?
- Are ebooks rated differently than physical books?
- Do books with descriptions get more ratings?
- Does series membership improve ratings?
- Most popular publishers
- Book recommendation graph using similar_books
- Language distribution of books
- Page count vs rating correlation
- How does rating variability relate to popularity?
- What patterns exist across genres?
- Additional questions to be added as the project evolves.

### Citations
If you use or build upon this dataset, please cite the original authors' papers as requested:

* Wan, M., & McAuley, J. (2018). Item Recommendation on Monotonic Behavior Chains. *Proceedings of the 12th ACM Conference on Recommender Systems (RecSys '18)*, 86–94.
* Wan, M., Misra, R., Nakashole, N., & McAuley, J. (2019). Fine-Grained Spoiler Detection from Large-Scale Review Corpora. *Proceedings of the 57th Annual Meeting of the Association for Computational Linguistics (ACL '19)*, 2605–2610.