# GettingStarted

# Recommended Engine IDs
### English Transcription - `1379a425-67ac-4546-89b6-034b2b18ff1a`
### Optical Character Recogniton - `9a6ac62d-a881-8884-6ee0-f15ab84fcbe2`
### General Object Recogniton - `619d7252-d473-b42c-96c6-5675b5e56afd`
### Sentiment Analysis - `104a6b61-5d7d-8a1c-fa32-d37b4c931e7c`
### Face Recognition - `3f115b93-97be-46f0-b0f2-7460db15ec34`
### Face Detection -   `84b513bd-d64d-3a35-9d42-579c8611fdbf`


## Create TDO with Asset
``` mutation{
createTDOWithAsset(input:{
  startDateTime:1521052518
  stopDateTime:1521052518
  uri:"https://www.popsci.com/sites/popsci.com/files/images/2017/08/depositphotos_3979974_original.jpg"
}) {
  id
}

}
```
## Create Job with targetId from Create TDO

```
mutation{
  createJob(input:{
    targetId: "1234566"
    tasks:[{
      engineId:"1379a425-67ac-4546-89b6-034b2b18ff1a"

    }, 
    {
      engineId:"FAVORITEENGINEID"

    }]
  }){
    id
  }
}

```
