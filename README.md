# CoderDojo Zurich, Registration Webapp

Ask the the people who registered to a Coderdojo, how many kids they will bring for each topic.

This services is tailored for CoderDojo using Meetup for registrations:

- The parent or the kids are registering.
- Only the kids participate.
- The mentors are also registering through Meetup.

This is a javascript application that queries an API providing a bridge to Meetup with the following services:

- `GET: /event/{id}/rvsps`: list of all participant having registred through Meetup.
- `GET: event/{id}`: information about the event.
- `POST: /event/{eventId}/participant/{userId}`: number of kids for each offer.

More details about the data exchanged [in our PHP API](https://github.com/aoloe/php-coderdojozh-registration-api).

## Install

You can upload the files in this repository to your server, change  the value of `apiUrl` to point to your API and browse to `http://your-url.com/?id=the-event-id`.

## Features

- Accept all the group's events by using the `id` parameter in the url.
- Automatically list the people who are registered and those on the waiting list.
- Let the participants set the number of persons for each 


- Let the parents specify the number of kids for each activity.
- Let new mentors say that they will be mentoring (and the organizers count them).
- Highlight the participants not having yet filled any field.
- There is no security: everybody can fill any field.
- Connect the list to a Meetup event, by simply specifying the event id in the url.
- Only works for one Meetup group at a time (to limit the abuses).
