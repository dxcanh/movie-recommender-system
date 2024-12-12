# Movie Recommendation System

## Quick Start

To deploy an example HDFS cluster, run:
```
  docker-compose up -d
```

## Ensure your Hadoop cluster is running

## Execute the Recommender Engine
```
hadoop jar recommender-engine/recommender.jar Driver movie-dataset/movie_rating_cut.txt movie-dataset/movie-titles.txt /dataDividedByUser /coOccurrenceMatrix /Normalize /Multiplication /Sum /RecommendationList /RecommendationListName /RecommendName
```
## Copy output file to local
```
hadoop fs -get / ~/Bigdata-Movie-Recommendation/output
```
