

Currently running on heroku, in https://bus-stop.herokuapp.com/ | https://git.heroku.com/bus-stop.git
You can post data into any widget, i.e. to change the welcome message:

post the raw json to http://bus-stop.herokuapp.com/widgets/welcome
{ "auth_token": "", "text": "lookie" }

to change the jobs list:

http://bus-stop.herokuapp.com/widgets/jobs
{ "auth_token": "", "items":[{"label":"label name","value":"value"},{"label":"label2","value":"value2"}] }

where you can replace welcome with the name of any widget and pass any data- attribute in the json, i.e. text/title/more-info

to make the videos go, just pass it on the url via a curl command or similar i.e. this will work:

Full-Screen:
bus-stop.herokuapp.com/api/youtube/show?url=https://www.youtube.com/watch?v=EXc1-WheCd0&index=1&list=PLiqUtLfTLPR9ya-K1gTzscM7acSq1Smag
