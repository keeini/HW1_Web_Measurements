# HW1_Web_Measurements

Target Business Page for Q3:
https://www.yelp.com/biz/sushi-and-k-grill-fenton

## Tool Versions
OS: Mac Sequoia 15.7.1
Curl: curl 8.1.1
Browser: Google Chrome for Q3
Web Scraper Chrome Extension

# Question 2 Answers
All predictions, commands, and the request manifest are contained in the google doc, **CSCI_4360_HW1_Kee**, nearly all of my answers that could be typed out are contained in this document, so always refer back to it.

As a reference, I will provide the answers in this README as well.

Baseline
Command:
curl -L -D baseline-headers.txt \
-o baseline.html \
"https://www.yelp.com/biz/sushi-and-k-grill-fenton"
Timestamp: Tue Sep 22 12:49:37 CDT 2026
Final URL: https://www.yelp.com/biz/sushi-and-k-grill-fenton
Status code: 403 Forbidden
Content type: text/html; charset=UTF-8
Saved response body: baseline.html
Byte count: 776 bytes
SHA-256: ca02…3edd
Body classification: Block page, no review data was returned. The response asked the user to enable JS and disable any ad blocker and loaded a CAPTCHA script from captcha-delivery.com.

Browser-like User-Agent
Command: 
curl -L -D useragent-headers.txt \
-o useragent.html \
-A "Mozilla/5.0" \
"https://www.yelp.com/biz/sushi-and-k-grill-fenton"
Timestamp: Tue Sep 22 12:54:11 CDT 2026
Final URL: https://www.yelp.com/biz/sushi-and-k-grill-fenton
Status code: 403 Forbidden
Content type: text/html; charset=UTF-8
Saved response body: useragent.html
Byte count: 776 bytes
SHA-256: 0de3…acde
Body classification: Block page, no review data was returned. The response asked the user to enable JS and disable any ad blocker and loaded a CAPTCHA script from captcha-delivery.com.

Different Accept-Language
Command:
curl -L -D language-headers.txt \
-o language.html \
-H "Accept-Language: es-ES" \
"https://www.yelp.com/biz/sushi-and-k-grill-fenton"
Timestamp: Tue Sep 22 12:56:39 CDT 2026
Final URL: https://www.yelp.com/biz/sushi-and-k-grill-fenton
Status code: 403 Forbidden
Content type: text/html; charset=UTF-8
Saved response body: language.html
Byte count: 776 bytes
SHA-256: 62b3…8219
Body classification: Block page, no review data was returned. The response asked the user to enable JS and disable any ad blocker and loaded a CAPTCHA script from captcha-delivery.com.



Cookie Reuse
Command: 
curl -L -D cookies-headers.txt \
-o cookies.html \
-b cookies.txt \
"https://www.yelp.com/biz/sushi-and-k-grill-fenton"
Timestamp: Tue Sep 22 12:59:07 CDT 2026
Final URL: https://www.yelp.com/biz/sushi-and-k-grill-fenton
Status code: 403 Forbidden
Content type: text/html; charset=UTF-8
Saved response body: cookies.html
Byte count: 776 bytes
SHA-256: 7376…8ba9
Body classification: Block page, no review data was returned. The response asked the user to enable JS and disable any ad blocker and loaded a CAPTCHA script from captcha-delivery.com.
