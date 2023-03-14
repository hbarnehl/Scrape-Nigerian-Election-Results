# Scrape-Nigerian-Election-Results
These notebooks can be used to scrape Nigerian election results. While I only downloaded the results from the Lagos state, the notebooks can easily be adapted to download all results.

The election results are stored on the inec website in the following file structure: state:LGA:ward:polling unit.
Users should first use collect_ward_links to get all the links to individual wards of their preferred state. I used the notebooks for Lagos state, but the notebook can easily be adapted to loop through all states.
Next, scrape_images does the actual scraping of results images. Due to the nature of selenium, the display of the machine carrying out the task should remain on, otherwise selenium throws not clickable errors. The scraper will also open a log to help debugging.
Check_status_and_convert can be used to check the current status of the scraper, showing the number of images per LGA or ward.

Precaution:
I downloaded all files as jpgs because I thought they were all stored as images. In fact, some of them are stored as pdfs. I corrected this later with the last notebook.
