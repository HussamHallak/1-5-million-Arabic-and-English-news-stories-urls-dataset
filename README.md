# 1.5-million-Arabic-and-English-news-stories'-URLs-dataset

This is a collection of Arabic and English news dataset collected from four different major Arabic and English news outlets that are geared towards Arabs, English speaking Arabs, Arabic speakers around the world, and English speakers who are interested in the Arabic narratives of world news (Aljazeera Arabic, Alarabiya, Aljazeera English, and Arab News). Such a collection can be used to conduct research on news similarity, machine translation (MT), Arabic Named Entity Recognition and Classification (NERC), and perform a systematic comparisons of different approaches.

We examined multiple ways to collect news stories from multiple news outlets in Arabic and English. After settling on  what we discovered to be the best method, we collected 1.5 million news stories from four different news outlets and examined link rot in each website. Furthermore, we developed a method to eliminate links that do not lead to a news story. 

I have written a script to use ultimate-sitemap-parser 0.5 to collect news stories' links from news websites. Using the library proved to be effective since it works on any news outlet website without customization.

After collecting all news stories from all sitemaps for all selected news outlets, the stories are grouped by date. Grouping stories by date allows researchers to limit their research to a subset of stories based on their published date if needed. This step is time consuming since all stories have to be downloaded. Also, the library is not 100% reliable since finding the published date of a story is not always possible.

While collecting the URLs to build this dataset, I verified that the story is still accessible from the live web which eliminates problems related to link rot.

Where to find the news stories' links in this dataset?
1. Location of stories' URLs grouped by date: Dataset/Links grouped by date/
2. Location of stories' URLs that did not return 200 or 404 when crawled. These URLs could be crawled at a later date (1010 URLs): Dataset/links not to stories or to be crawled at a later date/links_to_redo.txt
3. Location of URLs that did not return published date. They are mainly URLs to pages other than news stories: Dataset/links not to stories or to be crawled at a later date/None.txt
4. Location of he set of URLs collected from Aljazeera.com: Dataset/aljazeera_English_sitemap_links_set.txt
5. Location of he set of URLs collected from Aljazeera.net: Dataset/aljazeera_Arabic_sitemap_links_set.txt
6. Location of he set of URLs collected from Alarabiya.com: Dataset/alarabiya_sitemap_links_set.txt
7. Location of he set of URLs collected from arabnews.com: Dataset/arabnews_sitemap_links_set.txt

This dataset is presented and studeied in a <a href='https://ws-dl.blogspot.com/2023/08/2023-08-10-collecting-15-million.html'>blog post</a> on WS-DL research group blogs site.
