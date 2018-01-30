# Project Overview

For this project I was given a web-based application that reads RSS feeds. The original developer of this application saw the value in testing, and started writing their first test suite! Unfortunately, they decided to move on to start their own company and left an application with an incomplete test suite which I was tasked to complete.

I was able to use [Jasmine](http://jasmine.github.io) to write a number of tests against the pre-existing application. Which will test the underlying business logic of the application as well as the event handling and DOM manipulation.

#### View the completed project [here](https://sandraisrael.github.io/feed-reader-testing-fend/) 

Testing is an important part of the development process and many organizations practice a standard of development known as "test-driven development". This is when developers write tests first, before they ever start developing their application. All the tests initially fail and then they start writing application code to make these tests pass.

Whether you work in an organization that uses test-driven development or in an organization that uses tests to make sure future feature development doesn't break existing features, it's an important skill to have!

## How I completed this project
I was tasked to write the following tests in different test suites. Some tests required asynchronous function so I used callbacks - the `done()` argument within call to `beforeEach()`
1. A test that loops through each feed in the `allFeeds` object and ensures it has a URL defined and that the URL is not empty.
2. A test that loops through each feed in the `allFeeds` object and ensures it has a name defined and that the name is not empty.
3. A test that ensures the menu element is hidden by default under "The Menu" test suite.
4. Test that ensures the menu changes visibility when the menu icon is clicked.
5. A test that ensures when the `loadFeed` function is called and completes its work, there is at least a single `.entry` element within the `.feed` container.
6. A test that ensures when a new feed is loaded by the `loadFeed` function that the content actually changes
