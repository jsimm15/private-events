# README

Odin Project: Private Events - Ruby on Rails

The purpose of this project is to build a functional event planning app in Rails,
focusing on creating the appropriate Active Record associations in order to establish
the many-to-many relationships between User and Event models. The app also uses Devise 
to handle user sign-in.

The app consists of two primary models, User and Event, with a third intermediary model,
Event_Lists, to handle the :through(many-to-many) relationship between Event and User.

Each event has a single creator and event list, and can be attended by multiple attendees(users).
Each user can create and attend multiple events. 

The app's root path will be the Event model's index page, listing all created events. The Event's
show page will list all the attendees for the event. The User's show page will display a list of
all events created by that user, as well as a list of that user's attended_events. 
