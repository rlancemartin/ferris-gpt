# Ferris GPT

This app enables AI-powered search for Tim Ferris podcast.

## Dataset
 
Transcripts here - 
https://tim.blog/category/the-tim-ferriss-show-transcripts/

All steps outlined in -
`scripts/make_index.ipynb`
 
TO DO: Add 1-151 -  
https://tim.blog/2018/09/20/all-transcripts-from-the-tim-ferriss-show/?utm_source=redirect&utm_medium=redirect&utm_campaign=redirect

## Search

Use Langchain `VectorDBQAChain` to - 
* Embed the user query
* Perform similarity search on Pinecone embeddings
* Synthesize the answer from relevant chunks with `GPT 3.5`

## Search

Relevant chunks with metadata (links) are displayed as source documents.
 
This builds on the excellent UI from https://github.com/mckaywrigley/wait-but-why-gpt.

## Deploy

Deploy to Fly.io.

## Credits

Thanks to [Mckay Wrigley](https://twitter.com/mckaywrigley) for open-sourcing his UI.
 
Thanks to Tim Ferris for the excellent podcast and transcripts.

## Local testing

`yarn dev`

## Contact

If you have any questions, feel free to reach out to me on [Twitter](https://twitter.com/RLanceMartin)!
