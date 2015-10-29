Automating Your Browser and Desktop Apps (w/ Python)
@AISweigart
InventWithPython.com
bit.ly/automatetalk

10am    - Intro from O'Reilly Rep (about the speaker/webcast stuff)
10:02   - Intro from Al
        - Discussed book structure / why programming is his interest / stuff related to Creative Commons
10:04   - Web Scraping
        - Selenium
        -   - automated way of testing your browser
        -   - just install selenium w/ pip
        
            from selenium import webdriver
            browser = webdriver.Firefox()
            browser.get('http://automatetheboringstuff.com')
            elem = browser.find_element_by_css_selector('.entry-content > ol:nth-child(15) > li:nth-child(1) > a:nth-child(1)')
            elem.click()
            browser.quit()

10:12   - live demo of the code above.
        - to find the css selector:
            - find a link and right click and 'inspect element' (in firefox)
            - then right click on the item and 'copy unique selector' (in firefox)

10:21   - there is also an find_elements_by_css_selector() method <-- note the plurality of elements

10:23   - referencing Zen of Python = 'Flat is better than nested'
        - Try to keep things simple with regards to opening tabs and nesting requests

10:28   - Some discussion about obtaining html data
 
10:32   - PyAutoGui
        - live demo -- simple interface to move x/y related position and clicking, etc.
        
10:45   - Warning:
        - be careful about allowing automation to just run without any failsafes.
        
10:50   - What is GUI automation used for? (Recap)

10:51   - last live demo -- playing a Flash game automated.

10:55   - Q/A
