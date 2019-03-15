# groucho_wasm

This is a demo project to try out go and webassembly. 
The code grouchifies an image by placing a groucho mask on the face of a person in that image.
For instance here you can see an image of groucho marx being grouchified.

![alt-text](https://cdn.jsdelivr.net/gh/bitsmag/groucho_wasm@master/grouchified_groucho.gif "groucho wasm")

After cloning the repo you can 

run
‘GOOS=js GOARCH=wasm go build -o main.wasm‘
to compile to wasm

run 
‘goexec 'http.ListenAndServe(":8080", http.FileServer(http.Dir(".")))'‘
to serve the files

and visit
‘localhost:8080‘
to grouchify an image