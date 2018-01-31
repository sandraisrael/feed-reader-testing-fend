# Project Overview

For this project I was given a web-based application that reads RSS feeds. The original developer of this application saw the value in testing, and started writing their first test suite! Unfortunately, they decided to move on to start their own company and left an application with an incomplete test suite which I was tasked to complete. I used [Jasmine](http://jasmine.github.io) to write a number of tests.

## How to Open app

You can view the [completed project here](https://sandraisrael.github.io/feed-reader-testing-fend/) 

**OR**

### Run the app on your local machine
1. Download/clone this repository and open in your favorite code editor 
2. Run `node -v`on the terminal or command line. If nothing shows up or you get an error, [Install Node](https://nodejs.org/en/)
3. Run `npm install -g http-server`
4. Then run `http-server -o` in the project directory


## How I completed this project
I was tasked to write the following tests in different test suites. Some tests required asynchronous function so I used callbacks - the `done()` argument within call to `beforeEach()`
1. A test that loops through each feed in the `allFeeds` object and ensures it has a URL defined and that the URL is not empty.
2. A test that loops through each feed in the `allFeeds` object and ensures it has a name defined and that the name is not empty.
3. A test that ensures the menu element is hidden by default under "The Menu" test suite.
4. Test that ensures the menu changes visibility when the menu icon is clicked.
5. A test that ensures when the `loadFeed` function is called and completes its work, there is at least a single `.entry` element within the `.feed` container.
6. A test that ensures when a new feed is loaded by the `loadFeed` function that the content actually changes
