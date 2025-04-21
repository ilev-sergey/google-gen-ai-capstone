# Playbill AI

This repository is a сapstone project within the [Google Generative AI intensive course](https://rsvp.withgoogle.com/events/google-generative-ai-intensive_2025q1/home).

# Use Case

Gen AI model (Gemini 2.0 flash) is used as a part of the service for aggregation of theater playbills.

## Problem

There are a lot of theaters in Moscow and tracking premieres in all of them is a unpleasant task. Despite there are aggregation services that collect this info, they are mostly uncomfortable for users as they don't have different filters, such as choosing location, specific play or stage director. Moreover, crawling through a variety of filters is also time-consuming and discouraging for users.

## Solution

The provided solution allows to transform arbitrary user input into an appropriate SQL-query and then return the response basing on the data in the database. Currently only text is supported, but it's possible to extend it to voice input as well.

## Example

E.g. user asks: "Plays for the coming month by Shakespeare, Williams or Chekhov" that is transformed into SQL-query that is passed into database. The result is "There are no plays by Shakespeare, Williams, or Chekhov in the coming month" because there aren't any performances by these authors in the local database. See more examples below. 


# Gen AI Capabilities

The project combines such AI capabilities as
- Structured output (SQL-query)
- Few-show prompting
- Function Calling
- Grounding (for showing reviews)

# Future

The developed solution will be used in conjunction with developing API for theatres (link will be provided later) as a part of aggregation service deployed both as a web-application and as telegram bot.
