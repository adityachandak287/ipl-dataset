# IPL Dataset

Simple node.js app to display IPL dataset using express, mongoDB and server side rendering using ejs.

## Screenshots

|                        | 2008 Season                                  | 2016 Season                                  |
| :--------------------: | -------------------------------------------- | -------------------------------------------- |
|         Table          | <img src="images/2008-home.png" width=480 /> | <img src="images/2016-home.png" width=480 /> |
| Mumbai Indians Matches | <img src="images/2008-MI.png" width=480 />   | <img src="images/2016-MI.PNG" width=480 />   |

## How to run project locally

### Populate mongoDB (needs to be done only once)

Extract zip file drom `data` folder and run the following command to import CSV file into mongoDB.

```cmd
mongoimport --type csv -d ipl -c matches matches.csv --headerline
```

Run python script from `scripts` folder to make Table collection in mongoDB

```cmd
python3 makeTableCollection.py
```

### Run server

```
npm start
```

Navigate to http://localhost:3000/.

## Resources

Dataset can be found [here](http://hck.re/A1Fz4c).
