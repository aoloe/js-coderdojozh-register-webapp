# CoderDojo Zurich, Registration Webapp

Ask the the people who registered to a Coderdojo, how many kids they will bring for each topic.

- `GET: /event/{id}/rvsps`: list of all participant having registred through Meetup.
- `GET: event/{id}`: information about the event.
- `POST: /event/{eventId}/participant/{userId}`: number of kids for each offer.

You can see the more details about the API in our [PHP sample API](https://github.com/aoloe/php-coderdojozh-registration-api).

## Install

You can upload the files in this repository to your server, change  the value of `apiUrl` to point to your API and browse to `http://your-url.com/?id=the-event-id`.
