## place search happy path
* greet
  - utter_greet
* mood_great
  - utter_happy
  - utter_how_can_i_help
* seach_places_query{"place_type":"atm", "location":"Patna"}
  - action_place_search
* goodbye
  - utter_goodbye

## place search with location
* greet
  - utter_greet
* search_place_query_with_location
  - utter_ask_location
* inform_locations{"location":"patna"}
  - action_place_search
* goodbye
  - utter_goodbye

## sad path 1
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* affirm
  - utter_happy

## sad path 2
* greet
  - utter_greet
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* deny
  - utter_goodbye

## say goodbye
* goodbye
  - utter_goodbye

## bot challenge
* bot_challenge
  - utter_iamabot
