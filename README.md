# HW1_Web_Measurements

Target Business Page for Q2 and Q3:
https://www.yelp.com/biz/sushi-and-k-grill-fenton

## Tool Versions
- OS: Mac Sequoia 15.7.1
- Curl: curl 8.1.1
- Browser: Google Chrome
- Web Scraper Chrome Extension

## Question Answers
All predictions, commands, and the request manifest are contained in the google doc, **Question_Answers_CSCI_4360_HW1_Kee**, nearly all of my answers that could be typed out are contained in this document, so always refer back to it.

These were the full hashes for the four requests:
- Baseline: ca02c2092c1cb31438e9b8018ca00dac21b0ac5249f0d27197fa55d0b2d73edd
- Browser-Like User-Agent: 0de30432ac562e6eafcc3c0981169765e462f16bae40f79733c30a5dcbfcacde
- Different Accept-Language: 62b385569dcaa5302348af552b8f815b1f03e1110d61c017e1143ae490a08219
- Cookie Reuse: 7376bda716aeace3c3cdb9df06520f9581b0109fd6638404df50f21228048ba9

## Q2 Reproduction Instructions
1. Open a terminal on macOS.
2. Navigate to the file containing the experiment answers.
3. Run the four curl commands shown in Question 2.
4. After each request, record the timestamp, byte count, SHA-256 hash, HTTP status code, and content type.

## Q3 Reproduction Instructions
1. Open Google Chrome and navigate to: https://www.yelp.com/biz/sushi-and-k-grill-fenton
2. Open Chrome Developer Tools.
3. Select the Web Scraper tab.
4. Import the provided sitemap configuration file: yelp-sushi-sitemap.json
5. Open the sitemap and verify that the main repeated selector is review.
6. Confirm that the main repeated selector is "review", and that the following child selectors are present.
   - reviewer
   - rating
   - date
   - review_text
7. Confirm that business_name is also included as a page-level field.
8. Run the scraper and export the results as CSV.
9. Verify that each exported record contains:
   - reviewer pseudonym
   - rating
   - review date
   - review text
   - business name



