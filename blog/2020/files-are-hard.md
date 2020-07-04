{"date": "2020-07-03", "title": "Files Are Hard"}

Someone linked to this on HN: [Files Are Hard](https://danluu.com/file-consistency/). It describes the problems that can occur with even the most basic file IO. A naive approach is often fine, but for critical applications doing a lot with files, beware:

> You need to checksum your data since you will get silent errors and corruption. The only questions are whether or not you detect the errors and whether or not your record format only destroys a single record when corruption happens, or if it destroys the entire database. As far as I can tell, most desktop email client developers have chosen to go the route of destroying all of your email if corruption happens.