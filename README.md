#SteamNLPProject

## Project Summary

This project was my first attempt at creating my own deep neural network from scratch. I chose to apply this technology towards a hobby of mine, video games.

Steam is a PC platform service that allows users to buy games and have them all available to download through their library. For each game, there exists a store page that has general info about the game as well as user reviews and an overall rating for it. Each review includes a body of text, a score based on how helpful/funny other users find it, and a thumbs up/down rating.

Using a bag of words style approach, I downloaded a json array of user reviews through steam's API. I then formatted and cleaned the data, built an encoder on the body of text, and passed it into an embedding layer and recurrent neural net. Ultimately, the network is capable of learning how specific words can be used to predict the overall sentiment of the review.

### Files

I have each part of the process separated into a different notebook for ease of use. There are also two tsv files which can be used to visualize the word embeddings with google's free tool. (http://projector.tensorflow.org/). There are also text files that store the encoder, as well as the raw reviews at different stages of processing.

### Future Goals

Currently, the api request only takes a single game ID, I would like to feed lists at some point, although pulling from too many games will mean losing a lot of significant game-specific words.
