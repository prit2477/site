---
title: Use the database
permalink: /utilizing/writing-code/use-the-database/
course: utilizing # There are 4 courses: introduction, fundamentals, utilizing, adopting
chapter_number: 02 # The sections in each course are called chapters
chapter: Writing code # Each chapter has a name
lesson_number: 0130 # The numbers for lessons are incremented in counts of 10 for the most part. I did that so I could swoop in videos in the middle without renaming anything. Probably best to not use these numbers anywhere in the UI
lesson_id: f34238344b71 # Every lesson has a uniq ID
video_url: https://vimeo.com/259610299
type: video # Can be video, assignment, or quiz. Quizez are not ported for now. Assignments are just videos with a different icon
discussion_id: f34238344b71
---
# Resources
## Links
* [The client](https://store.docker.com/community/images/jfahrer/checker-u-dev-a3)

## The SQL statment
```
INSERT INTO requests (ip, path, host, requested_at)
VALUES ('127.21.0.4', '/', '8e358f1ba0db', '2018-01-09 10:38:10 +0000');
```