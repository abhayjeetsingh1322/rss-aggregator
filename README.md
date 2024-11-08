# RSS Aggregator

## Description
This project builds on the RSS Reader to process multiple RSS feeds from an input XML file. It generates:
1. Individual HTML pages for each RSS feed with tables of links to news items.
2. An HTML index page that links to all the feed pages.

## Objectives
- Refactor and reuse existing RSS Reader functionality.
- Handle multiple data sources using XML processing with `XMLTree`.
- Generate dynamic HTML pages programmatically.

## Features
1. **Input**:
   - XML file specifying feed URLs, names, and output file names.
   - Example input:
     ```xml
     <feeds title="News Aggregator">
       <feed url="https://example.com/rss1.xml" name="Example Feed 1" file="feed1.html" />
       <feed url="https://example.com/rss2.xml" name="Example Feed 2" file="feed2.html" />
     </feeds>
     ```

2. **Output**:
   - HTML index page:
     - Includes a title and a list of links to individual feed pages.
   - Individual feed pages:
     - Tables of links to news items, similar to the RSS Reader project.

3. **Refactored Functionality**:
   - Extracts feed processing into a reusable method `processFeed`.

## Technologies Used
- Java
- `XMLTree` library for XML processing
- RSS 2.0 specification

## How to Run
1. Clone the repository:
   ```bash
   git clone [repository URL]
