# Weather service

## Problem definition
 -  We need to implement a new weather service. That service will face several API consumers who will request weather temperature information.

## Requirements
 - The API client provides the city and receives the temperature
 - Example: When we provide Sofia we expect to receive 4
 - Additionally, the weather temperature should contain a sign indicating the temperature trend. The trend should be calculated as the deviation between the temperature and the average of the last 10 days (calculation should be simple, avoid usage of statistics formulas).
 - - A negative, positive or static sign is then added as a suffix to the temperature value
 - - Example 4 :hot_face: or 4 :cold_face: or 4 -

## Must haves
 - Code in PHP
 - You're free to choose any storage mechanism you wish. We expect to be able to run the application locally by using docker compose, with no local dependencies required.
 - Full test coverage

## Bonus points
 - Using of Symfony framework
 - Imagine that you call a third-party API to get the weather every hour. Client A calls you for the following city Sofia, and 10 seconds later Client B calls you for the same city.
 - Can you minimise the networking calls to the third party for repeated city, within the 1-hour window?
 - UI
